# razorpay-payment-python_test_guide
Payment with Razorpay using python and flask

With reference from the following:-

		https://razorpay.com

		https://razorpay.com/docs/payment-gateway/web-integration/standard/   

		https://razorpay.com/docs/payment-gateway/server-integration/python/usage/

		https://github.com/razorpay/razorpay-python-testapp


This project is for understanding the integration of the Razorpay api using python, flask; setting up flask and acessing data between different html pages for different tasks(order_creation, making_payment, completing_payment). 

Used :- razorpay = 1.2.0, python3

## Steps to follow:

***Step 1)*** Make an account on [Razorpay](https://dashboard.razorpay.com/?utm_expid=.zXHqVB47Rw6qUb6ych9wOQ.0&utm_referrer=https%3A%2F%2Fdashboard.razorpay.com%2F#/access/signup).
		After that generate your test API Keys under the Settings option. Copy/Download your KeyId and KeySecret.  


***Step 2)*** Clone the repository on your desktop.


***Step 3)*** In the server.py file, replace the "KEY ID", "KEY SECRET" with your generated test "KeyId" and "KeySecret" and save the changes. For test purpose, enter the required amount of payment.


***Step 4)*** Open the repository on your desktop(here used Windows 10), then use the following command in your terminal(cmd) to setup a virtual environment using pip3 (for python3).

		> python3 -m venv test_env

For activating the virtual environment name test_env. We can give any name to the virtual environment, here we have given "test_env" (default is "venv")

		> test_env\Scripts\activate
			
			
***Step 5)*** Once you have activated the virtual environment, install the packages using requirements.txt.
			
		> pip3 install -r requirements.txt
			

***Step 6)*** Run the server.py file.

		> python3 server.py
				
	You will get a local address, enter the address in your browser. and that's it.

Later after the payment you can see that the payment is reflected in Transactions option in your Razorpay Dashboard.
			
			
The server.py generates three files named 

		'order_database.txt' containing order details,

		'payment_success_database.txt' containing payment_id,order_id,signature,

		'payment_detail_database.txt' containing detailed payment information.
		
		
***Step 7)*** After completing the testing deactivate the virtual environment.

		> deactivate
			
	This will deactivate the virtual environment and bring you back to normal cmd/terminal.


#### *Thank You!*
#### Hope that this was helpful. Kindly refer the references mentioned above / official Razorpay documentation for more info.
