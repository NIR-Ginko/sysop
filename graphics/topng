#!/bin/sh
# По умолчанию обрабатывает JPEG.
for file in `ls *.jpg *.JPG *.gif *.GIF *.tif *.tiff`
do
var="`echo ${file%.*}`"
convert "$file" "$var.png"
rm -f "$file"
done
