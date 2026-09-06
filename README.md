📌 Project Overview
The Metro Ticket Generating System is a ServiceNow-based project designed to digitize the metro ticket booking process.

The system allows passengers to select their source and destination stations, choose the journey type, specify the number of passengers, select a payment mode, calculate the ticket amount, and generate a QR-based digital ticket.

The main goal is to reduce waiting time, minimize manual effort, improve fare calculation accuracy, and provide a convenient digital ticketing experience.

🎯 Objectives
Digitize the metro ticket booking process using ServiceNow.
Reduce passenger waiting time and manual ticketing effort.
Provide easy source and destination station selection.
Automate fare calculation.
Support digital payment options such as UPI and Card.
Generate QR-based digital metro tickets.
Reduce paper usage through digital tickets.
Improve operational efficiency and customer convenience.
👥 Stakeholders
Passengers – Book metro tickets and receive QR-based tickets.
Station Managers – Maintain station information.
Metro Operations Team – Support metro operations.
IT Administrators – Maintain the ServiceNow system.
🛠️ Technologies Used
ServiceNow
Service Catalog
Custom Tables
Catalog Variables
Catalog Client Scripts
JavaScript
ServiceNow Portal Widget
QR Code API
ServiceNow ACLs
GitHub
🏗️ Main Components
1. Metro Station's Details Table
A custom ServiceNow table is used to store metro station information.

Table: u_metro_station_s_details

The table is used for:

Starting From
Going To
2. Book A Metro Ticket
The Service Catalog item provides the passenger ticket-booking form.

Catalog Item: Book A Metro Ticket

The form contains:

Starting From
Going To
Type Of Journey
No Of Passengers
Amount For Single Journey
Amount Including Return
Mode Of Payment
3. Journey Type
Passengers can select:

Single Journey
Return Journey
4. Number of Passengers
The system supports:

1 Passenger
2 Passengers
3 Passengers
4 Passengers
5. Payment Mode
Available payment options:

UPI
Card
Others
6. Fare Calculation
The system calculates the ticket amount based on journey type and number of passengers.

7. QR Code Generation
A QR code is generated for the digital metro ticket and displayed to the passenger.

8. Metro QR Widget
Widget Name: Metro QR Widget

Widget ID: metro_qr_widget

The widget displays the generated QR code and scanning instructions.

🔄 Ticket Booking Flow
Passenger
    ↓
Book A Metro Ticket
    ↓
Select Starting From
    ↓
Select Going To
    ↓
Select Journey Type
    ↓
Select Number of Passengers
    ↓
Calculate Fare
    ↓
Select Payment Mode
    ↓
Generate QR Code
    ↓
Display QR Ticket
    ↓
Scan at Metro Gate
