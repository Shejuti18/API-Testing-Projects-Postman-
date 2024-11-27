GoRest API Testing:

Gorest APi url : https://gorest.co.in/

End points to test:
POST    	/public/v2/users		Create a new user
GET     	/public/v2/users/6942457	Get user details
PUT|PATCH 	/public/v2/users/6942457	Update user details
DELETE 		/public/v2/users/6942457	Delete user

Access Token : 372c4865736fd847287a2abfeb610da0dfd38e363e648ce37725142aa5da3030

Request body for POST or PUT request: bcz for post and put request only response body or data is needed.

{
  "name":"Tenali Ramakrishna", 
  "gender":"male", 
  "email":"tenali.ramakrishna@15ce.com", 
  "status":"active"
}

Now i will do API chaining concept for these requests in POSTMAN.

>created a collection name GorestAPI
>added requests POST,GET,PUT,Deelete
>Executed Sucessfully




*Things to remember: 
1. i cant create post requests with same data. So everytime the data have to be different. Thats why we need to dynamically change this data for every time whenever we are sending request. Thats why we need to write some scripts that needed to be send before sending the request. So we need to write the scripts on the "Pre Request Script"  . We  write this script in javascript using "random" function to create random data.
