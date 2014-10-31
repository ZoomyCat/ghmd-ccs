## Steps to configuring website on gihub.io to work with ghmd-ccs.

For a basic setup this is very easy:

1. Create a directory called `template` in the root of your website.

2. Copy the original `index.html` file into the `template` directory.

3. Make a duplicate of the `template/index.html` called `index-template.html` in the `template` directory.
  * At this point your `template` directory structure should look like this.
    * `template`
    * `template/index.html`
    * `template/index-template.html`

4. Setup your `.gitignore` file.
  * Create a file called `.gitignore` in the root directory of your website if it does not already exist.
  * Modify `.gitignore` and add `ghmd-ccs` to the file.
    * This makes sure ghmd-ccs is not added to your website.

#### Next!
[Clone ghmd-ccs into the website.](clone-ghmd-ccs.html)
