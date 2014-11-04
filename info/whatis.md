### What is ghmd-ccs?

ghmd-ccs is an unofficial GitHub Markdown to HTML Content Creation System.

### What does it do?

This suite of scripts will be used in being able to dynamically generate websites from a template html file and the content will be pulled in by .md files. If the name of the .md file is README the name of html file will be index.html. If the name is anything other than README it will created a index file with a corresponding name, eg `info.md` will become `info.html`.

The html files created in this process will overwrite the previous versions, No need to backup since your previous version is your previous git commit.