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

>We can also add videos to our posts

>![13_add_video](https://user-images.githubusercontent.com/69532931/117463701-d1d41800-af04-11eb-882f-7842e0f0c61b.png)

>![14_add_video_2](https://user-images.githubusercontent.com/69532931/117463730-d6003580-af04-11eb-91a0-cd48cb019be6.png)

>Users can comment on other posts

>![15_add_comment](https://user-images.githubusercontent.com/69532931/117463795-e7494200-af04-11eb-8d71-c50e8f43f6d6.png)

>![16_add_comment_2](https://user-images.githubusercontent.com/69532931/117463809-ea443280-af04-11eb-995b-b0670d4ac3dc.png)

>Users can like others posts

>![17_liking_post](https://user-images.githubusercontent.com/69532931/117463870-f6c88b00-af04-11eb-9510-56027da2883f.png)

>Notice in the top right a notification icon pops up

>![18_notification](https://user-images.githubusercontent.com/69532931/117463930-047e1080-af05-11eb-92f4-77849bdcff4f.png)

>Lets go view the users profile
```
Users can access their profile by either clicking the right image icon and clicking on my profile
Our users can click profile on the nav-bar
```

>![19_my_profile](https://user-images.githubusercontent.com/69532931/117464125-37c09f80-af05-11eb-87bf-2105e13d9095.png)

>![20_my_profile_2](https://user-images.githubusercontent.com/69532931/117464140-3abb9000-af05-11eb-871b-f11de5ffe4ff.png)

>This is the profile page. Notice on the left it loads only the users posts and on the right shows the users information. 

>![21_my_profile_3](https://user-images.githubusercontent.com/69532931/117464321-6179c680-af05-11eb-81bd-307738bbf6d8.png)

>Lets edit the users information
```
Hit the edit account below the users information
Lets change our account name, add a description and add a new profile page.
Hit the blue submit button when you are ready to submit. 
```
>![22_edit_profile](https://user-images.githubusercontent.com/69532931/117464746-d0efb600-af05-11eb-962f-002496d42d14.png)

>![23_edit_profile](https://user-images.githubusercontent.com/69532931/117464751-d3521000-af05-11eb-9ce1-3e7a05d9fea5.png)

>Now our profile has been updated. 

>![24_edit_profile_3](https://user-images.githubusercontent.com/69532931/117464893-f67cbf80-af05-11eb-83c6-9383e372ec5a.png)

>Lets view another users profile. 
```
Hit the users search in the nav-bar
```
>![25_search_users](https://user-images.githubusercontent.com/69532931/117465054-23c96d80-af06-11eb-81d4-953cdae652eb.png)

>It takes you to an empty page with a search bar. Lets lookup admin. 

>![26_search_users_2](https://user-images.githubusercontent.com/69532931/117465429-8b7fb880-af06-11eb-8fac-467fe3fbcdb1.png)

>![27_search_user_3](https://user-images.githubusercontent.com/69532931/117465436-8de21280-af06-11eb-82ea-8ebb3993c756.png)

>Similiar to our profile view it loads the users posts and their information on the right. 

>Lets follow admin.

>![28_follow_user](https://user-images.githubusercontent.com/69532931/117465955-0c3eb480-af07-11eb-9f52-96faa6dc9578.png)

>Now that we followed a user. We can go back to our home page and view the users posts in our home feed. 

>![29_first_follow](https://user-images.githubusercontent.com/69532931/117466074-2ed0cd80-af07-11eb-9e04-1c4e9312ab45.png)

>Lets go view our chatroom functionality. 
```
Hit the chatroom in the nav-bar
```

>Notice that your user is loggedin into the chatroom.

>![30_chatroom_2](https://user-images.githubusercontent.com/69532931/117466207-4c9e3280-af07-11eb-8c54-cd4ae5fa2ebf.png)

>Lets have our admin also log in. 

>![31_chatroom_2](https://user-images.githubusercontent.com/69532931/117466544-af8fc980-af07-11eb-821c-7313eb9d267d.png)

>Now that we have two users, let's have them talk to each other. 

>![32_chatroom_3](https://user-images.githubusercontent.com/69532931/117466608-c46c5d00-af07-11eb-8cfd-fee1c384620f.png)

>![33_chatroom_4](https://user-images.githubusercontent.com/69532931/117466615-c6ceb700-af07-11eb-9305-c29df5311325.png)

>![34_chatroom_5](https://user-images.githubusercontent.com/69532931/117466623-c8987a80-af07-11eb-9713-efca0f9a8142.png)

>We can also logout. Click on your profile image in the right corner and hit the logout. 

>![35_logout](https://user-images.githubusercontent.com/69532931/117466711-e239c200-af07-11eb-9d11-0ca1fd94300b.png)

>![36_loggedout](https://user-images.githubusercontent.com/69532931/117466726-e534b280-af07-11eb-9a41-3a85446a9b7b.png)


## **Contributors**

This product was created by: Revature Full Stack batch of March 2021


## **License**

This project uses the following license: [<The MIT License>](https://www.mit.edu/~amini/LICENSE.md).
