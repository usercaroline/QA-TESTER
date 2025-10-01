
# Test Case - Student Registration

## Test ID
TC001

## Objective
Verify that the student registration form on Demo QA works correctly.

## Pre-conditions
- Access to the site: https://demoqa.com/automation-practice-form
- Compatible browser (Chrome, Firefox, etc.)
- No user previously registered with the same data

## Steps
1. Open the site: https://demoqa.com/automation-practice-form
2. Fill in "First Name" with a valid name
3. Fill in "Last Name" with a valid surname
4. Fill in "Email" with a valid email address
5. Select the gender: Male, Female, or Other
6. Fill in "Mobile" with a valid 10-digit number
7. Select date of birth using the date picker
8. Select hobbies (e.g., Sports, Reading, Music)
9. Fill in "Current Address" with a valid address
10. Select State and City
11. Click "Submit"

## Expected Result
The form is submitted successfully and a confirmation message appears with all entered data.

## Actual Result
Form submitted successfully. All entered data appears correctly in the confirmation message.

## Status
✅ Passed

![Form submission success](images/FormSubmissionSuccess.png)

______________________________________________________________________________________________

# Test Case - Student Registration (Negative Scenarios)

## Test ID
TC001-N1

## Objective
Verify that the form prevents submission with invalid data or missing required fields.

## Pre-conditions
- Access to the site: https://demoqa.com/automation-practice-form
- Compatible browser
- No user previously registered with the same data

## Steps - Invalid Phone
1. Open the form
2. Fill in "First Name" and "Last Name" correctly
3. Fill in "Email" correctly
4. Select a gender
5. Fill in "Mobile" with LESS than 10 digits
6. Click "Submit"

## Expected Result
- The form should **not submit**
- An error message should indicate invalid mobile number

## Actual Result
Form did not submit. Error message displayed: "enter a 10-digit mobile number"

## Status
✅ Passed

![Form submission success](images/negativescenario.png) 

_____________________________________________________________________________________________

# Test Case - Student Registration (Missing Last Name)

## Test ID
TC001-N2

## Objective
Verify that the form prevents submission when the "Last Name" field is left empty.

## Pre-conditions
- Access to: https://demoqa.com/automation-practice-form
- Compatible browser
- Other required fields are filled correctly

## Steps
1. Open the student registration form.
2. Fill in "First Name" with a valid name.
3. Leave "Last Name" empty.
4. Fill in all other required fields correctly.
5. Click "Submit".

## Expected Result
- Form should not submit.
- The system should indicate that "Last Name" is required (e.g., field highlight or error message).

## Actual Result
- Form did not submit.
- The "Last Name" field is highlighted in red with an exclamation mark.
- No additional error message appeared.

## Status
✅ Passed

![Form submission success](images/missinglastname.png) 

_______________________________________________________________________________________________-g