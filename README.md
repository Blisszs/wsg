# My website generator script

A simple script inspired by another script I found on the web. I didn't really like somethings about it and decided to make my own. It uses pandoc for file conversions and that is about it.

It generates a website by converting markdown files into html and then "sandwich" it together with a footer and header.

## Usage

```console
wsg SOURCE_DIRECTORY DESTINATION_DIRECTORY
```

The base directory where the script is ran must contain the following files: "_footer.html", "_header.html", "_rss.xml" and "_stylesheet.css" (the last one being optional). The _rss.xml file will must contain the beginning of your rss until the first item tag.

The SOURCE_DIRECTORY is the folder which contains all the markdown files. All markdown files inside will be converted to html and will retain the same name (only the file extension changes). It also must contain a directory called exactly "blog". The blog directory must contain all the markdown files you intend to post as a blog. All of posts will be displayed on a file named blog.html and will be added to the rss.xml file.

The end result of the script will be in the DESTINATION_DIRECTORY.
