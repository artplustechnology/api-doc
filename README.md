api-doc for wunder-v2

# User



# Work

**Get a work**
----
Return an array of works

* **URL**

  /api/v2/works
  
* **Method:**

  `GET**
  
* **URL Params**

  None
  
* **Data Params**

  None
  
* **Success Response:**

  * **Status** 200 <br />

* **Error Response**

* **Sample Call**
  ```javascript
    $.ajax({
      url: "/api/v2/works",
      dataType: "json",
      type : "GET",
      success : function(r) {
        console.log(r);
      }
    });
  ```

**Upload a work**
----
Return json data with status and message

* **URL**

  /api/v2/works/:bucket-name/upload

* **Method:**

  `POST`

* **URL Params**

  **Required:**

  `bucket-name=[string]`
  
* **Data Params**

  **Required**

  `ownerId=[string]`

  `title=[string]`

  `year=[number]`

  `material=[string]`

  `description=[string]`

  `timeextract=[string]` Format: HH:MM:SS
  
  `watermark=[string]`

  `user_file=[File]`

* **Success Response:**

  * **Status:** 200 <br />
    **Message:** `Uploaded successfully!`
 
* **Error Response:**


* **Sample Call:**
