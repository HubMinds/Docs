# HubMinds #

UP2110375
UP2108568
UP2110125
UP2112778
UP2129277
UP2054746

## Intro ##

Welcome to the HubMinds app, your all-in-one solution for staying informed and organized throughout your day! With our Hub, you can effortlessly access key information such as your calendar events, the latest weather updates, and breaking news, all in one convenient place. Whether you're planning your schedule, preparing for the day ahead, or simply staying up-to-date with the world around you, HubMinds makes it easy.

## The Scope ##

We aimed to build an application with four main components: weather, calendar, news, and bus routes. However, we were only able to complete the weather, news, and calendar components:

- **Weather:** We wanted to create an accurate real-time weather forecast that provides temperature, humidity, wind, and more, using an API for real-time data.

- **Calendar:** The calendar is not just a standard display but interactive, allowing users to add and manage events with detailed descriptions.

- **News:** Using an API, we fetch the latest news stories, allowing users to browse headlines and read full articles.

## User Requirements ##

1. **Adding Personal Information:** Implement a feature for users to add personalized calendars and reminders.

2. **Interface Preferences:** Develop a modular app with customizable widgets and a notification system to cater to various user preferences.

3. **Morning Check Routine:** Provide tools for a personalized morning routine with real-time updates on weather, news, and schedules.

4. **User Support and Training:** Implement a tutorial with an opt-out option for users of varying technological proficiency levels.

### Instructions on How to Set Up/Run Your Project ###

# Flutter App Setup #
To get started with the HubMinds app, follow these setup instructions:

# Prerequisites #
Ensure Flutter is installed on your system. If you need to install Flutter, visit the [Flutter installation guide](https://flutter.dev/docs/get-started/install).

# Clone the Repository #
To set up the project, begin by cloning the HubMinds repository to your local machine:
``` 
$ git clone https://github.com/HubMinds/SmartHub-Flutter.git
$ cd SmartHub-Flutter ```

# Install Dependencies #
Next, install all the necessary dependencies for the project:
``` 
$ flutter pub get ```

# Pod Install #
Install ios dependencies:
``` 
$ cd ios
$ pod install
$ cd .. ```

# Run the Application #
Finally, launch the app on a connected device or emulator:
``` 
$ flutter run ```

# Python API Setup #
To set up the backend API for HubMinds, which handles data fetching and processing, follow these instructions:

# Prerequisites #
Ensure you have Python installed on your system. Python 3.8 or newer is recommended. You also need pip for managing Python packages.

# Setup Python Environment #
It's recommended to use a virtual environment to keep dependencies organized and separate from your main system. Create and activate it with:
``` 
$ python3 -m venv env
$ source env/bin/activate  # On Windows use `env\Scripts\activate` ```

# Install Dependencies #
Install all required Python packages defined in a requirements.txt file:
``` 
$ pip install -r requirements.txt ```

# Clone the Repository #
To set up the API, clone the repository to your local machine:
``` 
$ git clone -b flask https://github.com/HubMinds/SmartHub-API.git
$ cd SmartHub-API ```

# Run the API #
On your server or locally, install pm2 and run the app.py:
``` 
$ pm2 start app.py --name flask-app --interpreter=/path/to/venv/python/binary ```

For a simple way to make the API internet facing, use ngrok:
``` 
$ pm2 start "ngrok http 5000" --name ngrok ```

With this method, you will have to replace the source code API url to fit your server.

# In case the Firebase is not linked properly here is how to link it #

# install the firebase CLI
``` 
$ https://firebase.google.com/docs/cli#setup_update_cli ```

# login to firebase CLI #
``` 
$ firebase login ```

# install flutterFire #
``` 
$ dart pub global activate flutterfire_cli ```

# configure FlutterFire in the directory containing your project #
``` 
$ flutterfire configure ```

# From your Flutter project directory, run the following command to install the core plugin: #
``` 
$ flutter pub add firebase_core ```

# From your Flutter project directory, run the following command to ensure that your Flutter app's Firebase configuration is up-to-date: #
```
$ flutterfire configure ```

# After these changes it should run #


Main Components
-----------

- Calendar - The calendar feature in our app provides users with a clean and visually appealing interface, displaying dates, days of the week, and existing events. Users can easily create new events by tapping on a specific date and time, entering details as what the event is. They have the flexibility to edit or delete events and view detailed information by clicking on them. 

- News - Our news function seamlessly integrates with an API to deliver the latest headlines and articles across various categories like world news, business, sports, and entertainment. Users are greeted with an attractive display of headlines upon entering the news section, where they can easily scroll through and select articles of interest. With a simple tap, users can access the full articles.

- Weather - Our weather feature uses with an API, providing users with real-time weather data and forecasts for their location. Users can easily access current weather conditions, including temperature, humidity and wind speed. Additionally, the app offers detailed forecasts for future time intervals, in 3-hour segments, allowing users to plan ahead. Temperature and humidity information is prominently displayed, aiding users in assessing comfort levels and the chance of rain. Weather data is presented in visually appealing formats, utilizing icons, colors, and intuitive layouts for easier understanding.

- Log In - The login page provides a secure gateway for users to access their accounts. Users are prompted to input their registered email address and password into the text fields. There is also a registration button that can allow users to register their email and password in order to access the app. Once the required information is entered, the user clicks the login button, and enters the app. The database stores the user email and passwords that are valid log in details.

- Feedback Form - This component works by the user entering the email that they used to access the app and then entering their desired feedback in the text field suggested. The feedback is then sent to the firebase into a collection named feedback.
