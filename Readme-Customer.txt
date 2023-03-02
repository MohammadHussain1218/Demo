Customer Module:
Tomcat server port no : 9095


==================================================== POST method ==============================================
Inserting customer records
method : POST

URL: http://localhost:9095/customer/addCustomer

Postman: Body :  Raw : JSON : 
Record-1: ------------------
{
	"customerName":"ravi",
	"mobileNumber":1231230,
	"emailId":"ravi@gmail.com",
	"password":"ravi@1"
}
Record-2:-------------------
{
	"customerName":"raju",
	"mobileNumber":1000121,
	"emailId":"rajul@gmail.com",
	"password":"raju@1"
}


========================================================PUT method ============================================
Updating the customer record by customer id:
method : PUT

URL : http://localhost:9095/customer/updateCustomer/{customerId}

URL : http://localhost:9095/customer/updateCustomer/3

Postman: Body :  Raw : JSON : 
{
	"customerName":"raju",
	"mobileNumber":1111111,
	"emailId":"rajul@gmail.com",
	"password":"raju@3"
}

====================================================== GET method =============================================
View record by ID-----------------------------------
method : GET

URL : http://localhost:9095/customer/viewCustomer/{customerId}

URL : http://localhost:9095/customer/viewCustomer/2

Postman Output: {
    				"customerId": 1,
   					"customerName": "ravi",
 				    "mobileNumber": 1231230,
    				"emailId": "ravi@gmail.com",
    				"password": "ravi@1"
				}


View All records ----------------------------------
method : GET

URL : http://localhost:9095/customer/viewAllCustomer

Postman Output:[
    				{
   					    "customerId": 1,
        				"customerName": "ravi",
        				"mobileNumber": 1231230,
        				"emailId": "ravi@gmail.com",
        				"password": "ravi@1"
    				},
    				{
        				"customerId": 2,
        				"customerName": "rahul",
        				"mobileNumber": 1202301,
        				"emailId": "rahul@gmail.com",
        				"password": "rahul@1"
    				},
    				{
        				"customerId": 3,
        				"customerName": "raju",
        				"mobileNumber": 1111111,
        				"emailId": "rajul@gmail.com",
        				"password": "raju@3"
    				}
				]


====================================================== DELETE method ==================================
Deleting customer record by customer id:
method : DELETE

URL : http://localhost:9095/customer/delete/{customerId}

URL : http://localhost:9095/customer/delete/2

				
	