HubMinds
=======================================
UP2110375
UP2108568
UP2110125
UP2112778
UP2129277
UP2054746

Intro
---
Welcome to the HubMinds app, we designed this application to be an all-in-one smartphone app that can have all the information that the user would need. With our Hub, you can access the current news storys, the weather forecast in three hour intervals and also a calendar that can be used to plan events. All on a customisable screen.

The Scope
------
We aimed to build an application with four main components: weather, calendar, news, and bus routes. However, we were only able to complete the weather, news, and calendar components:

- **Weather:** We wanted to create an accurate real-time weather forecast that provides temperature, humidity, wind, and more, using an API for real-time data.

- **Calendar:** The calendar is not just a standard display but interactive, allowing users to add and manage events with detailed descriptions.

- **News:** Using an API, we fetch the latest news stories, allowing users to browse headlines and read full articles.

User Requirements
------------
1. **Adding Personal Information:** Implement a feature for users to add personalized calendars and reminders.

2. **Interface Preferences:** Develop a modular app with customizable widgets and a notification system to cater to various user preferences.

3. **Morning Check Routine:** Provide tools for a personalized morning routine with real-time updates on weather, news, and schedules.

4. **User Support and Training:** Implement a tutorial with an opt-out option for users of varying technological proficiency levels.

Instructions on How to Set Up/Run Your Project
----------------------
### Flutter App Setup
To get started with the HubMinds app, follow these setup instructions:

#### Prerequisites
Ensure Flutter is installed on your system. If you need to install Flutter, visit the [Flutter installation guide](https://flutter.dev/docs/get-started/install).

#### Clone the Repository
To set up the project, begin by cloning the HubMinds repository to your local machine:
```bash
$ git clone https://github.com/HubMinds/SmartHub-Flutter.git
$ cd SmartHub-Flutter

#### Install Dependencies
Next, install all the necessary dependencies for the project:
```bash
$ flutter pub get

#### Pod Install
Install ios dependencies:
```bash
$ cd ios
$ pod install
$ cd ..

#### Run the Application
Finally, launch the app on a connected device or emulator:
```bash
$ flutter run

### Python API Setup
To set up the backend API for HubMinds, which handles data fetching and processing, follow these instructions:

#### Prerequisites
Ensure you have Python installed on your system. Python 3.8 or newer is recommended. You also need pip for managing Python packages.

#### Setup Python Environment
It's recommended to use a virtual environment to keep dependencies organized and separate from your main system. Create and activate it with:
```bash
$ python3 -m venv env
$ source env/bin/activate  # On Windows use `env\Scripts\activate`

#### Install Dependencies
Install all required Python packages defined in a requirements.txt file:
```bash
$ pip install -r requirements.txt

#### Clone the Repository
To set up the API, clone the repository to your local machine:
```bash
$ git clone -b flask https://github.com/HubMinds/SmartHub-API.git
$ cd SmartHub-API

#### Run the API
On your server or locally, install pm2 and run the app.py:
```bash
$ pm2 start app.py --name flask-app --interpreter=/path/to/venv/python/binary

For a simple way to make the API internet facing, use ngrok:
```bash
$ pm2 start "ngrok http 5000" --name ngrok

With this method, you will have to replace the source code API url to fit your server.

Main Components
-----------

- Calendar - The calendar feature in our app provides users with a clean and visually appealing interface, displaying dates and existing events. Users can easily create new events by tapping on a specific date and time, entering details to describe what the event is. Also, the events are flexible so that once an event is created it can also be deleted by the user. 

- News - Our news function integrates with an API to deliver the latest headlines and articles. Users are greeted with an array of headlines when entering the news section, where they can easily scroll through and select articles of interest. Once the user has selected an article, the user is then displayed the full article from the news source. 

- Weather - Our weather feature uses an API, providing users with real-time weather data and forecasts for their location. Users can access current weather conditions, including temperature, humidity and wind speed. Additionally, the app offers detailed forecasts for future time intervals, in 3-hour segments, allowing users to plan ahead. Temperature and humidity information is displayed alongside images making it simple and easy for the user to understand. 

- Log In - The login page provides an easy to use and secure way for users to access their accounts. Users are prompted to input their registered email address and password into the text fields. There is also a registration button that can allow users to register their email and password, if they are first time users of the app, in order to access the app. Once the required information is entered, the user clicks the login button, and enters the app. The database stores the user email and passwords that are valid log in details.

- Feedback Form - This component works by the user entering the email that they used to access the app and then entering their desired feedback. in the text field suggested. The feedback is then sent to the firebase into a collection named feedback.
