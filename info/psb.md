### psb

psb is short for push sidebar. It will be used to push the sidebar from the main website to other sub websites.

### Design.

#### Files.

As usual I will probably have a main program that does the work and a config file that holds the information needed to run the program. The configuration file makes it easy to modify how the program operates to fit your needs.

Name | Description
---- | ----
psb | This is the main program that pushes the sidebar to the rest of the website.
psb.conf | The config file that allows for easy modification of the layout.

### What will psb.conf contain?

Variable name | Type | Description
---- | ---- | ----
main_site | Variable | Contains the name of the main website. In the context of edge226.github.io that is what would be contained here.
sub_sites | Array | This will contain a listing of all sub websites that are to be updated with a new sidebar menu. The template sidebar.html and sidebar.emmet will be replaced with ones from the main_site.
site_dir | Variable | This dictates the location of the main_site and sub_sites.
update_files | Array | For my usage this will only contain sidebar.* but could contain anything that may need to be updated through the ghmd-ccs [template system](about-templates.html).

### How does the program work?

The program is extremely simple, It copies files from a main website template directory into sub website template directories.

The program will copy $site_dir/$main_site/template/$update_files into $site_dir/$sub_sites/template/ using rsync.
