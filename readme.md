# README.md for Telegram Multi-Account Invite Tool

This README provides a comprehensive guide for running the **Telegram Multi-Account Invite Tool** on your PC and mobile devices using a VPS.

## Prerequisites

- **Python 3.x** installed on your local machine or VPS.
- **Telegram API credentials** (API ID and API Hash).
- A valid **Telegram account** for authentication.

## Installation Steps

### For PC (Windows/Linux)

1. **Install Python:**
   - Download from [python.org](https://www.python.org/downloads/).
   - Verify installation by running:
     ```
     python --version
     ```

2. **Install Required Packages:**
   - Open your terminal and install the necessary packages:
     ```
     pip install telethon colorama aiolimiter
     ```

3. **Download the Script:**
   - Clone or download the script from your repository.

4. **Prepare Configuration:**
   - Create a file named `acck.json` with your Telegram account details in JSON format:
     ```
     {
       "+1234567890": {
         "api_id": "YOUR_API_ID",
         "api_hash": "YOUR_API_HASH",
         "session_name": "session_file_name",
         "user_id": "USER_ID",
         "first_name": "FirstName"
       }
     }
     ```

5. **Run the Script:**
   - Execute the script using Python:
     ```
     python your_script_name.py
     ```

### For Mobile Devices Using VPS

1. **Set Up a VPS:**
   - Choose a VPS provider and create an instance with a Linux distribution.

2. **Connect to Your VPS:**
   - Use SSH to connect to your server:
     ```
     ssh username@your_vps_ip
     ```

3. **Install Python on VPS:**
   - Update your package list and install Python:
     ```
     sudo apt update
     sudo apt install python3 python3-pip
     ```

4. **Install Required Packages:**
   - Install necessary libraries:
     ```
     pip3 install telethon colorama aiolimiter
     ```

5. **Upload Your Script:**
   - Use SCP or any file transfer method to upload your script and `acck.json` file to the VPS.

6. **Run the Script on VPS:**
   - Navigate to the directory where your script is located and run it:
     ```
     python3 your_script_name.py
     ```

## Usage Instructions

1. **Add Telegram Accounts:** Select option 1 from the main menu to add accounts.
2. **Invite Group Members:** Select option 2 to invite members from one group to another.
3. **View Saved Accounts:** Select option 3 to view all saved accounts.
4. **Remove Account:** Use option 4 to remove an account from the saved list.
5. **Exit:** Choose option 5 to exit the application.

## Important Notes

- Handle your API credentials securely.
- Be cautious about Telegram's usage policies to avoid account bans.
- The tool is designed for educational purposes; misuse may lead to penalties from Telegram.

## Troubleshooting

If you encounter issues:

- Check if all dependencies are installed correctly.
- Review logs for detailed error messages.
- Ensure that you have a stable internet connection.