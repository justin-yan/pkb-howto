# Dotfiles

If you're following [One Folder](../principles/one-folder.md), then your PKB is a great place to put your [Dotfiles](https://github.com/webpro/awesome-dotfiles).  Configuring a new machine can look as simple as:

1. Synchronize your PKB.
2. Deploy your dotfiles.
3. You're ready to be productive!

There are a [variety of ways to do this](https://github.com/webpro/awesome-dotfiles#tools), so we'll just look at a dead-simple setup, and you can add more advanced tools to your heart's content.

### Bash and Symlinks

The idea here is pretty simple.  Assuming you have a folder `~/pkb/Dotfiles/` , what we want to do is to put your actual dotfiles in this folder, and then _symlink_ them to where the applications are expecting to find them.  Here's a very crude version of what this might look like:

```text
~/pkb/Dotfiles$ ls -a
.bash_justin  install.sh  git/  sublime/
```

When I set up a new computer, the first thing I do is synchronize my PKB, and then I run the `install.sh` script above, which does the following:

{% code title="install.sh" %}
```text
#!/usr/bin/sh

# link dotfiles
export DOTFILES_DIR=/home/justin/pkb/Dotfiles
ln -f -n -s $DOTFILES_DIR/git $HOME/.git
ln -f -s $HOME/.git/.gitconfig $HOME/.gitconfig
mkdir -p $HOME/.config/sublime-text-3/Packages
ln -f -n -s $DOTFILES_DIR/sublime $HOME/.config/sublime-text-3/Packages/User

# Add utility env-vars and utility bash aliases/functions
if ! grep .bash_justin ~/.bashrc ; then
    echo "if [ -f \$DOTFILES_DIR/.bash_justin ]; then" >> ~/.bashrc
    echo "    . \$DOTFILES_DIR/.bash_justin" >> ~/.bashrc
    echo "fi" >> ~/.bashrc
fi
```
{% endcode %}

This is an idempotent script \(the `-f` and `-n` flags are important\), and so if you discover a new set of dotfiles to preserve, e.g. `.my.cnf`, move it into the Dotfiles folder, add the corresponding symlink command to the install script \(`ln -f -s $HOME/.my.cnf $DOTFILES_DIR/.my.cnf`\), and then re-run the install script.

Now, if any of your configurations change, they'll automatically be preserved in your PKB and propagate across all of your devices.

