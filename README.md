File2PNG
========

This is a shell script that stores any file as PNG image. It's based on `convert` util from **Imagemagick**.

### Usage

Store `input_file` as `output_file.png`:

    file2png -c store -i input_file -o output_file.png

Restore file:
    
    file2png -c restore -i input_file.png -o output_file
    

Example container-image:

![output example](https://i.imgur.com/G6MYiXh.png "output example")

Resulting image file size remains almost same.

### Install

Copy `file2png` script to any place where you will run it from (`/usr/local/bin` for example).

Requirements:

* `convert` util from Imagemagick
* `grep`
* `sed`
* `bc`
* `awk`
* `sha256sum`
* `dd`
* `mktemp`
