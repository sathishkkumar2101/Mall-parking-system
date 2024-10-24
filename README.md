# Parking Management System for Malls

## Objective
The Parking Management System aims to enhance the parking experience in malls by providing:
- Real-time detection of parking space availability using IoT sensors.
- A user-friendly web application that displays the availability of parking spots.
- Integration with AWS services for efficient backend management.

## Features
- Detects parking space availability using ultrasonic IoT sensors.
- Provides real-time updates on parking spot availability through a web application.
- Allows users to view available parking spots in real-time.
- Integrates with AWS services such as DynamoDB, Lambda, and IoT Core for backend management.

## System Architecture
The system architecture consists of the following components:

1. **IoT Devices (Ultrasonic Sensors)**: Detect whether a parking spot is occupied or available.
   
2. **AWS IoT Core**: Facilitates communication between IoT devices and the cloud infrastructure.

3. **AWS Lambda**: Executes serverless backend logic, including sensor data handling, database interactions, and API responses.

4. **DynamoDB**: A NoSQL database used to store parking space data, including real-time sensor status and reservation information.

5. **API Gateway**: Exposes API endpoints for the web application to interact with the backend.

6. **Web Application (Frontend)**: Displays real-time parking information and user interaction features.

## Technologies Used
- **Hardware**: Ultrasonic Sensors, ESP8266 Wi-Fi Module
- **Cloud Services**: AWS IoT Core, AWS Lambda, AWS DynamoDB, AWS API Gateway
- **Programming Languages**: Arduino IDE for ESP8266 programming, JavaScript/HTML/CSS for the web application

## Getting Started

### Prerequisites
- An AWS account with access to IoT Core, Lambda, DynamoDB, and API Gateway.
- Hardware components (ESP8266, ultrasonic sensors).
- Basic understanding of Arduino programming.

### Setup Instructions
1. **IoT Device Setup**:
   - Connect the ultrasonic sensors to the ESP8266 module.
   - Program the ESP8266 using the Arduino IDE to send sensor data to AWS IoT Core via MQTT.

2. **AWS Setup**:
   - Set up AWS IoT Core to manage IoT devices and enable MQTT communication.
   - Create an AWS Lambda function to process incoming sensor data and interact with DynamoDB.
   - Set up a DynamoDB table to store parking data.
   - Create an API Gateway to expose endpoints for the web application.

3. **Web Application**:
   - Clone this repository to your local machine.
   - Open the project in your preferred text editor or IDE.
   - Update the API endpoints in the frontend code to point to your deployed API Gateway.
   - Run a local server to view the application.

4. **Testing**:
   - Deploy the IoT devices and test the parking space detection.
   - Access the web application to view real-time parking data.

## Usage
- The web application will automatically fetch and display parking space availability.
- Users can check for available spots in real-time.

## Contributing
Contributions are welcome! If you have suggestions for improvements or want to add features, feel free to fork the repository and submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- AWS Documentation for various services used.
- Community forums and tutorials for assistance with IoT and AWS setup.

## Contact
For any questions or feedback, please reach out to Sathish at [your-email@example.com].
