## Project: Automating User Deletion in Informatica Using Python
This project demonstrates how to automate the process of deleting users from a specific user group in Informatica using Python and the Informatica API. The script logs into the Informatica platform, retrieves user group details, and deletes all users from the group using API calls.

### How It Works:
#### 1. Login:

- The script logs into the Informatica environment using a username and password via a POST request.
- A session ID and base API URL are extracted from the response to authenticate further requests.

#### 2. Retrieve User Group Details:

- The script queries the Informatica API to retrieve details of a specific user group based on the group name provided. This includes retrieving the group ID and the list of users.

#### 3. Delete Users:

- The script then loops through each user in the group and sends a PUT request to remove them from the user group.

### Documentations:
- [Login API](https://docs.informatica.com/integration-cloud/b2b-gateway/current-version/rest-api-reference/platform-rest-api-version-3-resources/login.html)
- [Getting user group details API](https://docs.informatica.com/integration-cloud/b2b-gateway/current-version/rest-api-reference/platform-rest-api-version-3-resources/user-groups/getting-user-group-details.html)
- [Deleting a user group API](https://docs.informatica.com/integration-cloud/b2b-gateway/current-version/rest-api-reference/platform-rest-api-version-3-resources/user-groups/deleting-a-user-group.html)
