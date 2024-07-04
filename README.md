# Gimbal-using-Aruino
A gimbal is a device that allows an object to rotate around an axis. It is commonly used in cameras to stabilize the footage by counteracting the movements and vibrations. Building a gimbal with an Arduino Nano, MPU6050, MG996R servo motors, and a buck converter involves several components and steps.

Arduino Nano - A compact microcontroller board based on the ATmega328P, used to process data and control the gimbal.

MPU6050 - An Inertial Measurement Unit (IMU) sensor that includes a gyroscope and accelerometer. It provides real-time orientation and acceleration data.

MG996R Servo Motors - High-torque servo motors used to control the movement of the gimbal’s axes (pitch, roll, and yaw).

Buck Converter - A DC-DC converter used to step down voltage to a level suitable for the Arduino and other components.

**Working of the Gimbal**:
The MPU6050 sensor measures the orientation and acceleration of the gimbal. It provides data on pitch, roll, and yaw angles.
The Arduino Nano reads the data from the MPU6050 sensor and processes it.
Based on the processed data, the Arduino Nano sends PWM (Pulse Width Modulation) signals to the MG996R servo motors. These signals control the position of the servos, adjusting the gimbal to stabilize the camera.
The buck converter ensures that all components receive the correct voltage. It steps down the input voltage from a battery or power supply to the levels required by the Arduino Nano and the servos.
