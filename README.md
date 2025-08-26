# ECE 515 Course Website 

author: itabrah2@ilinois.edu

## Fall 2025

This is the repository for the ECE 515 website for the Fall 2025 offering of
the course. This repostiory uses the [Quarto](https://quarto.org/) publishing system. 

To preview the website, simply install the Quarto engine and run on the
command line (while in the root folder of the repository)

```
quarto preview
```

Quarto should launch a preview of the website in a browser. 

### Scribing

You must sent in a `.qmd` file to be used with the format of the website for extra credit. You may use TikZ, Visio, InkScape etc. to draw figures. 

## Publishing 

When the website is ready to be deployed, run:

```
quarto render
```

from the root folder. This will create a folder `_site` within the root folder.
The contents of this folder can be simply copied over to the destination. For
example (for Instructors, **NOT** for scribes):

```
rsync -avzh --progress _site/ sftp.courses.grainger.illinois.edu:/ece515/fa2025/
```

