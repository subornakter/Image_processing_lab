## LAB1,2


## Reading, Displaying, and Inspecting a Digital Image
 Using a programming environment of your choice (e.g., Python with OpenCV/PIL, or MATLAB), read any digital image file from disk, display it on screen, and print its width, height, number of color channels, and data type (e.g., 8-bit unsigned integer). Repeat for one grayscale image and one color image, and note the differences in the reported properties.

## Converting a Color Image to Grayscale
 Load a color (RGB) image, convert it to grayscale using your programming environment's built-in function, and display the original and grayscale versions side by side. Report the change in the number of channels and the data size (in bytes) before and after conversion.

Classifying an Unknown Image Write a program that accepts any image file as input and automatically determines whether it is a binary image (only two possible pixel values), a grayscale image (single-channel intensity values), or a full-color image (multiple channels), printing the result along with the reasoning (e.g., "detected 2 unique pixel values, so this is a binary image").

## Surveying Imaging Modalities 
Collect five sample images, each from a different imaging modality discussed in Chapter 1 (for example: an X-ray, a satellite/remote-sensing image, a microscopy image, an ultrasound image, and an infrared image). For each, load it into your program, display it, and write one sentence stating its modality and one real-world application area for that modality.

Thresholding a Grayscale Image into Binary Read an 8-bit grayscale image. Ask the user for a threshold value between 0 and 255. Create and display a binary image in which every pixel with intensity greater than or equal to the threshold becomes white (255) and every pixel below it becomes black (0). Test with at least three different threshold values and compare the results.

## Observing the Checkerboard Effect (Spatial Resolution)
  Take any grayscale image and resample it to reduce its spatial resolution to 128×128, 64×64, 32×32, and 16×16 pixels, while keeping the intensity resolution fixed at 8 bits (256 gray levels). Display all four results alongside the original, and describe in one paragraph the blocky "checkerboard effect" that appears as resolution decreases.

## Observing False Contouring (Intensity Resolution) 
Take any grayscale image with smooth intensity variations (e.g., a face or sky region) and reduce its number of gray levels from 256 down to 128, 64, 32, 16, 8, 4, and 2, while keeping the spatial resolution unchanged. Display the results and describe the "false contouring" (banding) effect that becomes visible, especially in smoothly shaded areas.

## Comparing Image Interpolation Methods 
Take a small image (e.g., 64×64 pixels) and enlarge it four times its original size using three different interpolation methods: nearest-neighbor, bilinear, and bicubic. Display the three enlarged results side by side and describe, in your own words, the visible quality difference between them (blockiness vs. smoothness).

## Computing and Interpreting an Image Histogram 
Write a program that reads a grayscale image, computes its histogram (the count of pixels at each intensity level from 0 to 255), and plots it as a bar chart. Test the program on a dark image, a bright image, and a low-contrast image, and state for each one whether the histogram confirms your visual impression.

## Finding Pixel Neighbors 
Write a function that takes an image and a pixel coordinate (x, y) as input, and returns three sets: its 4-neighbors N4(p), its diagonal neighbors ND(p), and its 8-neighbors N8(p). Make sure the function correctly handles pixels on the image border or in a corner, where some neighbors do not exist. Test it on a pixel in the middle of the image, one on an edge, and one in a corner.

## Computing Distance Measures Between Pixels 
Write a program that takes the coordinates of two pixels as input and computes the Euclidean distance, the city-block distance (D4), and the chessboard distance (D8) between them. Verify your program's output by calculating at least two test cases by hand and comparing them to the program's result.

## Image Arithmetic and Change Detection 
Write a program that performs pixel-by-pixel addition, subtraction, multiplication, and division between two images of the same size. Then, using two nearly identical images (e.g., the same scene photographed a few seconds apart, or one image with a small object added), use image subtraction to highlight only the region where the two images differ.

## Noise Reduction by Image Averaging 
Take a single clean image and generate 20 noisy copies of it by adding random Gaussian noise independently to each copy. Average all 20 noisy copies together pixel by pixel. Display one individual noisy copy next to the final averaged result, and explain why averaging reduces the visible noise.

## Set and Logical Operations on Binary Images
Create two binary images of the same size, each containing a simple shape (e.g., a white circle and a white square that partially overlap). Write a program to compute and display the AND, OR, NOT, and XOR of the two images, and describe what each result represents in terms of the two original shapes.

Basic Geometric Transformations Write a program that applies the following transformations to an input image, one at a time: (a) translation by a given number of pixels in the x and y directions, (b) rotation by a given angle in degrees around the image center, and (c) scaling by a given factor. Display the original image alongside each transformed version, and note any empty (black) regions that appear as a result of the transformation.
