# Haystack Informatics take-home exercise
The purpose of this exercise is to demonstrate your thought process, implementation, and interpretation of a task similar to that which may occur at Haystack Informatics.  There is no right or wrong way to do this exercise, rather, we would like to simply get a sense for your general coding ability and style.  


While working on this exercise, please consider relevant edge cases and error handling, and leave comments in your code to help describe some of your thought processes.


This exercise consists of two parts:
1. ReactJS implementation of a basic API.
2. Minimal backend API with two endpoints.


## Frontend Application
We are most interested in seeing a ReactJS implementation.  There are 3 particular use cases for the UI that we are looking to see at a minimum:
- Main page - The default state of the application. This should display a brief description of the application, along with a method of navigating or viewing a patient list.
- Patient list - The ability to view the list of patients from the Backend API endpoint.
- Patient list - The ability to search for a specific patient from the Backend API endpoint.


## Backend API
You may use whatever language you feel most comfortable in.  We will provide a basic dataset that will need to be returned as a list or to be filtered for an endpoint.


### Provided dataset
In the `/data` folder there are two files, a [csv file](data/patients.csv) and [json file](data/patients.json).  Choose whichever one of these you prefer, and use it to provide data to the backend endpoints.

The data structure provided is as follows:
- full_name
- first
- last
- gender
- mrn
- id
- birthdate


### Endpoints

| Endpoint | Supported Methods | Description |
| -------- | ----------------- | ----------- |
| /        | GET | Description of the exercise |
| /patients| GET | List of patients          |


#### /
This endpoint should return a brief description about the project, it may be a static value that is returned.


#### /patients
This endpoint should return a list of patients for consumption of the frontend.


**Required use cases for endpoint**


| Argument | Expected output |
| --------- | --------------- |
| _(none)_ | Full list of patients |
| name | Patients `full_name` that match or have a partial match to the string provided |


## Requirements
**At a minimum:**
- [ ] Instructions on how to use/run your implementation of this exercise.
- [ ] Backend API has an endpoint of `/patients` in any language that you choose.
- [ ] Endpoint: `/patients` with no arguments returns a valid JSON list of patients.
- [ ] Endpoint: `/patients` with the name argument should return a valid list of patients that include that string in their `full_name`
- [ ] Frontend includes a main page that displays the description of the application, along with a method of navigating or viewing a patient list.
- [ ] Frontend view that shows a list of all patients (Showing the id, name, and mrn ) from the backend API.
- [ ] Frontend view that allows the ability to search for a specific string via the Backend API and shows the result.

**Bonus:**
- [ ] Add a Frontend view and Backend endpoint to view one patient specifically by mrn.
- [ ] Sortability of the patient list.
- [ ] Unit testing of any of the above logic.
- [ ] Anything you could think of that may be valuable in this application.
