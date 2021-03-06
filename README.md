# codepathweek4assignment
# Project 4 - Forgery, Theft, and Hijacking Prevention

Time spent: **3** hours spent in total

## User Stories

The following **required** functionality is completed:

1\. [√]  Required: Test for initial vulnerabilities

2\. [√]  Required: Configure sessions
  * [√]  Required: Only allow session IDs to come from cookies
  * [√]  Required: Expire after one day
  * [√]  Required: Use cookies which are marked as HttpOnly

3\. [√]  Required: Complete Login page.
  * [√]  Required: Show an error message when username is not found.
  * [√]  Required: Show an error message when username is found but password does not match.
  * [√]  Required: After login, store user ID in session data.
  * [√]  Required: After login, store user last login time in session data.
  * [√]  Required: Regenerate the session ID at the appropriate point.

4\. [√]  Required: Require login to access staff area pages.
  * [√]  Required: Add a login requirement to *almost all* staff area pages.
  * [√]  Required: Write code for `last_login_is_recent()`.

5\. [√]  Required: Complete Logout page.
  * [√]  Required: Add code to destroy the user's session file after logging out.

6\. [√]  Required: Add CSRF protections to the state forms.
  * [√]  Required: Create a CSRF token.
  * [√]  Required: Add CSRF tokens to forms.
  * [√]  Required: Compare tokens against the stored version of the token.
  * [√]  Required: Only process forms data sent by POST requests.
  * [√]  Required: Confirm request referer is from the same domain as the host.
  * [√]  Required: Store the CSRF token in the user's session.
  * [√]  Required: Add the same CSRF token to the login form as a hidden input.
  * [√]  Required: When submitted, confirm that session and form tokens match.
  * [√]  Required: If tokens do not match, show an error message.
  * [√]  Required: Make sure that a logged-in user can use pages as expected.

7\. [√]  Required: Ensure the application is not vulnerable to XSS attacks.

8\. [√]  Required: Ensure the application is not vulnerable to SQL Injection attacks.

9\. [√]  Required: Run all tests from Objective 1 again and confirm that your application is no longer vulnerable to any test.


The following advanced user stories are optional:

* [ ]  Bonus Objective 1: Identify security flaw in Objective #4 (requiring login on staff pages)
  * [ ]  Identify the security principal not being followed.
  * [ ]  Write a short description of how the code could be modified to be more secure.

* [ ] Bonus Objective 2: Add CSRF protections to all forms in the staff directory

* [ ]  Bonus Objective 3: CSRF tokens only valid for 10 minutes.

* [ ]  Bonus Objective 4: Sessions are valid only if user-agent string matches previous value.

* [ ]  Advanced Objective: Set/Get Signed-Encrypted Cookie
  * [ ]  Create "public/set\_secret\_cookie.php".
  * [ ]  Create "public/get\_secret\_cookie.php".
  * [ ]  Encrypt and sign cookie before storing.
  * [ ]  Verify cookie is signed correctly or show error message.
  * [ ]  Decrypt cookie.

## Video Walkthrough

Here's a walkthrough of implemented user stories:

<img src='http://i.imgur.com/wVfZldu.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

GIF created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while building the app.

## License

    Copyright [yyyy] [Indrajit Gurung]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.