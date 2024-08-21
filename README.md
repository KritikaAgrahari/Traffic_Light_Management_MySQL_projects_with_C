# Traffic_Light_Management_MySQL_projects_with_C
A Smart City Traffic Management system is an excellent choice for a capstone project. It involves using technology to monitor, manage, and optimize traffic flow in a city to improve efficiency, reduce congestion, and enhance overall transportation experiences. Here’s a comprehensive guide on how you can approach this project:

## Project Overview
### Objective: 
Develop a database system to manage and analyze traffic data collected from various sensors across a city. The goal is to optimize traffic flow, monitor congestion, and provide actionable insights.

# Key Components

#### 1. Database Design
#### 2. Data Collection
#### 3. Query Development
#### 4. Performance Optimization
#### 5. Visualization and Reporting
#### 6. Real-Time Data Integration




## Database Schema
The system uses a MySQL database with the following tables:

#### Traffic_Sensors
- **SensorID** (Primary Key, INT)
- **Location** (VARCHAR)
- **Type** (VARCHAR, e.g., camera, loop sensor)
- **InstallationDate** (DATE)

#### Traffic_Data
- **DataID** (Primary Key, INT)
- **SensorID** (Foreign Key, INT)
- **Timestamp** (DATETIME)
- **VehicleCount** (INT)
- **AverageSpeed** (FLOAT)
- **OccupancyRate** (FLOAT)

#### Traffic_Lights
- **TrafficLightID** (Primary Key, INT)
- **Location** (VARCHAR)
- **Status** (VARCHAR, e.g., Red, Green, Yellow)
- **LastChangeTime** (DATETIME)

#### Traffic_Incidents
- **IncidentID** (Primary Key, INT)
- **Timestamp** (DATETIME)
- **Location** (VARCHAR)
- **Description** (TEXT)
- **Severity** (VARCHAR, e.g., Minor, Major)

#### Traffic_Reports
- **ReportID** (Primary Key, INT)
- **Timestamp** (DATETIME)
- **ReportType** (VARCHAR, e.g., Daily Summary, Peak Hour Analysis)
- **Details** (TEXT)

## 2. Data Collection

### Sensor Integration
Set up various sensors throughout the city to collect real-time data on traffic conditions.

### Data Logging
Ensure that data from sensors is logged consistently and accurately into the database.

### Data Sources
Consider integrating data from external sources like weather reports or public transportation schedules for a comprehensive analysis.

## Getting Started

### Prerequisites
- **C Compiler**: Ensure you have a C compiler (like GCC) installed.
- **MySQL Server**: Install and configure MySQL server.
- **MySQL Connector/C**: Required to connect C programs with MySQL databases.

## Setup and Installation

### MySQL Server Setup
1. **Install MySQL Server**:
   ```sh
   sudo apt-get install mysql-server
2. **Secure MySQL Installation**:
   ```sh
   sudo mysql_secure_installation
3. **Create DATABASE**:
   ```sh
   CREATE DATABASE Event_management;

## MySQL Connector/C Setup
4. **Install MySQL Connector/C**:
   ```sh
   sudo apt-get install libmysqlclient-dev

### Project Setup
5. **Clone the Repository**:
   ```sh
   git clone <https://github.com/TheShyamTripathi/Event_Management_systems_projectUsing_SQL_AND_C/>
6. **Navigate to Project Directory**:
   ```sh
   cd event-management-system
7. **Compile the program**:
   ```sh
   gcc -o event-management main.c -lymsqlclient
8. **Run the Program**:
   ```sh
   ./event_management

## Sample Commands

Below are some example commands used in the system:

### Add User:
```perl
add_user("John Doe", "john@example.com", "Organizer");
```
### Create Event:
```bash
   create_event("Tech Conference", "2024-09-15", "10:00 AM", "Auditorium");
```
### Register for Event:
```bash
   register_for_event(2, 5); // UserID = 2, EventID = 5
```
### Mark Attendence:
```bash
   mark_attendance(2, 5); // UserID = 2, EventID = 5
```

## Usage
### Add Users:
- Organizers and participants can be added to the system.

### Create Events:
- Organizers can create events by providing details like title, date, time, and location.

### Register for Events:
- Participants can browse available events and register for them.

### Track Attendance:
- The system allows attendance marking for participants who attend events.


## Contribution
We welcome contributions to enhance the functionality of this project. Feel free to fork the repository, make changes, and submit a pull request.

## Authors
- [Shyam Tripathi](https://github.com/TheShyamTripathi)
- [Harrsh Singh Tiwari](https://github.com/Harsh14055/)
- [Richa Kumari Jaishwal](https://github.com/Richajaishwal0)
- [Binay Kushwaha](https://github.com/GOLD3PHOENIXsurili)

## Future Enhancements

Some potential future improvements for the system:

- Implement a graphical user interface (GUI).
- Add notifications for event reminders.
- Implement feedback and reporting features.


## Acknowledgements
We would like to thank our professors and mentors for their guidance and support throughout this project.


## Collaboration
We welcome collaboration from anyone interested in contributing to this project. If you have any ideas, suggestions, or would like to contribute code, please feel free to fork the repository and submit a pull request.

---

Thank you for your interest in our project!

[Project Repository](https://github.com/KritikaAgrahari/Traffic_Light_Management_MySQL_projects_with_C/)


