# About Project

This project is the current news feeds portal. We can view/read the news which are actively being updated.
The news are also categorised to get the category based news.

Source News API : https://newsapi.org/

## I am using free tier so it provides only 1000 calls in 24 hours. So, it may not update the data to store if the given quota is fnished.

### In the condtion of exhausted API call limits

I've used .env file to get the API Key and there i've stated 3 API keys named (REACT_APP_API_KEY,REACT_APP_API_KEY_1,REACT_APP_API_KEY_2).
You can find and replace all the occurance of the keys in the actions and testing files according to your convenience.

## This is the React web application for a news feeds platform.

The main focus here is to create a super fast and production-ready application.
<br>
Following are the highlights of this project:

- **React web app**: The [**News API**](https://newsapi.org/) provides news feeds according to different arguments passed to it. Which is displayed on the frontend side using ReactJS.
- **React Hooks**: This application uses hooks APIs from React, Redux, React Router and other libraries.
- **Separation of concern principle is applied**: Each component has been given a particular role. The role of the components is mutually exclusive.
- **Feature encapsulation is adopted**: The files or components that are related to a particular feature have been grouped unless those components are required in multiple features. This enhances the ability to share code across projects.
- **State management using Redux**: The Redux architecture is very well suited for scalable web apps. It is excellent in server side rendering for components that need data from the API server. It is also preferred over the context in the project.
- **Latest libraries and patterns**: All the libraries used in this project are standard, concerning the latest and modern web development practices.
- **Testing Library**: I've used Jest to implement unit test cases on my redux async actions calls.

## Architecture of an UI component

<p align="center">
   <img src="./src/images/ui-component-architecture.png">
</p>
<br>

## How to build and run this project

- Install nodejs if you already don't have it on your machine. Which will provide you the access to npm package manager.
- Navigate to the root of the project.
- Install all the dependencies which our project will require. Write `npm install` in the terminal
- After successful installation of dependencies, Run the project:
  - Development: Execute `npm run watch`
  - Production: Execute `npm start`
- You will be able to access the website from locally on your browser on port 3000

## Website Pages

- Landing (Dashboard)
- News Details Page
- Categorised News Listing

## Project Directory Structure

```
.
new_updates/
┣ public/
┃ ┣ favicon.ico
┃ ┣ index.html
┃ ┣ logo192.png
┃ ┣ logo512.png
┃ ┣ manifest.json
┃ ┗ robots.txt
┣ src/
┃ ┣ components/
┃ ┃ ┣ common/
┃ ┃ ┃ ┣ carousel.js
┃ ┃ ┃ ┣ catogies.js
┃ ┃ ┃ ┣ header.js
┃ ┃ ┃ ┣ sports.js
┃ ┃ ┃ ┗ topTech.js
┃ ┃ ┣ category.js
┃ ┃ ┣ details.js
┃ ┃ ┗ home.js
┃ ┣ images/
┃ ┣ redux/
┃ ┃ ┣ actions/
┃ ┃ ┃ ┗ newsActions.js
┃ ┃ ┣ reducers/
┃ ┃ ┃ ┗ newsReducers.js
┃ ┃ ┗ types/
┃ ┃   ┗ newsTypes.js
┃ ┣ route/
┃ ┃ ┗ route.js
┃ ┣ __testing__/
┃ ┃ ┗ newsActions.test.js
┃ ┣ App.css
┃ ┣ App.js
┃ ┣ App.test.js
┃ ┣ index.css
┃ ┣ index.js
┃ ┣ logo.svg
┃ ┣ reportWebVitals.js
┃ ┣ setupTests.js
┃ ┗ store.js
┣ .gitignore
┣ news_update.zip
┣ package-lock.json
┣ package.json
┗ README.md
```
