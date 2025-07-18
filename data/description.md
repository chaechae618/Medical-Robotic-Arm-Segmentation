1. Original Image (RGB)
- Color image of the robot arm captured with a high-resolution camera.
- Used as input to the segmentation model.

2. Label File (.txt)
- Each line represents a polygon indicating the boundary of a part of the robot arm.
- Every polygon starts with 0, which is the class ID for the robot arm.
- These polygons are later merged into a single PNG mask.

3. Mask Image (PNG)
- White (255): Robot Arm area
- Black (0): Background area
- All polygons from the label file are combined into one binary mask image.
- Used as the target label for segmentation training.
