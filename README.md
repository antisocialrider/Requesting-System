# TS Request Service Features

This document outlines the key features of the TS Requestservice, explaining how to use them from both the perspective of a regular player requesting a service and an authorized operator.

## For All Players

### 1. Main Menu Access
* **How to Use**: Type `/requestui` in your in-game chat to open the main menu.

### 2. Request a Service
* **Description**: Players can request various roadside assistance services.
* **How to Use**:
    1.  Open the main menu (`/requestui`).
    2.  Click "Request a Service".
    3.  **Select Location**: Choose from "Current GPS Location" (uses your current position) or a preset location like "Legion Square", "Sandy Shores Airfield", or "Paleto Bay Bank".
    4.  **Choose Assistance Type**: Select the type of help you need (e.g., Towing, Recovery, Fuel, Mechanic).
    5.  **Add Photos**: You *must* add at least one photo. You can either:
        * **Upload via Link**: Enter a direct image URL (e.g., from Discord, Imgur).
        * **Take Picture**: Use the in-game camera to snap a photo, which will automatically be added.
    6.  **Provide Vehicle Description & Notes**: Enter details about your vehicle (make, model, color, license plate) and any additional notes for the operator.
    7.  **Proceed to Confirmation**: Click the "Proceed to Confirmation" button.
    8.  **Confirmation Screen**: Review your request and set a payment offer. The system will display a default starting pay for your selected service. Your offer must be equal to or higher than this default.
    9.  **Confirm & Request**: Click this button to submit your request to available operators.

### 3. My Active Requests
* **Description**: View the status of your active roadside assistance requests.
* **How to Use**:
    1.  Open the main menu (`/requestui`).
    2.  Click "My Active Requests".
    3.  You will see a list of your requests, their current status (e.g., Pending, In Progress, En Route, On Scene, Completed, Cancelled), and the assigned operator (if any).
    4.  **Cancel Request**: If a request is still "Pending" or "In Progress", you can cancel it from here.
    5.  **Payment Prompt**: If an operator sends a payment request, a modal will appear where you can "Accept & Pay" or "Deny Payment".

### 4. Service Information
* **Description**: Provides details about the types of services offered and their estimated costs.
* **How to Use**:
    1.  Open the main menu (`/requestui`).
    2.  Click "Service Information".
    3.  Browse through the available service cards.

### 5. Settings
* **Description**: Customize UI preferences such as notification volume and whether to receive notifications.
* **How to Use**:
    1.  Open the main menu (`/requestui`).
    2.  Click "Settings".
    3.  Adjust the UI Volume slider (0-100%).
    4.  Toggle Notifications On/Off.
    5.  Your settings are saved automatically.

### 6. Submitting Feedback
* **Description**: Provide feedback on completed services, including a rating and message.
* **How to Use**: After a job is completed, a feedback button may appear on your request card (or related UI element). Click it to submit your feedback.

### 7. Closing the UI
* **How to Use**: Press the `ESC` key or click the back button on the main menu.

## For Operators (Configured Job/Grade Required)

### 1. Logging In/Out of Duty
* **Description**: Operators can toggle their on-duty status, making them visible for accepting jobs.
* **How to Use**:
    1.  Open the main menu (`/requestui`).
    2.  Click the "Log In as Operator" button.
    3.  Your status will change to "On Duty". Click the button again to go "Off Duty".
    4.  You can also set a custom status (e.g., "Available", "On Break") via the "My Contact Details" section in Operator Mode.

### 2. Operator Mode
* **Description**: Access the operator-specific dashboard to manage jobs.
* **How to Use**:
    1.  Log in as an operator.
    2.  From the main menu, click "Operator Mode".

### 3. My Contact Details
* **Description**: View and update your public operator details.
* **How to Use**:
    1.  In "Operator Mode", your contact details card is visible.
    2.  Update your "Name" and "Company" fields.
    3.  Select your "Status" (Available, On Break).
    4.  Click "Update Details" to save changes.

### 4. Available Jobs
* **Description**: View a list of pending service requests from players.
* **How to Use**:
    1.  In "Operator Mode", the "Available Jobs" section displays current requests.
    2.  Click on a job card to expand its details, including requester, location, description, payment offer, and photos.
    3.  Click "Accept Job" to claim the request.
    4.  The list will automatically update as new jobs come in or are accepted by others.

### 5. Current Job
* **Description**: Manage the job you have accepted.
* **How to Use**:
    1.  After accepting a job, this card will appear.
    2.  **Update Status**: Buttons will appear based on the current job status:
        * "Mark En Route": When you start heading to the location.
        * "Mark On Scene": When you arrive at the location.
    3.  **Payment Request**: Once "On Scene", an input field will appear, pre-filled with the original offer. Enter the final amount and click "Send Payment Request" to prompt the customer for payment.
    4.  **Detach from Job**: If necessary, you can detach from the job. A confirmation prompt will appear.
    5.  **Blip Management**: A blip will be created on your map leading to the job location.

### 6. Message Customer
* **Description**: Send direct messages to the customer of your current active job.
* **How to Use**:
    1.  While on an active job, the "Message Customer" card will be available.
    2.  Type your message in the text area.
    3.  Click "Send Message".

## For Admins (Configured Identifier Required)

### 1. Dev/Admin Tools Access
* **How to Use**:
    1.  Open the main menu (`/requestui`).
    2.  Go to "Settings".
    3.  If your identifier is listed in the config, you will see a button to access "Dev/Admin Tools". Click it.

### 2. Active Requests Management
* **Description**: View and manage all active (pending, in progress, completed) requests.
* **How to Use**:
    1.  In "Dev/Admin Tools", the "Active Requests" card shows a list of all jobs.
    2.  Use the search bar to filter requests by Job ID, Requester ID, or Operator ID.
    3.  Expand any request card to see full details.
    4.  **Admin Cancel Request**: Click to forcefully cancel any active request.
    5.  **Admin Assign Job**: Assign a pending job to a specific on-duty operator.

### 3. On-Duty Operators Monitoring
* **Description**: View a list of all operators currently logged into duty.
* **How to Use**:
    1.  In "Dev/Admin Tools", the "On-Duty Operators" card lists all active operators.
    2.  Use the search bar to filter operators by Name or ID.
    3.  Sort the list by Name, Status, or Player ID in ascending or descending order.
    4.  **Admin Kick Operator**: Force an operator off duty.
