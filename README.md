# Unstitcher
An image unsticher originaly made for Minecraft.

This was made a long time ago when Minecraft was moving from texture sheets to individual images per thing.

I am only now uploading it as it may be usfull to others.

## How To
The program is expecting an image in .png format and a text file with extension .config of the same name.

There can be multiple pairs of these files.

It is expecting them to be in the same folder as the .jar file.

The .png image is expected to be a 16 x 16 set of images.

The resolution of the image does not matter as long as it is divisible by 16.

The file has no UI and does not show any progress bar when running.

## Config
The config file has several setup options.

The first line should be "output=/".

You can add a folder path to this but it must end in "/".


Next are the icon locations.

This is done with the row then collom seperate with a "." followed by an "=" and then the filename without an extension.

The file names can have spaces.

Example:

3.5=Testing


You can comment our lines by starting them with a "*".

Example:

*3.5=Testing


You can setup an array of images to be exported as one image with "-".

This will be noted as the upper left location and the lower right location seperated by a comma.

Example:

-3.5,5.6=Testing Long


## Output Notes
The config name can also be a filepath then filename to have images go to different locations.

This filepath will be added to the master output path noted on the first line.

Example:

5.6=icons/Test

If the unsticher finds a file with the same name that it is trying to create it will check if the files are the same.

If the files are the same it will do nothing, if they are different then it will override the file.
