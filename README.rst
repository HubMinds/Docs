HubMinds
=======================================
-Fin UP2110375
-Jake UP2108568
Intro
---
Welcome to HubMinds app, your all-in-one solution for staying informed and organized throughout your day! With our Hub, you can effortlessly access key information such as your calendar events, the latest weather updates, and breaking news, all in one convenient place. Whether you're planning your schedule, preparing for the day ahead, or simply staying up-to-date with the world around you.

The Scope
------
We aimed to build an application with four main components: weather, calendar, news and bus routes. However, we were only able to complete the weather, news and calendar. 

- Weather - We wanted to create an accurate real time weather forecast that not only provides the temperature but other information like humidity and wind. Also, we planned for it to be able to give forecasts for later in the day not just the current time. This was achieved by using an API to obtain accurate weather forecasts for the requested location.

- Calendar - The calendar was intended to not only be a standard calendar that displays the current date but also to be interactive. Events can be added onto specific dates and times. Furthermore, descriptions for the events can be added aswell allowing the user to store their own specific events.

- News - An API was used to scrape the internet in order to obtain the latest news stories. The user can scroll throught the headlines and select any of them, this will in turn take the user to the full article. 


The user requirements 
------------
1. Adding Personal Information
User Feedback: Users expressed a strong desire to add their own information, such as a personalised calendar and reminders.
Analysis: The majority favours a modular approach, allowing users to customise the hub with their own content.
System Requirement: Implement a feature enabling users to add personalised information, including calendars, reminders, and customizable content on the hub.

2. Interface Preferences
User Feedback: Preferences for interface vary based on demographics, with professionals favouring widgets and seniors preferring simplicity.
Analysis: Almost all users wanted a modular app to avoid redundant data in regards to their needs but different ages and professionalism of users wanted to source the data in different ways such as notifications and widgets.
System Requirement: Develop both a modular app that is complimented by a customisable home screen widget and a push notification system to cater to diverse preferences.
Implementation: The user will be able to select what order they want the data to appear on the screen in and how they want it to be displayed.

3. Morning Check Routine
User Feedback: Varied morning routines, including checking weather, news, and schedules.
Analysis: Users prioritise different information based on their roles and responsibilities.
System Requirement: Provide real-time weather updates, customizable news feeds, and modular widgets for personalised morning check routines.
Implementation: The user will be able to select what time they want the roundup or they can select to not have it at all

4. User Support and Training
User Feedback: Mixed opinions on tutorials, with a preference for an option to opt-out.
Analysis: Acknowledgment of varying user proficiency levels.
System Requirement: Implement a tutorial with an opt-out option to enhance accessibility for users with different levels of technological familiarity.
Implementation: A opt-out tutorial on first login while remaining accessible whenever, additionally a support form for specific problems


Elements of implementation
-----------


Instructions on how to set up/run your project
----------------------
Clone the github repository
.. code-block:: bash
   $ git clone https://github.com/HubMinds/SmartHub-Flutter.git


Main Components
-----------

- Calendar - 
The calendar feature in our app provides users with a clean and visually appealing interface, displaying dates, days of the week, and existing events. Users can easily create new events by tapping on a specific date and time, entering details as what the event is. They have the flexibility to edit or delete events and view detailed information by clicking on them. 

- News - Our news function seamlessly integrates with an API to deliver the latest headlines and articles across various categories like world news, business, sports, and entertainment. Users are greeted with an attractive display of headlines upon entering the news section, where they can easily scroll through and select articles of interest. With a simple tap, users can access the full articles.

- Weather - Our weather feature uses with an API, providing users with real-time weather data and forecasts for their location. Users can easily access current weather conditions, including temperature, humidity and wind speed. Additionally, the app offers detailed forecasts for future time intervals, in 3-hour segments, allowing users to plan ahead. Temperature and humidity information is prominently displayed, aiding users in assessing comfort levels and the chance of rain. Weather data is presented in visually appealing formats, utilizing icons, colors, and intuitive layouts for easier understanding.
