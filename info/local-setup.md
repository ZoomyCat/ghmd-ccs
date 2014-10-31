## How to install ghmd-ccs dependencies?

### What do I need?

#### ruby
```
pacman -S ruby
apt-get install ruby
yum --install ruby
```
#### github-markdown & github-markup
```
gem install github-markdown
gem install github-markup
```

## You will get a warning similar to this:
WARNING: You don't have `/home/username/.gem/ruby/2.1.0/bin` in your PATH,
gem executables will not run.

To fix this you will need to add the location given in the warning above to your `~/.profile` file with to file as shown below.

```
PATH="$PATH:/home/username/.gem/ruby/2.1.0/bin:"
export PATH
```

Your computer is now configured with all dependencies required to be able to run ghmd-css.

#### Next!
[Create a compatible website.](create-website.html)
