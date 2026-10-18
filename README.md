# NumPy Image Pixel Manipulator

Made for my Essentials of AI (Core) course.

An image is just a grid of numbers, so in this project I edit one using only NumPy, with no loops and no image editing apps. I made an Indian flag from scratch and played around with it.

## What it does
- Creates a 200x300 RGB image using `np.zeros` and `np.full`
- Draws the stripes and the blue chakra square using array slicing
- Crops it, mirrors it, flips it upside down, and pulls out just the red channel
- Makes it brighter and darker (converts to `float32` first so `uint8` doesn't overflow)
- Uses a boolean mask to count bright pixels
- Compares memory of `uint8` vs `float64` (180,000 bytes vs 1,440,000 bytes, so 8x)

## Screenshots
<img width="847" height="422" alt="image" src="https://github.com/user-attachments/assets/e409be58-6f29-472c-82a4-b17bc236a914" />
<img width="841" height="168" alt="image" src="https://github.com/user-attachments/assets/ef9fcc1d-62b1-4364-b92e-fba59698f179" />
<img width="846" height="225" alt="image" src="https://github.com/user-attachments/assets/78a31feb-f2ef-479c-acd3-d7a46507fda6" />


## Run it
Click the **Open in Colab** badge at the top of the notebook and run all cells. Only NumPy and Matplotlib are needed, and both come preinstalled in Colab.

## What I learned
- An image is a 3D array (height, width, colour)
- Slicing can crop and flip without loops
- `uint8` overflows if you do maths on it directly
- `uint8` uses 8x less memory than `float64`

## Tech
Python, NumPy, Matplotlib, Google Colab
