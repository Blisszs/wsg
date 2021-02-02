# My website generator script

A simple script inspired by another script I found on the web. I didn't really like somethings about it and decided to make my own. It uses pandoc for file conversions and that is about it.

It generates a website by converting markdown files into html and then "sandwich" it together with a footer and header.

## Usage

```console
sitegen SOURCE_DIRECTORY DESTINATION_DIRECTORY
```

The SOURCE_DIRECTORY is the folder which contains all the markdown files. All markdown files inside will be converted to html and will retain the same name (only the file extension changes). It also must contain a directory called exactly "blog" else the script will not run. The blog folder must contain all the markdown files you intend to post as a blog. All of posts will be displayed on a file named blog.html. At last, the directory must contain a css file named stylesheet.css.

the base directory where the script is run must contain two files called "_footer.html" and "_header.html". These will be utilized to "sandwich" the main content of the page.

The result will be in the DESTINATION_DIRECTORY.
