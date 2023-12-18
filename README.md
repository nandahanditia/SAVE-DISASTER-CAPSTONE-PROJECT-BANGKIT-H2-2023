# Endpoint Route

- ### User Authentication

  - **[POST]** _User Login_
  URL Route:
  `/auth/login`

    Additional Route: `<string:id>`

    Request:

    ```
    {
      "email": "user@example.com",
      "password": "user_password"
    }
    ```

    Response:

    ```
    {
      "error": false,
      "token": "user_access_token",
      "user": {
        "id": "user_id",
        "email": "user@example.com",
        "name": "User Name"
      }
    }
    ```

    ```
  - **[POST]** _User Logout_
  URL Route:
  `/auth/logout`

    Additional Route: `<string:id>`

    Request:

    ```
     {
      "token": "user_access_token"
    }
    ```

    Response:

    ```
   {
      "message": "Logout successful"
    }
    ```

    ```
- ### User Registration

  - **[POST]** _User Registration_
  URL Route:
  `/auth/register`

    Additional Route: `<string:id>`

    Request:

    ```
   {
      "name": "User Name",
      "email": "user@example.com",
      "password": "user_password"
    }
    ```

    Response:

    ```
    {
      "error": false,
      "message": "User registered successfully",
      "user": {
        "id": "user_id",
        "email": "user@example.com",
        "name": "User Name"
      }
    }
    ```

    ```
