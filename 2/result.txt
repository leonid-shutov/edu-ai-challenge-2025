**Title**  
Logout Button Unresponsive on Safari Browser

**Description**  
The logout button does not respond when clicked in the Safari browser. The user is unable to log out of the application, and there is no visual or functional feedback indicating that the action was registered.

**Steps to Reproduce**  
1. Launch the application using Safari.  
2. Log in with a valid user account.  
3. Locate and click the logout button (typically in the navigation bar or user dropdown).  
4. Observe that no action is taken.

**Expected vs Actual Behavior**  
- *Expected*: Clicking the logout button should terminate the session and redirect the user to the login screen or show a logout confirmation.  
- *Actual*: Clicking the logout button does nothing. There is no response, redirection, or message shown.

**Environment**  
- Browser: Safari  
- OS: Likely macOS or iOS (based on browser)  
- Device: Not specified  
- Application Version: Unknown

**Severity or Impact**  
High – A fundamental action (logout) fails on Safari, affecting user experience and session security.

**Verification**  
After implementing a fix, test in the latest versions of Safari on both macOS and iOS. Confirm that clicking the logout button reliably ends the session and redirects the user. Include automated tests if applicable.
