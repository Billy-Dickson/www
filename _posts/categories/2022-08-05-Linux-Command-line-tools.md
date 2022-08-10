---
layout: single
title:  "exiftool - Remove exif data from photos"
date:   2022-08-10 13:37:08 +0000
categories: Computing Linux Homelab
publish: false
---

## How to remove exif data from photos

Here's a handy linux command line tool that removes exif data from photographs, This one I use to remove the exif data from photos before I publish them to my website. Removing EXIF is a smart idea, particularly if you're especially privacy-conscious however, as we mentioned, your biggest concern is most likely the geolocation information.

### Install the appication

~~~bash
sudo apt install exiftool
~~~

### Show the metadata

~~~bash
exiftool photo.jpg
~~~

### Show metedata for all *.jpg files. Note: The extension is case sensitive

~~~bash
exiftool -ext jpg
~~~

### Same as above, but include sub directories

~~~bash
exiftool -r -ext jpg .
~~~

### Remove all metadata

~~~bash
exiftool -all= -overwrite_original photo.jpg
~~~

### Remove all metadata of all *.jpg files in the current directory

~~~bash
exiftool -all= -overwrite_original -ext jpg
~~~

### Does the same as above, but includes subdirectories

~~~bash
exiftool -all= -r -overwrite_original -ext jpg .
~~~

### Remove all GPS metadata of *.jpg files in the current directory

~~~bash
exiftool -gps:all= *.jpg
~~~

## References

1) [Linux Nightly](https://linuxnightly.com/how-to-remove-exif-data-via-linux-command-line/)

2) Removing exif data using [other operating systems](https://www.howtogeek.com/203592/what-is-exif-data-and-how-to-remove-it/)