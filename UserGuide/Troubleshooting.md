# Troubleshooting Guide

This guide provides solutions to common issues users might face while using Trello or its API. Follow these steps to quickly resolve problems and get back on track.

---

## Common Issues for Trello Users

### 1. Problem: Unable to Log In
**Cause**: Incorrect email or password, or account not activated.  
**Solution**:
1. Double-check your email and password.
2. If you forgot your password, click **"Forgot Password"** on the login page and follow the instructions.
3. Ensure you have activated your account via the activation email sent during sign-up.

---

### 2. Problem: Unable to Invite Team Members
**Cause**: Email address is incorrect or user already exists in the workspace.  
**Solution**:
1. Verify the email addresses you are inviting.
2. Ensure the user has not already been added to the board or workspace.
3. Check your internet connection and try again.

---

### 3. Problem: Unable to Create a Board or Card
**Cause**: Account has reached the limit for free boards or lists.  
**Solution**:
1. Upgrade to a Trello Premium plan for additional boards.
2. Ensure you are logged in to the correct account.
3. Refresh your browser or app and try again.

---

## Common Issues for API Users

### 1. Problem: Invalid API Key or Token
**Cause**: The key or token used in the request is incorrect or expired.  
**Solution**:
1. Go to the [Trello API Key page](https://trello.com/app-key) and verify your API key and token.
2. If the token has expired, generate a new one.

---

### 2. Problem: Incorrect Parameters in Requests
**Cause**: Missing or invalid parameters in the API request.  
**Solution**:
1. Refer to the [API Documentation](../API/Endpoints.md) to verify the required parameters.
2. Ensure the parameter values match the expected types (e.g., `string`, `integer`).

---

### 3. Problem: API Rate Limits Exceeded
**Cause**: Too many requests sent to the API in a short period.  
**Solution**:
1. Review Trello’s rate limit guidelines and ensure your application respects the limits.
2. Add delays between API requests to avoid throttling.

---

## General Tips for Troubleshooting

1. **Check Trello Status**:
   - Visit [Trello Status](https://trello.status.atlassian.com/) to ensure there are no outages or maintenance.

2. **Clear Cache**:
   - If you encounter issues in the web app, clear your browser’s cache and cookies.

3. **Use Postman for API Testing**:
   - Test API requests in Postman to ensure your syntax and parameters are correct.

4. **Contact Support**:
   - For unresolved issues, contact Trello Support at [Trello Help](https://trello.com/contact).

---

## Notes

- If you are new to Trello, check the **Getting Started Guide** for setup instructions.
- For advanced tips, refer to the **Features Guide**.
