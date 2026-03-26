# API Testing Guide (Browser & Frontend Only)

## Live API

```bash
https://es6-reviewca.onrender.com/users
```

##  How to Test the Application

This project can be tested using:

* Browser (for viewing data)
*  Frontend HTML (`index.html`) for full interaction


#  1. CREATE User (Using HTML Form)

### Steps:

1. Open `index.html` in your browser
2. Enter:

   * Name
   * Age
3. Click **Submit**

### Expected Result:

*  Message: *User created successfully*
*  JSON response displayed on the page
*  Data saved in database


# 2. READ Users (Using Browser)

### Steps:

1. Open this link in your browser:

```bash
https://es6-reviewca.onrender.com/users
```

### Expected Result:

* A list of users in JSON format:

```json
[
  {
    "_id": "...",
    "name": "Apollo",
    "age": 20
  }
]
```

#  3. UPDATE User (Using HTML)

### Steps:

1. Open `index.html`
2. Scroll to **Update User section**
3. Enter:

   * User ID (copy from browser GET request)
   * New name
   * New age
4. Click **Update**

# Expected Result:

*  Message: *User updated successfully*
*  Updated data displayed


#  4. DELETE User (Using HTML)

### Steps:

1. Open `index.html`
2. Scroll to **Delete User section**
3. Enter User ID
4. Click **Delete**

# Expected Result:

*  Message: *User deleted successfully*
*  Confirmation response displayed


#  How to Get User ID

1. Open:

```bash
https://es6-reviewca.onrender.com/users
```

2. Copy the `_id` field:

```json
"_id": "123abc..."
```


#  Frontend Features

The `index.html` file allows:

* Creating users
* Updating users
* Deleting users
* Viewing responses directly


 Notes

* Internet connection is required (API is hosted online)
* Ensure correct User ID is used for update/delete
* API is hosted on Render and may take a few seconds to wake up


 Conclusion

All CRUD operations (Create, Read, Update, Delete) can be fully tested using only a web browser and the provided frontend interface, without the need for external tools.
