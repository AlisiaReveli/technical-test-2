# Technical test

## Introduction

Fabien just came back from a meeting with an incubator and told them we have a platform “up and running” to monitor people's activities and control the budget for their startups !

All others developers are busy and we need you to deliver the app for tomorrow.
Some bugs are left and we need you to fix those. Don't spend to much time on it.

We need you to follow these steps to understand the app and to fix the bug : 
 - Sign up to the app
 - Create at least 2 others users on people page ( not with signup ) 
 - Edit these profiles and add aditional information 
 - Create a project
 - Input some information about the project
 - Input some activities to track your work in the good project
  
Then, see what happens in the app and fix the bug you found doing that.

## Then
Time to be creative, and efficient. Do what you think would be the best for your product under a short period.

### The goal is to fix at least 3 bugs and implement 1 quick win feature than could help us sell the platform

## Setup api

- cd api
- Run `npm i`
- Run `npm run dev`

## Setup app

- cd app
- Run `npm i`
- Run `npm run dev`

## Finally

Fixes I made:
1. needed cors configuraton in sign up
2. user should be able to update name on the user update view
3. numeric values must be positive on the user update , business oriented fix
4. added also availability field  for updating, needed it because I couldn't find where I can update availability and I think it is the right space to add it 
5. I noticed password was visible when a user typed it(while creating user), I fixed it, made it with the standard bullet points, makes the platform more trusted
6. in the ProjectDetails component, you should check if project is defined before trying to access its properties., added a Loder there if the project wasn't defined,maybe a backend error happens for example and couldn't find project 
7. When you try to access a project, the way the backend sends the project is as an object inside an array. Therefore, you can either fix the way the backend sends the response, or you can handle the data differently in client side.
Send us the project and answer to those simple questions : 
- What bugs did you find ? How did you solve these and why ? 
- Which feature did you develop and why ? 
- Do you have any feedback about the code / architecture of the project and what was the difficulty you encountered while doing it ? 

