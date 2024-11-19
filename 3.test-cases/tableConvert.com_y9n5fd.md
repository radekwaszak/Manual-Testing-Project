|  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| v2.id | title | description | preconditions | postconditions | tags | priority | severity | type | behavior | automation | status | is_flaky | layer | steps_type | steps_actions | steps_result | steps_data | milestone_id | milestone | suite_id | suite_parent_id | suite | suite_without_cases | parameters | is_muted |
|  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | 4 |  | Registration / Sing-in functional tests | 1 |  |  |
| 11 | Verify successful registration with valid data | Validate that a user can successfully register with valid details | User is on the registration page; registration form is visible. | A new account is created and the user is redirected to the dashboard, signed-in. |  | high | critical | functional | undefined | is-not-automated | actual | no | unknown | classic | 1. ""Select the appropriate social title radiobutton - Mr. or Mrs." |  |  |  |  |  |  |  |  |  |  |
| 2. ""Enter a valid first name | last name | and email."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 3. ""Enter a strong | valid password."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 4. ""Complete the optional field - birthdate."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 5. ""Accept terms and conditions."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 6. ""Accept customer data privacy."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 7. ""Click the \""Save\"" button."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " | 1. ""The appropriate radiobutton is selected." |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 2. ""Text fields populate with the entered information."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 3. ""Password is accepted and hidden behind asterisks or similar masking."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 4. ""Text fields populate with the entered information."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 5. ""Checkbox is selected."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 6. ""Checkbox is selected."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 7. ""User is successfully registered and redirected to the dashboard | signed-in."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " | 1. """ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 2. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 3. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 4. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 5. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 6. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 7. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " |  |  | 4 |  | Registration / Sing-in functional tests |  |  | no |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 12 | Verify registration fails with invalid email format | Validate that the system rejects registration attempts with an invalid email format. | User is on the registration page. | No account is created; the user remains on the registration page with an error message. |  | high | critical | functional | undefined | is-not-automated | actual | no | unknown | classic | 1. ""Select the appropriate social title radiobutton - Mr. or Mrs." |  |  |  |  |  |  |  |  |  |  |
| 2. ""Enter a valid first name and last name."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 3. ""Enter an invalid email format (e.g. | \""user@domain\"")."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 4. ""Enter a strong | valid password."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 5. ""Accept terms and conditions."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 6. ""Accept customer data privacy."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 7. ""Click the \""Save\"" button."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " | 1. ""The appropriate radiobutton is selected." |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 2. ""Text fields populate with the entered information."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 3. ""Email field accepts input | but format does not meet validation criteria."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 4. ""Password is accepted and hidden behind asterisks or similar masking."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 5. ""Checkbox is selected."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 6. ""Checkbox is selected."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 7. ""Registration fails; an error message indicating \""Invalid email format\"" is displayed."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " | 1. """ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 2. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 3. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 4. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 5. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 6. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 7. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " |  |  | 4 |  | Registration / Sing-in functional tests |  |  | no |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 13 | Verify registration fails with unchecked mandatory checkbox | Validate that the system rejects registration attempts with the “Customer Data Privacy” checkbox not checked. | User is on the registration page. | No account is created; the user remains on the registration page with an information message “Check this box if you want to continue” displayed. |  | high | critical | functional | undefined | is-not-automated | actual | no | unknown | classic | 1. ""Select the appropriate social title radiobutton - Mr. or Mrs." |  |  |  |  |  |  |  |  |  |  |
| 2. ""Enter a valid first name | last name | and email."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 3. ""Enter a strong | valid password."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 4. ""Accept terms and conditions."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 5. ""Click the \""Save\"" button."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " | 1. ""The appropriate radiobutton is selected." |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 2. ""Text fields populate with the entered information."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 3. ""Password is accepted and hidden behind asterisks or similar masking."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 4. ""Checkbox is selected."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 5. ""Registration fails; an information message indicating \u201cCheck this box if you want to continue\u201d is displayed."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " | 1. """ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 2. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 3. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 4. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 5. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " |  |  | 4 |  | Registration / Sing-in functional tests |  |  | no |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 14 | Successful login with valid credentials | Verify that a user can successfully sign in with valid credentials. | User has a registered account; login page is accessible. | User is signed-in and directed to the dashboard. |  | high | critical | functional | undefined | is-not-automated | actual | no | unknown | classic | 1. ""Enter valid email and password." |  |  |  |  |  |  |  |  |  |  |
| 2. ""Click the \""Sign In\"" button."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " | 1. ""Credentials are entered correctly and match stored user data." |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 2. ""Login is successful; user is redirected to the dashboard."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " | 1. """ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 2. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " |  |  | 4 |  | Registration / Sing-in functional tests |  |  | no |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 15 | Verify login fails with incorrect password | Ensure login fails when an incorrect password is entered. | User has a registered account; login page is accessible. | User remains on the login page with an error message indicating incorrect credentials. |  | high | critical | functional | undefined | is-not-automated | actual | no | unknown | classic | 1. ""Enter a valid email but an incorrect password." |  |  |  |  |  |  |  |  |  |  |
| 2. ""Click the \""Sign In\"" button."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " | 1. ""Incorrect password is accepted into the password field." |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 2. ""Login fails; an error message stating \""Authentication failed\"" appears."" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " | 1. """ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 2. """" |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| " |  |  | 4 |  | Registration / Sing-in functional tests |  |  | no |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
