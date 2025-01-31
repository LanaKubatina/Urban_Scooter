# Urban Scooter Web and Mobile Apps
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
Urban Scooter is a two-part system consisting of a Web App for users and a Mobile App for couriers.
- **Web App** allows users to rent electric scooters and schedule deliveries. Users can select a scooter, specify a delivery location, and track its status.
- **Mobile App** is used by couriers to pick up scooters from warehouses and deliver them to users. Couriers receive assigned deliveries, navigate to destinations, and confirm drop-offs.
### Special Features
- **Real-time Order Placement:** Users can rent scooters and schedule deliveries through the web app.
- **Courier Assignment & Navigation:** Couriers receive optimized delivery routes in the mobile app.
- **Live Tracking:** Users can track scooter deliveries while couriers update statuses in real time.
- **Multi-platform Functionality:** Ensures seamless coordination between users and couriers.

## Tasks
During this project, I conducted comprehensive Quality Assurance (QA) testing on both the Web App and Mobile App, covering API functionality, UI/UX consistency, and data validation.

### Key Achievements:
1. **API Testing**
- Verified API responses for key actions:
  - Creating new deliveries (scooter orders).
  - Assigning orders to couriers.
  - Updating scooter delivery status.
- Ensured correct error handling and response codes.
- Used **Postman** to send test requests and analyze response times.
2. **Data Validation Testing**
- Conducted boundary testing on form inputs (e.g., user details, delivery addresses).
- Ensured consistent data handling across browsers (Opera, Chrome).
- Verified correct error messages for invalid inputs (e.g., incorrect phone numbers, incomplete addresses)
3. **Mobile App Testing (Courier Operations)**
- Tested the courier app’s ability to:
    - Receive assigned deliveries and update order status.
    - Scan scooter QR codes for pickup confirmation.
    - Navigate using in-app maps and complete deliveries.
- Identified issues with real-time status updates and incorrect navigation routes.
4. **Web App Testing (User Interface & Ordering Flow)**
- Verified UI elements:
    - Scooter selection and delivery request process.
    - Navigation between screens and form validation.
    - Order tracking and real-time updates.
- Ensured correct pricing and order summary calculations.
## Findings
### Overall Condition
The Urban Scooter platform functions well but has critical issues affecting order tracking, status updates, and navigation accuracy. These issues impact both user experience and courier operations.
### Summary
1. **API Issues:**
  - Some delivery orders failed to update correctly in the backend.
  - Status updates (e.g., "Out for Delivery") were not reflected in real-time.
  - QR code validation for scooter pick-up had inconsistencies.
2. **Data Validation Issues:**
  - Some invalid delivery addresses were accepted, causing failed orders.
  - User name fields allowed unsupported characters, leading to errors in tracking data.
3. **Mobile App Issues (Courier App):**
  - Navigation did not always show optimal routes, affecting delivery efficiency.
  - Status updates took too long to sync with the web app.
  - Push notifications for new delivery assignments that were delayed or missing.
4. **Web App Issues (User Platform):**
  - The order tracking screen did not constantly update correctly.
  - The pricing breakdown sometimes excluded delivery fees.
  - Order history did not always reflect completed deliveries.
### Key Areas for Improvement
In my test report, I highlighted several key areas for improvement:

✔️ Fix API synchronization to ensure real-time updates across platforms.

✔️ Improve delivery address validation to prevent failed scooter drop-offs.

✔️ Enhance route optimization for couriers in the mobile app.

✔️ Ensure push notifications are reliable for courier assignments.

✔️ Refine pricing logic to display correct final costs.
