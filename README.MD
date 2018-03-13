# Digital Mishnah

The Digital Mishnah Project aims to create a digital critical edition of the Mishnah. This will involve transcribing and encoding major (ideally all) manuscript witnesses to the text of the Mishnah, as well as citations in medieval and early modern commentaries.

* Provide digital renditions of manuscript witnesses
* Ability to show witnesses synoptically
* Ability to provide computer-processed collation of variants
* Statistical tools for measuring proximity or distance of witnesses

This is the TEI data for the project. The eXist web application code is located at [this GitHub repository](https://github.com/umd-mith/mishnah).

# Suggested workflow for eXist and GitHub

The repository includes an `ant` script to synchronize data between the database and a repositroy clone.

To commit changes to GitHub:

* run `ant get` to export data from the database
* commit and push changes to GitHub

To get changes from GitHub:

* pull from GitHub
* run `ant updatedb` to upload to the database (NB the existing data will be replaced)
