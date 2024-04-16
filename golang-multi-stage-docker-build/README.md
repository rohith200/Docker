**Multi Stage Docker Build**

The main purpose of choosing a golang based applciation to demostrate this example is golang is a statically-typed programming language that does not require a runtime in the traditional sense. Unlike dynamically-typed languages like Python, Ruby, and JavaScript, which rely on a runtime environment to execute their code, Go compiles directly to machine code, which can then be executed directly by the operating system.

So the real advantage of multi stage docker build and distro less images can be understand with a drastic decrease in the Image size.

Building docker image without using multistage build. 
![image](https://github.com/rohith200/Docker/assets/42884535/0eaec676-7303-4a5d-8ade-2525be7d428f)
![image](https://github.com/rohith200/Docker/assets/42884535/d2c6f41d-61cc-4d28-a0a4-633daca6a629)
![image](https://github.com/rohith200/Docker/assets/42884535/2854975d-67cc-4f23-8dcc-d230d0858469)
We can see here the image size is around 871MB
![image](https://github.com/rohith200/Docker/assets/42884535/c7eea270-6436-44e7-8d07-87989f879daf)

Building a Docker image using Multistage build.
From the below image it is clear that we could see the same image which we have build above here, it reduced to 1.83MB which nearly reduced around 800%.
![image](https://github.com/rohith200/Docker/assets/42884535/aecc1b2b-3fe0-49a8-9bfe-c875c6ed5e3c)



