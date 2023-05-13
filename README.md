# EE551
Stevens EE551 Final project.

This is a submission for EE551 - Engineering Programming: Python

This project utilizes material covered in the course such as installed libraries, functions, if else statements, for loops, while loops and file ops.

The idea of the project I took on building is a Python tool that takes in a CSV sheet of public companies info such as their industry, geographic location, revenue, number of employees etc. and can search through the sheet for companies that match criteria user inputted via graphical user interface, and creates analytical graphs about this data and saves a new CSV sheet of the resultant companies that fit this criteria. Resultant graphs would be Employee count vs Revenue, Revenue vs. State, and a map of the US graphing these points based on longitude and latitude. This program would utilize different packages and modules like matplotlib, numpy, pandas, etc. and include many different functions.

Upon running the code the user is faced with the Graphical User Interface:

<img width="1712" alt="Screenshot 2023-05-02 at 1 22 25 PM" src="https://user-images.githubusercontent.com/78391004/235738927-a022e8e4-846e-4466-9143-d8da653adb44.png">

Where the user can:

(1) Input a range of criteria they want to search the CSV sheet for such as:

- Range of company revenue in millions of dollars. 
  - Algorithm checks if company is within specified revenue range.

- Employee count of company. 
  - Algorithm checks if company is within specified employee count range.

- Dollar sales per employee ratio in millions of dollars per employee. 
  - Algorithm checks if company is within specified $/emp range.

- Distance from a geographic landmark. 
  - Algorithm finds company's longitude and latitude and compares it with landmark and finds distance between them in miles, and checks if distance is <= than specified.

- Specific US state of headquarters. 
  - Checks if company state is equal to specified state.

(2) Select which criteria they want to search using the checkboxes on the left side.

The search algorithm then takes the user input and scans the information found in the CSV sheet to find which companies fit the specified criteria.

When the search algorithm is complete, a new resultant CSV sheet called "answer.csv" is saved and analytical graphs are printed.

I will run an example search where I am only looking for companies $0-20 million in revenue and 200 miles from JFK airport.

The following are example analytical graphs:

Master sheet analytics:

Employee count vs. Revenue

<img width="550" alt="Screenshot 2023-05-13 at 5 08 41 PM" src="https://github.com/tylercona/EE551/assets/78391004/04b51db6-3803-4c26-bd33-a4442570a0b5">

Revenue vs. State

<img width="1320" alt="Screenshot 2023-05-13 at 5 09 37 PM" src="https://github.com/tylercona/EE551/assets/78391004/a6a02df7-7e86-4efc-b882-99b0ef726da7">

Latitude vs. Longitude

<img width="550" alt="Screenshot 2023-05-13 at 5 10 27 PM" src="https://github.com/tylercona/EE551/assets/78391004/86a7f12e-b5fe-4c11-8941-881c4c496d28">

Resultant subset analytics:

Employee count vs. Revenue

<img width="550" alt="Screenshot 2023-05-13 at 5 17 37 PM" src="https://github.com/tylercona/EE551/assets/78391004/5538c034-f9de-437e-a2c6-fa3ba8860885">

Revenue vs. State

<img width="1318" alt="Screenshot 2023-05-13 at 5 18 12 PM" src="https://github.com/tylercona/EE551/assets/78391004/357c0b0a-9ec1-4c10-9681-aca16a80b873">

Latitude vs. Longitude

<img width="550" alt="Screenshot 2023-05-13 at 5 18 52 PM" src="https://github.com/tylercona/EE551/assets/78391004/bf04ace8-6857-46d9-a325-399530cc1b39">

