# Watermark Generator
The goal of this is to add watermarks to images using OpenCV and Python. To get started, we’ll need a watermark.

## How to use
We require three command line arguments and can supply two additional (optional) ones. A full breakdown of each of the command line arguments can be found below:

- --watermark : Here we supply the path to the image we wish to use as the watermark. We presume that (1) this image is a PNG image with alpha transparency and (2) our watermark is smaller (in terms of both width and height) then all images in the dataset we are going to apply the watermark to.
- --input : This is the path to our input directory of images we are going to watermark.
- --output : We then need to supply an output directory to store our watermarked images.
- --alpha : The optional --alpha  value controls the level of transparency of the watermark. A value of 1.0 indicates that the watermark should be 100% opaque (i.e., not transparent). A value of 0.0 indicates that the watermark should be 100% transparent.
- --correct : Finally, this switch is used to control whether or not we should preserve a “bug” in how OpenCV handles alpha transparency. The only reason I’ve included this switch is for a matter of education regarding the OpenCV library. Unless you want to investigate this bug yourself, you’ll likely be leaving this parameter alone.

## Example usage
Navigate to the code directory and execute the following command:
- python watermark_dataset.py --watermark ankitz007.png --input input --output
Then, view the output images in the output directory.  
Cheers 🍻️
