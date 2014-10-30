ghmd-ccs is an unofficial GitHub Markdown to HTML Content Creation System.

### Dependencies
Name | On GitHub
---- | ----
ghmd2html | [github-markup](https://github.com/github/markup).
      | [github-markdown.](http://github.github.com/github-flavored-markdown/)

### [What feature is next?](plans)

Click the link above to see what feature I am thinking of working on next!

### Whats it do?

This suite of scripts will be used in being able to dynamically generate websites from a template html file and the content will be pulled in by README.md files.

The html files created in this process will overwrite the previous versions, No need to backup since your previous version is your previous git commit.

#### Some things to consider:

* I recommend adding "ghmd-cms" to the .gitignore file for your project if you clone directly into your project.

### How to use it?

If you cloned ghmd-cms into your website directory and added ghmd-cms to your .gitignore to ensure you will not re-upload ghmd-cms into your repository. This will ensure that ghmd-cms does not dirty your upload directory.

I do not suggest running ghmd2html manually. It is really just a library for update to call.

Usage is simple.

```
update
```

After that add and commit your index.html and README.md and your website will be up to date with the new content you just created, All in a more user friendly language.
