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

### Architecture Planning Template

**Benifit of using Planning Template**

If we do not have any template then it would be very long process. To reduce it we can create a simple shareable templates with multiple columns or slide like PowerPoint and in each template have one of the point from the Architecture Considerations and then this link are shared with the team and all can start filling what they know to come to very good conclusion as in very sort span of time. and keep them every one focused.

### Angular Style Guide

Do use the offcial [Angular Style Guide](https://angular.io/guide/styleguide) for the application.
* Coding conventions
* Naming rules
* Application structure
* Organizaing Module
* Creating and using components
* Creating and using servcies
* Lifecycle hooks

Help to keep the shape of the application in proper form even if there are large number of teams. Or after going through all the item we can boil it down to some specific rule if it don't seems right to follow all the official rules and Publish them and shared across your team.

### Other Considerations

* Accessibility 
* i18n
* Environments
* CI/CD
* CDN, container, server
* Unit testing
* End-to-end testing
* APIs
* Etc.

## Organizing Features and Modules

### Organizing Feature

> Do structure the app such that you
> can **L**ocate code quickly, **I**dentify the
> Code at a glance, keep the **F**lattest
> structure you can, and **T**ry to be **DRY**
> 
> - Angular Style Guide


**LIFT**
* Locate code quickly - Structure the code and files such that you need not to dig very much deep for finding any specific piece of code.
* Identify the code at a glance - How we name our files.
* Keep the flattest structure you can - disadvantage of nested strucuture
* Try to be Dry - every one knows.

1. Avoid `convention-based` structure - we create a folder like component and dump all the component there. Instead try to keep it `Feature-based` structure. Only use `convention-based` structure when we have lots of componenet children for the same parent, then something in the specific sub folder we can maintain a `convention-based` structure for the application.
1. use the `Angular CLI` to generate initial feature folder/component
1. Minimum of one module per feature
2. Avoid deeply nested folder, Because `Flat structure` this will help in refactoring, maintance and importing.

### Feature Modules

Most of the information is provided in Angular style guide. 
On addition to this, One thing on which we should give emphasis is that as in general practice, we usually create top level feature module and then add all the functionality on the same module at the root level. The potential issue with this approach is that, when multiple developer are working on it or multiple team is working on it then root component developer need to know all information about the sub functionality of the application which is not the case because when any bug and Change request is required then we need to check all the information or code associated with it, which should not be like that as we all try to follow single responsibilty principle. So what we should do in this case is to create a multiple sub module of the feature module and from there which can be loaded based on the route hence it will allow to keep the things clean and separate in case of Complete feature module.

### Core and Shared Modules
### Core and Shared Action
### Create/Consuming a Custom Library
### 







