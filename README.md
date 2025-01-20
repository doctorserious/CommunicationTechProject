# CommunicationTechProject

# Direction Classification of Accelerometer Data Using the K-means Algorithm

## Description
In this project, a system is developed that uses the nRF5340-DK development board, an accelerometer, a Raspberry Pi, a Linux server, and the K-means algorithm. The nRF5340-DK device sends data from its attached accelerometer to the Raspberry Pi via Bluetooth. The Raspberry Pi transfers the received data to a MySQL database located on a Linux server. The data received by the database is stored in a .csv file, which is used to develop a Python application utilizing the K-means algorithm for creating a neural network.

## Technologies and Skills Used in the Project

### Hardware and Platforms
- **nRF5340-DK**: Measures data from the accelerometer (GY-61 ADXL335), such as acceleration and orientation, and wirelessly transmits it to the Raspberry Pi using a 433 MHz Bluetooth connection.
- **Raspberry Pi 3 Model B v1.2**: Forwards the received data from the nRF5340-DK to the MySQL server located on the school network using the HTTP protocol.
- **Laptop**: For writing code, monitoring the database, remote connection to the Raspberry Pi, and Linux server.

### Operating Systems and Tools
- **Windows**: Windows 11 and 10.
- **Linux**: Debian-based 32-bit Raspberry Pi OS (latest version).
- **GitHub and GitBash**: For managing the project's files and versions.

### Programming Languages and Development Environments
- **Visual Studio Code**: The development environment used for writing C and Python code.
- **Google Colab**: Used for writing code for the neural network classifier.
- **Python**: For the Raspberry Pi program, which receives sensor data and transfers it to the database, as well as machine learning programs.
- **SQL**: For MySQL database management to store accelerometer data.
- **C**: The programming language used for the nRF5340-DK, which collects accelerometer data and sends it to the Raspberry Pi via Bluetooth.
- **Linux**: For operating the Raspberry Pi and the Linux server.

### Database Software
- **MySQL**: A self-created database on one of the Linux server addresses.

### Data Analysis and Machine Learning
- **K-means Algorithm**: We use the K-means algorithm to cluster the accelerometer's x, y, and z-axis data into six cluster centers by calculating the distances to the nearest cluster's random value. The new center of the cluster is calculated as the average of the data points it has received. The process of dividing data points into clusters and calculating averages continues until no significant changes are observed in the centers.
  
- **Neural Network Classifier**: Classifies the measurement data into the correct category using two Dense layers, adding the neural network coefficients. The result is a probability value for each direction. An alternative method for classifying measurement data alongside the K-means algorithm.

- **Confusion Matrix**: The confusion matrix indicates the efficiency of the classification algorithm.
- **Wireshark**: An application used to examine the data packets of the traffic between devices.

### Version Control and Collaboration
- **Git and GitHub**: For managing the project files and version control.
- **Kanban Board**: For tracking completed and ongoing tasks.
- **Discord**: For daily information sharing and file exchange.

- ## Project Participants: Juho Kupila and Jaakko Lukkari
