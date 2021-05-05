# Link Social Media

## Project Description
Link is the second iteration of a social media application created by Team Avatar as part of the Revature Full Stack Angular training program in April 2021. Developed with a microservice architecture, this web application allows every user to follow each other and view each other's posts. Each user has their own account that they can customize with their own information. Within this network, users can interact with each other through comments, likes, and a global chatroom. This social media application is meant to ease the transition of becoming a Revature employee.

## Technologies Used

- Spring Boot
	- Euereka Discovery Client
	- Spring Boot Actuator
	- Spring Web MVC
	- Lombok
	- Spring Mail
	- Java Persistence API
- Java - version 1.8
- PostgrSQL - version 13.2
- AWS Java S3 SDK
- Auth0 JSON Web Token
- JUnit
- Log4J
- H2 Database Testing
- Angular - version 8
- TypeScript
- HTML5
- CSS3
- Jasmine
- Karma
- StompJS - version 2.3.3
- SockJS - version 1.5.1
- SweetAlert2 - version 10.16.0

## Core Features

- Register an account and login.
- Create posts and interact with other posts.
- Search for users.
- View posts made by followed accounts.
- Create and edit personal profile information (bio, profile pic, email, password, etc).
- Chat with others in a global chatroom.
- Upload and share images and media.
- Receive personalized notifications.
- Account registration with MD5 hashed password.
- Login / Logout management with JWT authentication.
- Sends email messages during password reset process.
- Protects routes from unauthorized accesses with JWT checks.
- Like other posts in a feed.
- Comment on other posts.
- Images are uploaded to an S3 bucket.

## Getting Started
   
> Clone all Service Repositories
```
git clone https://github.com/LinkSocialNetwork/Eureka.git
git clone https://github.com/LinkSocialNetwork/Gateway.git
git clone https://github.com/LinkSocialNetwork/UserService.git
git clone https://github.com/LinkSocialNetwork/PostService.git
git clone https://github.com/LinkSocialNetwork/ChatService.git
git clone https://github.com/LinkSocialNetwork/NotificationService.git
```

> Clone FrontendClient
```
git clone https://github.com/LinkSocialNetwork/FrontendClient.git
```

> npm install in angular project folder
```
npm i FrontendClient/Angular
```

## **Usage**

> Run the services together, sequentially in an IDE
```
Eureka > Gateway > UserService > PostService > ChatService > NotificationService
```
>![01_running_services](https://user-images.githubusercontent.com/69532931/117219386-01c2d480-adba-11eb-9247-72b6afd549d7.png)


> Visit the Eureka url and confirm Eureka can see all the services above
```
http://localhost:9999/Eureka
```
>![02_Eureka_services](https://user-images.githubusercontent.com/69532931/117219665-94637380-adba-11eb-8817-76c373a791c2.png)

> Run angular project
```
cd FrontendClient/Angular
ng serve -o 
```
>![03_Angular_serve](https://user-images.githubusercontent.com/69532931/117220350-e5c03280-adbb-11eb-964c-9a918028140d.png)00

> Visit the frontend url
```
http://localhost:4200
```
>![04_loginpage](https://user-images.githubusercontent.com/69532931/117221177-9b3fb580-adbd-11eb-9ec6-205146fe7c1e.png)

>Create a new User
```
Hit the signup button to register a new user
Fill in the form and hit sign up once you are done
```
>![05_signup](https://user-images.githubusercontent.com/69532931/117221539-51a39a80-adbe-11eb-8ac9-19acb876e195.png)

>![06_newuser](https://user-images.githubusercontent.com/69532931/117222020-59177380-adbf-11eb-9316-5b052f638ed3.png)

>Sign in new user

>![07_signin](https://user-images.githubusercontent.com/69532931/117222130-9aa81e80-adbf-11eb-8e6a-36115b3d80c2.png)

>Home feed

>![08_home_feed](https://user-images.githubusercontent.com/69532931/117222273-ed81d600-adbf-11eb-9ca2-18e53046f7aa.png)

>There is no posts so lets make a new post
```
Write something in the text box and once you are done hit the post button to submit
```
>![09_first_post](https://user-images.githubusercontent.com/69532931/117222718-faeb9000-adc0-11eb-803c-6f53a9fe53b9.png)

```
Now we have a new post!
```
>![10_first_post_2](https://user-images.githubusercontent.com/69532931/117222828-3f772b80-adc1-11eb-9aac-331f7bf3a48a.png)

>We can add images and videos to our post as well
```
Hit the image tab
```
>![11_add_image](https://user-images.githubusercontent.com/69532931/117222980-8c5b0200-adc1-11eb-875d-fc96f3144d77.png)
```
Hit the browse button and add an image
Notice the image preview
Hit the post button once you are ready to submit
```
>![12_add_image_2](https://user-images.githubusercontent.com/69532931/117223047-aeed1b00-adc1-11eb-86ce-dd2cf242634a.png)








## **License**

This project uses the following license: [<The MIT License>](https://www.mit.edu/~amini/LICENSE.md).
