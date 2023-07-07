# Image Resizer

This Python script utilizes OpenCV and the `simple_image_download` library to download and resize images from a website. It allows you to easily fetch a specified number of images related to a particular search term and resize them to 50% of their original size.

## Instructions

1. Install the required dependencies
   
2. Download the script file, `image_resizer.py`, and place it in your desired working directory.

3. Create an input folder in your working directory to store the downloaded images. You can name it as per your preference, such as `flowers_garden`.

4. Open the `image_resizer.py` file in a text editor and make the following modifications:

- Set the `limit` variable to specify the number of images you want to download. By default, it is set to 100.

- Optionally, adjust the search term in the `response().download('flowers_garden', limit)` line to search for images related to a different term. 

5. Run the script using the command:

python image_resizer.py


The script will start downloading the images and display the progress in the console.

6. After downloading the images, the script will create an output folder named `output_images` in your working directory.

7. Each downloaded image will be resized to 50% of its original size using OpenCV and saved in the output folder.

8. The console will display the progress of resizing and the path where each resized image is saved.

## Code Explanation

The code is divided into the following sections:

- **Imports**: It imports the necessary libraries, such as `cv2` (OpenCV), `os`, and `simple_image_download` for image downloading.

- **Downloading Images**: The script uses the `simple_image_download` library to download images based on a search term and saves them in the input folder.

- **Resizing Images**: The `resize_images` function iterates over each downloaded image, reads it using OpenCV, resizes it to 50% of its original size, and saves the resized image to the output folder.

## Usage

You can use this script to quickly download and resize images for various purposes, such as building datasets, creating thumbnails, or preparing images for machine learning tasks.

The default search term is "flowers," but you can customize it according to your requirements by modifying the `response().download('flowers_garden', limit)` line in the script.

## Limitations

- The script relies on the `simple_image_download` library to fetch images from the web. The quality and availability of images may vary based on the search term and the sources from which the library fetches the images.

- The resizing operation uses OpenCV's `cv2.resize` function with bilinear interpolation. You can modify the interpolation method or resize parameters according to your needs.

## References

- OpenCV: https://opencv.org/
- `simple_image_download` library: [GitHub Repository](https://github.com/RiddlerQ/simple_image_download)






