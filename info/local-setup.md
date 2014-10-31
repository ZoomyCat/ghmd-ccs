## How to install ghmd-ccs dependencies?

### What do I need?
Name | Command to get it.
----|----
ruby | `pacman -S ruby`
github-markdown | `gem install github-markdown`
github-markup | `gem install github-markup`

## You will get a warning similar to this:
WARNING: You don't have `/home/username/.gem/ruby/2.1.0/bin` in your PATH,
gem executables will not run.

To fix this you will need to add the location given in the warning above to your `/etc/profile` file with the following format.

```
PATH="$PATH:/home/username/.gem/ruby/2.1.0/bin"
export PATH
```

Your computer is now configured with all dependencies required to be able to run ghmd-css.

#### Next!
[Create a compatible website.](create-website.html)
