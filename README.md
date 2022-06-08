# ImageToAscii
convert jpg imgs to ascii text image art

notebooks collects the process of creating the functionality and help to understand what's going on
.py are the main programs

*ImageToAsciiOP.py*:
it transforms given jpg image into a string of ascii caracters so when pasting it in a txt or so you can see the whole picture 
params:
    *path_in*: where the picture
    *path_out*: where the output
    *invert*: false if u are using dark background, true if light
    *resolution*: a ratio of compression of the photo (0,1] recomended around 0.1 depends on the size of the pic
    *contrast*: a ratio of contras pre aplied to image, (0,inf) contrast > 1 more contrast and <1 less
    
to call the program just run:
python imageToAsciiOP.py <path_in> <path_out> <resolution> <contrast> <invert>
example:
python ImageToAsciiOP.py imgs/modus.jpg out/canvas.txt 0.1 1.7 true
  
*asciiToImage.py*:
it transforms the output file from ImageToAsciiOP to a jpg picture so you can take your creation as a picture instead as a .txt 
params:
    *path_in*: where the .txt
    *path_out*: where the output
    *backGround_color*: rgb like background color
    *font_color*: rgb like font color
    
to call the program just run:
python asciiToImage.py <path_in> <path_out> <red_Back> <green_Back> <blue_Back> <red_Font> <green_Font> <blue_Font>
example:
python asciiToImage.py out/canvas.txt out/canvas.jpg 216 075 032 0 0 0
  
