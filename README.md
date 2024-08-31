# Alternative Simple Project 1: Modifying YOLOv1 to Detect Circles Instead of Rectangles

This project serves as an alternative to the basic Project 1 and is designed for students who may find the original project challenging. The goal is to modify the YOLOv1 architecture to detect circular bounding shapes around objects instead of the standard rectangular boxes. This approach simplifies certain aspects of object detection while still providing a solid learning experience in modifying deep learning models.

**Note:** This project is based on the YOLOv1 implementation available in this [repository](https://github.com/saebswaity/YOLO).

## Steps Involved:

1. **Dataset Modification**: 
   - You will begin by creating a new labeled dataset where each object's bounding box is represented as a circle.
   - Replace the original rectangle representation `(x_center, y_center, width, height)` with a circular one `(x_center, y_center, radius)`.

   The radius is calculated using the formula:
r_c = sqrt((h^2 + w^2)) / 2

   where `h` is the height and `w` is the width of the original rectangular bounding box.

2. **YOLOv1 Architecture Update**:
- Modify the YOLOv1 network's head to predict the parameters of a circle instead of a rectangle.
- Update the loss function to handle the circular representation, focusing on minimizing errors in predicting the circle’s center and radius.

3. **Label Visualization**:
- Change the code responsible for drawing labels on images to render circles instead of rectangles using the new format.

This project is designed to provide a simpler alternative while still allowing you to engage with important concepts in deep learning and computer vision.

Good luck! 🙂


