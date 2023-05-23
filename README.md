# Door-Detection-and-distance-estimation-in-Habitat-Environment



This project focuses on detecting doors in images and estimating the distance from the camera to the detected doors. It utilizes the YOLOv8 object detection model for door detection and depth extraction techniques for estimating distances.

## Prerequisites

Before running the project, ensure that you have the following dependencies installed:

- Python 3.x
- OpenCV
- PyTorch
- NumPy

## Installation

1. Clone the repository:

   ```shell
   git clone https://github.com/Alihassan7212/Door-Detection-and-distance-estimation-in-Habitat-Environment
   ```

2. Change into the project directory:

   ```shell
   cd door-detection
   ```

3. Install the required Python packages:

   ```shell
   pip install -r requirements.txt
   ```

## Usage

1. Add your input images to the `images` directory.

2. Run the door detection script:

   ```shell
   python door_detection.py
   ```

   The script will use the YOLOv8 model to detect doors in the input images. You have to do some chages if you want to train the model on your own dataset

3. Run the depth extraction script:

   ```shell
   python depth_extraction.py
   ```

   This script will use glb files to extract depth information from the scenes.

4. Run the distance estimation script:

   ```shell
   python distance_estimation.py
   ```

   The distance estimation script will utilize the depth information to estimate the distance from the camera to each detected door.

5. View the results:

   The output images with detected doors and estimated distances will be saved in the `output` directory(or the directory you will chose for the output).

## Configuration

- You can modify the detection threshold and other parameters in the `door_detection.py` file to adjust the detection accuracy.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- The YOLOv8 model implementation is based on the [YOLOv8](https://github.com/ultralytics/yolov8) repository.
- The depth extraction techniques are based on the [Habitat-Sim](https://github.com/facebookresearch/habitat-sim) framework.

## Youtube Video
Link: https://youtu.be/vrRd3olJI9Q

## Contributing

Contributions are welcome! Please feel free to open issues or submit pull requests.

## Contact

If you have any questions or suggestions, please contact [your-email@example.com](mailto:alihassanbhatti.b74@gmail.com).

---
Feel free to customize this README file according to your specific project details and requirements.
