# AutoTeams

This Flask application allows users to upload CSV or Excel files containing email addresses, send announcements to those email addresses via Microsoft Teams, and retrieve responses from the recipients.

## UI
![Screenshot 2024-04-04 141921](https://github.com/JaiR3152/AutoTeams/assets/165999620/da9f2917-1192-479e-b566-4e3160676c14)


## Features

- **Upload File**: Users can upload CSV or Excel files containing email addresses.
- **Send Message**: Users can send announcements to the recipients listed in the uploaded files.
- **Get Responses**: Users can retrieve responses from the recipients and export them to an Excel file.
- **Delete File**: Users can delete uploaded files.

## Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/JaiR3152/AutoTeams.git
   ```

2. Navigate to the project directory:

   ```bash
   cd AutoTeams
   ```

3. Install the required Python packages using pip:

   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the project directory and add the following environment variables:

   ```plaintext
   CLIENT_ID=<your-client-id>
   R_URL=<your-redirect-url>
   C_S=<your-client-secret>
   ```

   Replace `<your-client-id>`, `<your-redirect-url>`, and `<your-client-secret>` with your Microsoft Teams application's client ID, redirect URL, and client secret respectively.

5. Run the Flask application:

   ```bash
   python main.py
   ```

6. Access the application in your web browser at `http://localhost:5000`.

## Usage

1. **Upload File**: Navigate to the homepage and upload a CSV or Excel file containing email addresses.

2. **Send Message**: Once the file is uploaded, you can enter a message in the provided text area and send announcements to the recipients listed in the uploaded file.

3. **Get Responses**: After sending announcements, you can retrieve responses from the recipients by clicking the "Get Responses" button next to the uploaded file. The responses will be exported to an Excel file named `response.xlsx`.

4. **Delete File**: You can delete uploaded files by clicking the "Delete" button next to the file on the homepage.

## Dependencies

- Flask: Web framework for building the application.
- Pandas: Library for data manipulation and analysis.
- Requests: Library for making HTTP requests.
- Graph API: Microsoft's tool for developers to access data and relationships across Microsoft cloud services. 

