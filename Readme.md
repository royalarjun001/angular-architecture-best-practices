# Angular Architecture and Best Practices

## Planning the Application Architecture.

### Architecture Considerations

1. _Application Overview_ - Like what is application is for and how clients will going to use it and what advantage it will provide to them as term of business.
1. _Application Features_ - We might not have all the feature in starting but we have some thing to start hences, start listing all these features so that we can deal with specifics.
1. _Domain Security_ - Like roles on the server side, groups, claims, is it token based or some thing else like LDAP server.
1. _Domain Rule_ - What are domain rules we have, do it will be running on client side stricly, or on the Server side. Or on both places like validation.
1. _Logging_ - what we are doing when some error happens in the front end side of the application. Using local log or API based logging server infomrations.
1. _Services/communications_ - Http, Https. web sockets and other data exchange machinsums. Might help in state management in future.
1. _Data Modals_ - Planning for the most efficient way to Set or sub set of data to be rom arround in the application. 
1. _Feature Components_ - Structuring of the Componenets, It help in the communication of the components. 
1. _Shared Functionality_ - What kind of sharble functionality do we have like ... third party, native Libraries etc.

This are the main 9 point to be considered as a blue print of the application.
