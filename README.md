# Urban Scooter Web and Mobile App
**Skills:**
- Exploratory Testing
- UI Testing
- Cross-platform Testing
- Requirement Analysis
- Postman
- API Testing
- JSON
- Jira
- Command Line
- SQL
- Android Studio

## Overview
Urban Scooter is a two-part system consisting of a Web App for users and a Mobile App for couriers. The Web App allows users to rent electric scooters and schedule deliveries. Users can select a scooter, specify a delivery location, and track its status. The Mobile App will enable couriers to pick up scooters from warehouses and deliver them to users. Couriers receive assigned deliveries, navigate to destinations, and confirm drop-offs.
<p float="left">
  <kbd>
<img src="/Screenshots/Urban_Scooter_Order_Tracking.png" alt=" Using the web app, users can track their orders" width=60% heigh=60% hspace="45">
<img src="/Screenshots/Urban_Scooter_Login_Couriers.png" alt=" Using the mobile app, couriers can log in to their profile" width=16% heigh=16% hspace="45">
  </kbd>
</p>

### Special Features
- **Real-time Order Placement:** Users can rent scooters and schedule deliveries through the web app.
- **Courier Assignment & Navigation:** Couriers receive optimized delivery routes in the mobile app.
- **Live Tracking:** Users can track scooter deliveries while couriers update statuses in real time.
- **Multi-platform Functionality:** Ensures seamless coordination between users and couriers.

## Tasks
During this project, I conducted comprehensive Quality Assurance (QA) testing on both the **web and mobile** app, covering **API** functionality, **UI/UX** consistency, and **data validation**.

### Key Achievements:
1. **Web App Testing ([Checklist](https://docs.google.com/spreadsheets/d/1yudAWQtN34VO6AKA37JNbUF9M-ZxJEf2FdmvodB436g/edit?usp=sharing))**
- Verified UI elements:
    - Scooter selection and delivery request process.
    - Navigation between screens and form validation.
    - Order tracking and real-time updates.
- Ensured correct pricing and order summary calculations.
2. **Data Validation Testing ([Checklist](https://docs.google.com/spreadsheets/d/1GuoLiCJjC_fBmzDPR57Lqf_k7Q8QeJiI97fKq1HP6jA/edit?usp=sharing))**
- Conducted boundary testing on form inputs (e.g., user details, delivery addresses).
- Ensured consistent data handling across browsers (Opera, Chrome).
- Verified correct error messages for invalid inputs (e.g., incorrect phone numbers, incomplete addresses)
3. **Mobile App Testing ([Test Cases](https://docs.google.com/spreadsheets/d/1EAT2vv8y0oh1cfxJHeJ-Qe0bj3CCuP_t1hKu8xBS0F4/edit?usp=sharing))**
- Tested the courier app’s ability to:
    - Receive assigned deliveries and update order status.
    - Scan scooter QR codes for pickup confirmation.
    - Navigate using in-app maps and complete deliveries.
- Identified issues with real-time status updates and incorrect navigation routes.
4. **API Testing ([Checklist](https://docs.google.com/spreadsheets/d/187omhoqsRgBQNaXkgskuijRdi6moDk0LZjOSv74UYJc/edit?usp=sharing))**
- Verified API responses for key actions:
  - Creating new deliveries (scooter orders).
  - Assigning orders to couriers.
  - Updating scooter delivery status.
- Ensured correct error handling and response codes.
- Used **Postman** to send test requests and analyze response times.
## Findings
### Overall Condition
The Urban Scooter platform functions well but has critical issues affecting order tracking, status updates, and navigation accuracy. These issues impact both user experience and courier operations.
### Summary
1. **Web App Issues ([Jira Bug Report](https://docs.google.com/document/d/19YYxafo25IJ56CbvWiGFopBeEvr-tv39KC2wy1aHxAw/edit?usp=sharing)):**
  - The order tracking screen did not constantly update correctly.
  - The pricing breakdown sometimes excluded delivery fees.
  - Order history did not always reflect completed deliveries.
2. **Data Validation Issues ([Jira Bug Report](https://docs.google.com/document/d/1OjlxnFyFyAB_SzsPANRAWq1VA6x90oApClOkJnxq0gw/edit?usp=sharing)):**
  - Some invalid delivery addresses were accepted, causing failed orders.
  - User name fields allowed unsupported characters, leading to errors in tracking data.
3. **Mobile App Issues ([Jira Bug Report](https://docs.google.com/document/d/1pfaclx0jMojZxj6Qif5zad9LDu5zpIjthJroRwti5RU/edit?usp=sharing)):**
  - Navigation did not always show optimal routes, affecting delivery efficiency.
  - Status updates took too long to sync with the web app.
  - Push notifications for new delivery assignments that were delayed or missing.
4. **API Issues ([Jira Bug Report](https://docs.google.com/document/d/1WJmiew2Ea4p8K_163eN2ytoJvRGd5_9yJCWxVgsbPmE/edit?usp=sharing)):**
  - Some delivery orders failed to update correctly in the backend.
  - Status updates (e.g., "Out for Delivery") were not reflected in real-time.
  - QR code validation for scooter pick-up had inconsistencies.
### Key Areas for Improvement
In my test report, I highlighted several key areas for improvement:
- Fix API synchronization to ensure real-time updates across platforms.
- Improve delivery address validation to prevent failed scooter drop-offs.
- Enhance route optimization for couriers in the mobile app.
- Ensure push notifications are reliable for courier assignments.
- Refine pricing logic to display correct final costs.
