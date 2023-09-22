<a name="readme-top"></a>


<div align="center">
  <h1><b>Meet App</b></h1>
</div>

<!-- TABLE OF CONTENTS -->

# Table of Contents

- [About the Project](#about-project)
  - [Built With](#built-with)
    - [Tech Stack](#tech-stack)
    - [Key Features](#key-features)
  - [Live Demo](#live-demo)
- [User stories and scenarios](#user-stories)
- [Author](#authors)

<!-- PROJECT DESCRIPTION -->

# About Meet App <a name="about-project"></a>

**Meet App** is a serverless, progressive web application (PWA) with React using a
test-driven development (TDD) technique. The application uses the Google
Calendar API to fetch upcoming events.

## Built With <a name="built-with"></a>

### Tech Stack <a name="tech-stack"></a>

React.js, TDD testing tools, Google Calendar API, OAuth2 for authentication, AWS Lambda for serverless functions, GitHub for version control, cross-browser and responsive design, PWA features, GitHub Pages for deployment, OOP for alerts, data visualization libraries, extensive test coverage, and performance monitoring tools.


<!-- Features -->

### Key Features <a name="key-features"></a>

- **Filter Events by City**
- **Show/Hide Event Details**
- **Specify Number of Events**
- **Use the App When Offline**
- **Add an App Shortcut to the Home Screen**
- **Display Charts Visualizing Event Details**

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- User Stories and Scenarios -->

## User Stories and Scenarios <a name="user-stories"></a>

### User storie 1 - Filter Events by City
As a user, I would like to be able to filter events by city so that I can see the list of events that take place in that city.
	
- **Scenario 1: When user hasn’t searched for a city, show upcoming events from all cities.**
    Given user hasn’t searched for any city;
    When the user opens the app;
    Then the user should see a list of upcoming events.

- **Scenario 2: User should see a list of suggestions when they search for a city.**
    Given the main page is open;
    When user starts typing in the city textbox;
    Then the user should receive a list of cities (suggestions) that match what they’ve typed.

- **Scenario 3: User can select a city from the suggested list.**
    Given user was typing “Berlin” in the city textbox AND the list of suggested cities is showing;
    When the user selects a city (e.g., “Berlin, Germany”) from the list;
    Then their city should be changed to that city (i.e., “Berlin, Germany”) AND the user should receive a list of upcoming events in that city.

### User storie 2 - Show/Hide Event Details
As a user, I would like to be able to show/hide event details so that I can see more/less information about an event.

- **Scenario 1: An event element is collapsed by default**
	Given the main page is open;
  When the user views an event in the events list;
  Then the event details of that event should be collapsed by default and the user should see only summary information about the event.

- **Scenario 2: User can expand an event to see details**
	Given the user is on the event listing page;
  When the user clicks on the "Show Details" button for a specific event;
  Then the user should see additional details about that event and the "Show Details" button for that event should change to "Hide Details".

- **Scenario 3: User can collapse an event to hide details**
	Given the user is on the event listing page and the user has already expanded the details for a specific event;
  When the user clicks on the "Hide Details" button for that event;
  Then the user should see only the basic event information and the "Hide Details" button for that event should change back to "Show Details". 


### User storie 3 - Specify Number of Events
As a user, I would like to be able to specify the number of events I want to view in the app so
that I can see more or fewer events in the events list at once.

- **Scenario 1: When user hasn't specified a number, 32 events are shown by default**
	Given the main page is open;
  When the user selects a city from the list and doesn't input a number in the "Number of events:" field;
  Then the app should display 32 events in the events list by default.


- **Scenario 2: User can change the number of events displayed**
	Given the user is on the event listing page;
	When the user input a number in the "Number of events:" field;
	Then the app should update the amount of events displayed to the inputed number.

### User storie 4 - Use the App When Offline
As a user, I would like to be able to use the app when offline so that I can see the events I viewed the last time I was online.

- **Scenario 1: Show cached data when there's no internet connection**
	Given the user has previously used the app with an internet connection and the user has viewed events while online;
  When the user opens the app without an internet connection;
  Then the app should display the cached event data and there should be no network-related error messages.

- **Scenario 2: Show error when user changes search settings (city, number of events)**
	Given the user has previously used the app with an internet connection and the user has viewed events while online;
  When the user changes the search settings, such as city or number of events and the user attempts to apply the changes without an internet connection;
  Then the app should display an error message indicating the need for an internet connection and the app should not apply the changed search settings until an internet connection is available.

### User storie 5 - Add an App Shortcut to the Home Screen
As a user, I would like to be able to add the app shortcut to my home screen so that I can
open the app faster.

- **Scenario 1: User can install the meet app as a shortcut on their device home screen**
	Given the user has the app installed on their device;
  When the user opens the app and the user navigates to the app's settings or options;
  Then the user should see instructions on how to add the app to the home screen and following the instructions, the app shortcut should be added to the device's home screen.

### User storie 6 - Display Charts Visualizing Event Details
As a user, I would like to be able to see a chart showing the upcoming events in each city so
that I know what events are organized in which city.

- **Scenario 1: Show a chart with the number of upcoming events in each city**
	Given the user has selected a city to see the events;
	When the events list loads on the page;
	Then the chart with number of upcoming events for that city should be displayed before the individual events.

### Serverless functions
In the Meet app, serverless functions will play a crucial role in handling authorization for accessing public calendar events from the Google Calendar API. Users need to be authorized to retrieve event data for rendering in the React app. This authorization is facilitated by serverless functions, which are a more efficient alternative to building and maintaining a full server for this purpose. In this context, serverless functions will generate and provide access tokens, ensuring secure access to the Google Calendar API. AWS Lambda will be the chosen cloud-service provider for implementing these serverless functions, making the app's architecture more scalable and cost-effective.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LIVE DEMO -->

## 🚀 Live Demo <a name="live-demo"></a>

- [Live Demo Link - coomming soon](https://google.com)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- AUTHORS -->

## Author <a name="authors"></a>

**Caroline Pimenta**

- GitHub: [@pimentacaroline](https://github.com/pimentacaroline)
- Website: https://carolinepimenta.com

This is a solo project guided by tutors and Mentors from <a href="https://careerfoundry.com/en/courses/become-a-web-developer/">CareerFoundry.</a>



