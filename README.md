GaugeReader
GaugeReader is an image classification model that provides three levels of output - High, Medium, and Low - based on the readings from a specific gauge. The model is trained using Keras and can be run on a PC connected to an Arduino board.

Requirements
To use GaugeReader, you will need the following:

Python 3.6 or later
Keras 2.2.5 or later
TensorFlow 1.14 or later
PySerial 3.4 or later
An Arduino board
An LED connected to Digital Pin 11 (positive) and ground (negative)
Installation
To install GaugeReader, you can clone the repository using the following command:

bash
Copy code
git clone https://github.com/<username>/GaugeReader.git
Once you have cloned the repository, you need to make sure that you have the required packages installed. You can install them using the following command:

bash
Copy code
pip install -r requirements.txt
Usage
To use GaugeReader, you need to follow these steps:

Connect your Arduino board to your PC using a USB cable.

Choose the correct COM port for the Arduino using device manager.

Make sure that the keras_model.h5 file and labels are in the open folder or change their path accordingly.

Set up an LED on digital pin 11 of the Arduino board for the positive connection and ground for the negative connection.

Run the gauge_reader.py file using the following command:

bash
Copy code
python gauge_reader.py
This will open the camera and start capturing images of the gauge.

Place the gauge in front of the camera and wait for the LED to light up with the corresponding reading level.

Contributing
If you want to contribute to GaugeReader, feel free to submit a pull request. We welcome any contributions that can help improve the accuracy and efficiency of the model.

License
GaugeReader is licensed under the MIT license. You are free to use, modify, and distribute the code as long as you include the original license in your distribution.

