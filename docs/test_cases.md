# Selected Functionality: Login System

## Description
The login system is responsible for validating user credentials before allowing access to the system.

## Rules
- Username must be **admin**
- Password must be **1234**
- Both username and password fields must not be empty


## Test Cases

### Positive Test Cases

| Test Case ID | Test Description | Input | Expected Result |
|-------------|----------------|-------|----------------|
| TC01 | Login with valid username and password | admin, 1234 | Login Successful |
| TC02 | Login using correct credentials | admin, 1234 | Login Successful |
| TC03 | Repeated login with valid credentials | admin, 1234 | Login Successful |
| TC04 | Successful login when fields are filled correctly | admin, 1234 | Login Successful |

### Negative Test Cases

| Test Case ID | Test Description | Input | Expected Result |
|-------------|----------------|-------|----------------|
| TC05 | Login with wrong password | admin, 0000 | Invalid Credentials |
| TC06 | Login with empty username | "", 1234 | Username or password cannot be empty |
