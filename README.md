🛒 FakeStore API Testing Project

📌 Project Overview

This project demonstrates API Testing of the FakeStore API using Postman.  

The primary goal of this project is to validate API functionality, verify API responses, and perform both positive and negative testing on different API endpoints.

The project includes:

- Authentication API Testing
  
- Product API Testing

- Cart API Testing

- API Response Validation
  
- Status Code Validation
  
- Response Time Validation
  
- Environment Variable Handling
  
- CRUD-based API Operations

This project helped in gaining hands-on experience with REST API Testing using Postman.


🛠 Tool Used

- Postman


📂 APIs Covered

🔐 Authentication API

 ✅ Valid Login
 
- Verify successful login with valid credentials
  
- Validate authentication response

❌ Invalid Login Credentials
- Verify error response for invalid username/password
  
- Validate unauthorized response status

 ⚠ Missing Field Validation
- Verify validation behavior when required fields are missing



📦 Products API

✅ Get Products API

- Fetch product list successfully
  
- Validate response data
  
- Validate product list is not empty
  
- Validate response status code


 🛒 Cart API

✅ Add Product to Cart

- Add products successfully into cart
  
- Validate request and response data
  
 ✅ Delete Cart API
 
- Delete existing cart successfully
  
- Validate delete operation response



✅ Test Scenarios Covered

- Positive Testing
  
- Negative Testing
  
- API Response Validation
  
- Status Code Validation
  
- Response Time Validation
  
- JSON Response Validation
  
- Environment Variable Usage



🧪 Sample Postman Test Scripts

Status Code Validation


pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});


Response Validation


pm.test("Products not empty", function () {
    var jsonData = pm.response.json();
    pm.expect(jsonData.length).to.be.above(0);
});


Response Time Validation

pm.test("Response time is less than 2000ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(2000);
});


📁 Project Structure



fakestore-api-testing-project

│

├── collections

│   └── FakeStore_API_Collection.json

│

├── environments

│   └── QA_Environment.json

│

├── screenshots

│   ├── collection-overview.png

│   ├── successful-api.png

│   └── invalid-login.png

│

└── README.md




📸 Screenshots Included

- Collection Overview

- Successful API Response

  
- Negative Testing Response



🚀 How to Execute the Project

1. Clone  the repository
   
2. Open Postman

3. Import the Collection JSON file
   
4. Import the Environment JSON file
   
5. Select QA Environment
   
6. Run APIs individually or using Collection Runner



📖 Learning Outcomes

Through this project, I gained practical experience in:

- REST API Testing using Postman
  
- Writing Postman Test Scripts
  
- Positive & Negative Testing
  
- API Response Validation
  
- Status Code Validation
  
- Response Time Validation
  
- Working with Environment Variables
  
- CRUD-based API Operations


👩‍💻 Author

Usha Nazare
