
# Lab Project Assignment Management Service with store-admin in Aldonquin Pet Store
The Algonquin Pet Store is a full-stack web application and management service is a backend service.To create and integrate the managment service we need to follow a structured approch for deployment. It intergrate the rabbitmq to retrive order messages.

### Features
- retrive order messages from RabbitMQ.
- Provide the REST API for accessing the information from order service.
- Deployment is done on Azure Web App.

### Step 1: Clone the Repository
Clone the repository:
```bash
git clone https://github.com/dua00006/managment-service.git
```
### Step 2: Configure the environment 
```bash
RABBITMQ_CONNECTION_STRING=amqp//:newuser:newpassword@<vm IP>:5672s
PORT=5600
```
### Step 3: Install the dependencies 

### Step 4: Run the service
```bash
python3 src/server.py
```
Test the server locally. Then connect to RabbitMQ and test.

### DEPLOYING THE MANAGMENT SERVICE ON WEB APP

1. Create Azure web app on azure portal. Once created add the variables with amqp for RabbitMQ and the PORT on which the managment service will run.
2. Create a workflow file.
3. Choose the repository from github and deploy and build.
4. Verify the deployment in github after pushing the code to the main branch.
5. Deleting all the resources after completion.

### Testing the Service

Test the service in .http file in vs code by send request and view the respone.

### Steps: 
1. Open vs code.
2. Go to test.http
3. Click on "Send Reques".
4. View the response.

### CONCLUSION

The managment-service provides the essential service to the order managment in Algonquin Pet Store.

