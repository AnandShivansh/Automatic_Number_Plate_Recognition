## Automatic_Number_Plate_Recognition
- Used PyTesseract OCR Reader.
- Takes an image, applies blurring, uses sobel to get horizontal lines. Then returns the binarized image.
- Gets the countours that most likely resemeber the shape of a license plate.
- Inspects the ratio of the contour to ensure it meets the requirements suitable to a real license plate.
- Checks the average color of the potential plate and if there is more white than black colors it returns true.
- Checks the angle of the rectangle potential license plate.
- Takes the extracted contours and once it passes the rotation and ratio checks it passes the potential license plate to PyTesseract for OCR reading.
