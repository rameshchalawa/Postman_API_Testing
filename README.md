#**GorestApi_ChainingWithTokenAuth.postman_collection.json**

Gorest API – Chaining With Token Auth  
This repository contains a Postman collection for testing the GoREST Users API with request chaining and token-based authentication.  

**Published Documentation:** https://documenter.getpostman.com/view/51509819/2sBXVo9TG7  

**Running The Collection**  

Import the Postman collection into your workspace.  

Create the QA environment (or any environment) and set:  

url_gorest = https://gorest.co.in  

gorest_token = <your GoREST personal access token> (if using a variable)  
Select the environment in Postman.  
In the Collection Runner:  
Choose the GorestApi_ChainingWithTokenAuth collection.  
Ensure the environment is set (e.g., QA).  

Run the collection from top to bottom:  
-Create User  
-Get User Details  
-Update User  
-Delete Request and Env Variable  

Verify results:  

Create User returns 201 and sets userid_env.  
Get User Details and Update User return 200.  
Delete Request and Env Variable returns 204 and unsets userid_env.  

--------------------------------------------------------------------------------------------------  
#**PetStore_UserModel.postman_collection.json**  
PetStore – User Model (Postman Collection)  
This repository contains a Postman collection for testing the User endpoints of the public Swagger Petstore API.  
The collection focuses on CRUD operations for users, using the firstName as a path parameter (via a Postman variable) to demonstrate variable-based testing and simple workflows.  

**Published Documentation:** https://documenter.getpostman.com/view/51509819/2sBXVo8TGj  

**How To Use This Collection**  

Import the collection into Postman  
Use the Postman Import feature and select the PetStore_UserModel collection file.  
Set up an environment  

Create an environment (e.g., QA).  
Add:  
firstName = John (or any test username you prefer)  
petstore_base_url = https://petstore.swagger.io/v2  
Select your environment in Postman  

Click the environment dropdown at the top right and choose your environment.  
Run the workflow manually  

Execute requests in this order:  
-Create User  
-Get User By firstName  
-Update User By firstName  
-Delete User By firstName  

Inspect responses and confirm the expected behavior:  
User is created, then readable, then updatable, and finally deleted.  

**Run via Collection Runner**  
Open the Collection Runner.  
Select the PetStore_UserModel collection and desired environment.  
Run all four requests in order (1 iteration).  
Use the Runner results to quickly verify status codes and payloads.
