# CellFinder
Finds regions of interest (ROIs) in an image based on pixel intensity and size. This script was used to detect acrosomes (labeled with GFP) in sperm cells, which are critical for the fertilization process.

The image is first read and high-pass filtered to ignore low-frequency features such as bubbles and dirt. Then, a threshold is found using Otsu's binarization process. The threshold minimizes variance within-class and maximizes variance across class.

![download](https://github.com/user-attachments/assets/5cbb5a7a-984c-4865-a9a7-041e396ce82d)

Next, regions of interest (ROIs) are found of connected pixels using the OpenCV package. The distribution of ROI sizes are dispalyed.

![download](https://github.com/user-attachments/assets/42da7d86-7b1e-448d-872b-87110d94b09d)

Finally, ROIs with size smaller than the user defined threshold are discarded. The original image is displayed with circles drawn around each ROI.

![download](https://github.com/user-attachments/assets/539719bb-9591-416a-9839-75ddbff3b8b2)
