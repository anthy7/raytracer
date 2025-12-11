# PPM

PPM is an image format. It's short for portable pixmap.

## Example

P3
3 2
255
255 0 0 0 255 0 0 0 255
255 255 0 255 255 255 0 0 0

## Explanation

P3 - means colours are in ASCII (P6 would've meant it was in binary)
3 2 means there's 3 columns, and two rows - i.e. the dimensions of the image, width x height
The following 255 means the max colour is 255, and signifies RGB triplets.
The following triplets represent a grid that looks like
Red Green Blue
Yellow White Black
