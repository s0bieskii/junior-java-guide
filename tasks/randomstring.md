# Random string generator

## Zadanie

Zadanie podesłane przez znajomego. Niestety nie mam do niego rozwiązania.

```
Create a mini application in Java. Application need to generate a file with random unique strings (every string in a separate row).
Users should be able to define how long the string will be (min and max length), specify possible chars of string (from what characters string should be made) and how much string he wants.

Requirements:
Application should use maven or gradle as dependency tool.
App should have a connection to the local database (sqlite, mysql or any other) .
App need to have REST endpoints that will be used for communication with it.
one endpoint to receive new job (POST)
one endpoint to check how many jobs are running (GET)
one endpoint to grab results. (GET)
App needs to check how many combinations of strings we can make from provided chars and if the user wants more than we can make the app return a detailed error message. So if a user wants to get 1000 strings from chars “a,b,c” we should return an error message.
App should allow you to generate multiple results in parallel. So you can ask the app to generate 10 tasks and get first for example the last result. For example:
You send the first request to generate 1M of unique strings.
You send second request to generate 10k of unique strings
You send a third request to generate 100k of unique strings.
As the second request is the shortest one you should get results faster than from the first and third request.
App should be available to download on the git repository (github, gitlab ,bitbucket or anything else). 
After download there should be only one command to run an application and second one to run tests. You can use any framework you want (Dropwizard, Spring, SpringBoot or any other).
```