# Angular Architecture and Best Practices

## Planning the Application Architecture.

### 1. Architecture Considerations

1. Application Overview - Like what is application is for and how clients will going to use it and what advantage it will provide to them as term of business.
2. Application Features - We might not have all the feature in starting but we have some thing to start hences, start listing all these features so that we can deal with specifics.
3. Domain Security - Like roles on the server side, groups, claims, is it token based or some thing else like LDAP server.
4. Domain Rule - What are domain rules we have, do it will be running on client side stricly, or on the Server side. Or on both places like validation.
5. Logging - what we are doing when some error happens in the front end side of the application. Using local log or API based logging server infomrations.
6. Services/communications - Http, Https. web sockets and other data exchange machinsums. Might help in state management in future.
7. Data Modals - Planning for the most efficient way to Set or sub set of data to be rom arround in the application. 
8. Feature Components - Structuring of the Componenets, It help in the communication of the components. 
9. Shared Functionality - What kind of sharble functionality do we have like ... third party, native Libraries etc.

This are the main 9 point to be considered as a blue print of the application.
