# Building Microservices with .NET Core 2.0 - Second Edition
This is the code repository for [Building Microservices with .NET Core 2.0 - Second Edition](https://www.packtpub.com/application-development/building-microservices-net-core-20-second-edition?utm_source=github&utm_medium=repository&utm_campaign=9781788393331), published by [Packt](https://www.packtpub.com/?utm_source=github). It contains all the supporting project files necessary to work through the book from start to finish.
## About the Book
The microservice architectural style promotes the development of complex applications as a suite of small services based on business capabilities. This book will help you identify the appropriate service boundaries within your business. We'll start by looking at what microservices are and their main characteristics.

Moving forward, you will be introduced to real-life application scenarios; after assessing the current issues, we will begin the journey of transforming this application by splitting it into a suite of microservices. You will identify service boundaries, split the application into multiple microservices, and define service contracts. You will find out how to configure, deploy, and monitor microservices, and configure scaling to allow the application to quickly adapt to increased demand in the future.

With an introduction to reactive microservices, you strategically gain further value to keep your code base simple, focusing on what is more important rather than on messy asynchronous calls.

## Instructions and Navigation
All of the code is organized into folders. Each folder starts with a number followed by the application name. For example, Chapter02.



The code will look like the following:
```
[HttpGet]
[Route("GetProductSync")]
public IActionResult GetIsStillSynchronous()
{
var task = Task.Run(async() => await
_productRepository.GetAllAsync());
return new OkObjectResult(task.Result.ToViewModel());
}
```

All supporting code samples in this book are tested on .NET Core 2.0 using Visual Studio
2017 update 3 and SQL Server 2008R2 or later on a Windows platform.

## Related Products
* [Building Microservices with Go](https://www.packtpub.com/application-development/building-microservices-go?utm_source=github&utm_medium=repository&utm_campaign=9781786468666)

* [Microservices with Kotlin](https://www.packtpub.com/web-development/microservices-kotlin?utm_source=github&utm_medium=repository&utm_campaign=9781788471459)

* [Microservices with Clojure](https://www.packtpub.com/application-development/microservices-clojure?utm_source=github&utm_medium=repository&utm_campaign=9781788622240)

### Suggestions and Feedback
[Click here](https://docs.google.com/forms/d/e/1FAIpQLSe5qwunkGf6PUvzPirPDtuy1Du5Rlzew23UBp2S-P3wB-GcwQ/viewform) if you have any feedback or suggestions.
