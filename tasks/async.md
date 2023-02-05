# Async recruitment task

## Zadanie
Zadanie to jest na Junior++ 
Przy tej rekrutacji dostałem dwa zadania to poniżej oraz [TO](breweries.md) i miałem sobie wybrać, które chcę zrobić, zrobiłem oba.
Moje rozwiązanie tego zadania znajdziesz [TUTAJ](https://github.com/s0bieskii/AsyncTask)

Tutaj feedback od firmy dt. zadania:
```
Co było fajne:
    użycie apache.poi
Popracuj jeszcze nad:
    mapowanie modelu do czegoś wygodniejszego niż csv i dopiero na nim operować
    kod mocno zagmatwany, trudny do analizy
```

Treść zadania:

```
Please design and implement a simple REST API for asynchronous Tasks Processing.
Task description:
1. The API should allow to create a task, read the status and the results of the task.
2. When the task is created then the customer receives the unique id of the task.
3. The customer can check the status and the results of the task using the received id.
Functional requirements:
• Task accepts two numbers as the parameters: the base and the exponent
• The result of the task is the exponentiation result: baseexponent
• While one task is executing the next tasks can also be started and processed, API is not blocked
• The status of the task should contain the information about the progress
• Optional *: There is an endpoint that lists all the tasks with their statuses and results
Technical requirements:
• Provide a docker-compose file that prepares the required stack. Choose the tools and libraries on
your own.
• Use Spring Boot with Java 14+ (Spring initializr might be helpful https://start.spring.io/ )
• You may use Thread.sleep(1000) or similar approach so the tasks processing takes more time.
• Please use GitHub, Bitbucket or similar tool.
• Please document briefly how to start the application and how to use the API.

```

**Examples of using the API:**
<table class="table table-dark table-striped">
                        <thead>
                        <tr>
                          <th scope="col">Input</th>
                          <th scope="col">Output</th>
                        </thead>
  <tbody>
                        <tr>
                          <td>POST /tasks
{ base: 2, exponent: 10 }</td>
                          <td>{ id: 1 }</td>
                        </tr>
                        <tr>
                          <td>GET /tasks/1 </td>
                          <td>{ id: 1, status: running, progress: 40% }</td>
                        </tr>
<tr>
                          <td>POST /tasks
{ base: 5, exponent: 100 }</td>
                          <td>{ id: 2 }</td>
                        </tr>
<tr>
                          <td>GET /tasks/2</td>
                          <td>{ id: 2, status: running, progress: 2% }</td>
                        </tr>
<tr>
                          <td>GET /tasks/1 </td>
                          <td>{ id: 1, status: finished, progress: 100%, result: 1024 }</td>
                        </tr>
<tr>
                          <td>*optional
GET /tasks</td>
                          <td>{ [
{ id: 1, status: finished, progress: 100%, result: 1024 },
{ id: 2, status: running, progress: 4% } ]}</td>
                        </tr>
  </tbody>
</table>