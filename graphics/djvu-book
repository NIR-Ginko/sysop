#!/bin/sh
# По умолчанию обрабатывает JPEG.
for file in `ls *.jpg`
do

# Для монохромных изображений:
#anytopnm $file | ppmtopgm | pgmtopbm -value 0.499 > $file.pbm
#cjb2 -dpi 300 $file.pbm $file.djvu

# Для цветных изображений:
anytopnm $file > $file.ppm
c44 -dpi 300 $file.ppm $file.djvu
rm -f $file.ppm
done
djvm -c x.djvu *.jpg.djvu
rm *.jpg.djvu

#see also pngtopnm