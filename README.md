**Dataset Description: On-Board Unit Data from an Electric Scooter**

This dataset contains comprehensive data collected from an on-board unit (OBU) mounted on an electric scooter. The data encompasses various scenarios, including:

1. **Static Conditions**: Measurements taken while the scooter is stationary.
2. **Conventional Driving Situations**: Data recorded during regular driving on different types of pavements, such as asphalt, concrete, and gravel.
3. **Lateral Rollovers**: Readings captured during instances of the scooter tipping over sideways.
4. **Frontal Collisions**: Data obtained from front-impact collisions.

The dataset includes parameters such as acceleration measurements, orientation, GPS position, gravity, gyroscopic orientation, illumination, and atmospheric pressure, providing valuable insights into the scooter's performance and safety under different conditions.

**Data Organization**:
- Each folder contains data from a specific test scenario, with a descriptive name indicating the nature of the test.
- Inside each folder, there is a README file that includes relevant details about the conducted test.
- There is a set of files within each folder, one for each collected parameter, in CSV format.
- Additional multimedia files can be included in the form of photos or videos, to understand specific test scenarios.

**File Details**:

The files included regarding the parameters gathered are:

- **Accelerometer.csv**: Contains a timestamp, the number of milliseconds since the recording started, and X, Y, and Z values. The acceleration value for each axis is measured in meters per second squared (m/s²).
- **AccelerometerLinear.csv**: Contains a timestamp, the number of milliseconds since the recording started, and X, Y, and Z values. The acceleration values are measured in meters per second squared (m/s²) and represent the linear acceleration without the influence of gravity.
- **Compass.csv**: Contains a timestamp, the number of milliseconds since the recording started, and X, Y, and Z values that represent the magnetic field strength along the three axes. The heading values given by the compass are measured in microteslas (µT).
- **GPS.csv**: Contains a timestamp, the number of milliseconds since the recording started, and the geographical position in latitude, longitude, and altitude values. The latitude and longitude values are measured in degrees (°), and the altitude values are measured in meters (m). Consider that this file is in blank when an indoor test is performed, or when the GPS signal is not acquired during the test.
- **Gravity.csv**: Contains a timestamp, the number of milliseconds since the recording started, and the acceleration due to gravity along the three axes X, Y, and Z. The gravity values are measured in meters per second squared (m/s²).
- **Light.csv**: Contains a timestamp, the number of milliseconds since the recording started, and an illuminance value. The illuminance values are measured in lux (lx), which is the standard unit for measuring the amount of light that hits a surface.
- **Pressure.csv**: Contains a timestamp, the number of milliseconds since the recording started, and a pressure value. The pressure values are measured in millibars (mbar), which is a common unit for measuring atmospheric pressure.
- **RotationVector.csv**: Contains a timestamp, the number of milliseconds since the recording started, X, Y, and Z values, a cosine value, and a heading accuracy value. The X, Y, and Z values represent the components of the rotation vector in the three-dimensional space and are dimensionless, normalized values ranging from -1 to 1. The cosine value is a scalar component of the quaternion representing the rotation, and the heading accuracy includes an indication of the measurement quality, when available.