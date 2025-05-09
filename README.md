# API Testing with Postman Using Swagger (OpenAPI)

This guide explains how to use **Postman** to test APIs using a **Swagger (OpenAPI)** specification file. It includes steps for importing the API and sending a base request.

## 📦 Requirements

- [Postman](https://www.postman.com/downloads/)
- Internet connection 

---

## 🔁 Importing collection file into Postman

1. **Open Postman.**
2. In the top left, click on **"Import"**.
3. Upload the collection file (Swagger Books API.postman_collection.json) 
4. Click **Continue**, then **Import**.

Your API collection will be created automatically in Postman.

---

## 🧪 Sending a Base Request

1. Open the imported collection.
2. Select a request 
3. Ensure the **Base URL** is correct. Set it in the collection/environment if needed:
   - Click the gear icon (⚙️) in the top right.
   - Add a new variable with the URL of API books 
     ```
     API = https://fakerestapi.azurewebsites.net/api/v1/Books
     ```
   - In the request URL, replace hardcoded domains with `{{API}}`.

4. Set any required headers (e.g., `Content-Type: application/json`, `Authorization`, etc.).
5. Click **Send** to test the request.

---

## 📁 Collection Variables  

You can create and manage variables for:

| Variable     |  Value                     | 
|--------------|----------------------------|
| API    | https://fakerestapi.azurewebsites.net/api/v1/Books  | 


Use variables in requests like:
GET {{API}}
