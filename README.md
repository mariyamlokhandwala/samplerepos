# Steps to follow

1. Change the location of the MS ACCESS FILE in application.properties as per your system location

2. Start application
mvn spring-boot:run

3. USE POSTMAN TO EXECUTE REST API

GET  /rest/noauth/default/{accountID} last 3 month statement of the particular account ID
SAMPLE DATA accountID 1
user and admin both can perform this action 

GET /rest/auth/statementByAmount/{acountID}{minAmount}{maxAmount}
SAMPLE DATA accountID=1 minAmount=100 maxAmount=1000
only admin can perform this action

GET /rest/auth/statementByDate/{acountID}{start}{end}
SAMPLE DATA accountID=1 start=2015-02-20 end=2020-02-20
only admin can perform this action


