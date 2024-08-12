# OrangeHRM Automation Project

This project automates various tasks on the OrangeHRM site, including logging in, creating new employees, saving credentials, and verifying data.

## Project Overview

The automation script performs the following steps:

1. **Login to OrangeHRM**: The script logs into the OrangeHRM site with a specified set of credentials.
2. **Add New Employee**: A new employee is created with a randomly generated username and password.
3. **Save Credentials**: The generated username and password are stored in an Excel file (`add_employee_data.xlsx`) for future use.
4. **Login with Saved Credentials**: The script retrieves the saved credentials from the Excel file and logs into the application with them.
5. **Verify Data**: Data from the Excel file is verified against the data in the OrangeHRM application.

## Technologies Used

- **Katalon Studio**: For automation scripting.
- **Groovy**: The scripting language used within Katalon Studio.
- **Apache POI**: For reading from and writing to Excel files.
- **OrangeHRM**: The application under test.

## Project Structure

- **Test Cases**
  - `login_using_new_creds`: Logs into the OrangeHRM site using credentials retrieved from the Excel file.
  - `add_employee`: Creates a new employee with a randomly generated username and password.
  - `test_case_to_verify_data`: Verifies that the employee data stored in the Excel file matches the data on the OrangeHRM site.
  
- **Global Variables**
  - `User_name`, `Password`: Stores the randomly generated username and password.
  - `First_name`, `Middle_name`, `Last_name`, `employee_id`: Stores the employee details.
  
- **Excel File**: `add_employee_data.xlsx`
  - Stores employee details such as `First_name`, `Middle_name`, `Last_name`, `Username`, `Password`, and `Employee_id`.

## How to Run

1. Clone the repository.
2. Open the project in Katalon Studio.
3. Run the test cases in the following sequence:
   - `add_employee`
   - `login_using_new_creds`
   - `test_case_to_verify_data`
4. Review the test results to ensure the data has been correctly added and verified.

## Contributing

Feel free to submit issues or pull requests if you find any bugs or have suggestions for improvements.

