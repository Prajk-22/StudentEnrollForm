#  **Login2explore**

##  **Student Enrollment Form**

**Description :** Student Enrollment Form that will store data in STUDENT-TABLE relation of SCHOOL-DB database. Input Fields: {Roll-No, Full-Name, Class, Birth-Date, Address, Enrollment-Date}

**Primary key:** Roll No.

It is a student registration form that saves the user's information in JSONPowerDB. Both serverless technology and REST APIs are supported. A student's roll number can be used to add or update them. The roll number is automatically verified on this form, and with the use of an API, the data submitted into other input fields is also verified so that the user can change as necessary. AJAX requests are used by the programme to enable quick and seamless interaction. Data of every kind, including numbers, strings, dates, and more, can be saved.

## **Benefits of using JsonPowerDB**
* Structured, semi-structured, and unstructured data, as well as various file formats and huge data, can be stored.
* CRUD operations with dynamic relational restrictions. 
* Simple to use in Memory,Real-Time.
* Schema free - easy to maintain.
* Serverless Support - fast development - cuts time to market.
* Multi-Mode database - one solution to variety of data.

## **Release History**
JsonPowerDB

Version: 1.0

### **Execute API**

```javascript
var baseUrl = "http://api.login2explore.com:5577";
function executeCommand(reqString, apiEndPointUrl) {
    var url = baseUrl + apiEndPointUrl;
    var jsonObj;
    $.post(url, reqString, function (result) {
        jsonObj = JSON.parse(result);
    }).fail(function (result) {
        var dataJsonObj = result.responseText;
        jsonObj = JSON.parse(dataJsonObj);
    });
    return jsonObj;
}
```
## Create a PUT Request String

```javascript
function createPUTRequest(connToken, jsonObj, dbName, relName) {
    var putRequest = "{\n"
            + "\"token\" : \""
            + connToken
            + "\","
            + "\"dbName\": \""
            + dbName
            + "\",\n" + "\"cmd\" : \"PUT\",\n"
            + "\"rel\" : \""
            + relName + "\","
            + "\"jsonStr\": \n"
            + jsonObj
            + "\n"
            + "}";
    return putRequest;
}

```
## Features

- Simple to Use
- Fast Response
- Detailed User Interface


## Tech Stack

**Client:** 
>HTML
>CSS
>Javascript
****
**Server:** 
>JsonPowerDB

# **Snapshots**

> ![first](https://github.com/user-attachments/assets/3a4349d1-0cd8-4747-85e1-d5a6bc35e07d)

> ![second](https://github.com/user-attachments/assets/46a253fc-fa70-4cef-8100-36c4c27c9201)

> ![third](https://github.com/user-attachments/assets/bf525a00-fb76-41bc-8a50-4415e3b9ed6d)

