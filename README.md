<h1 align="center">Android Developer Roadmap 2023</h1>

![alt text](https://github.com/cp-radhika-s/Android-Roadmap/blob/main/image/og_image.png)


The Android Developer Roadmap 2023 includes **28 practical exercises** that cover all the essential concepts used in day-to-day development.
# Guidelines 
Before starting any practical, it's important to conduct research and learn the necessary concepts.

As you progress through the practical exercises, make sure to apply the new knowledge you've gained in subsequent exercises. Try to allocate no more than 3-4 days to each practical.

To keep track of your progress and share your work with your team lead, create a repository on GitLab where you can upload your completed exercises for review.

To stay organized and track your progress, create tickets on ClickUp for each practical exercise. Each ticket should include a detailed description of the exercise, as well as an estimate of story points.

As you work on each practical exercise, move the corresponding ticket from the "To-Do" queue to the "Done" queue to keep track of your progress. This will help you stay focused and motivated as you work through the roadmap.

# Table of contents
* [Android XML](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#android-xml)
* [Android Activity](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#android-activity)
* [Fragment](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#fragment)
* [Intent](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#intent)
* [Jetpack Compose](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#jetpack-compose)
* [Networking](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#networking)
* [App Architecture](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#app-architecture)
* [Datastore](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#datastore)
* [Database](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#local-storage)
* [Dependency Injection](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#dependency-injection)
* [Kotlin Coroutine & Flow](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#kotlin-coroutine--flow)
* [Broadcast Receiver](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#broadcast-receiver--task-scheduling)
* [Android Service](https://github.com/canopas/android-developer-roadmap-2023-/edit/main/README.md#android-service)

# Android XML
### Practicle 1

#### Develop an onboard and sign-in screen for Messaging application
* App should responsive for different resolutions.
* The onboard screen should provide a brief introduction to the app's features, such as messaging, voice and video calls, and file sharing.
* The sign-in screen should allow the user to enter their email and password, and validation should be added to ensure the user enters a valid email address and password.
* After a successful login, the user should be redirected to the Home screen.
* The user should not be able to go back to the login screen once redirected to the Home screen.
* Add support for day/night theme.
* Here's [UI for refrence](https://cdn.dribbble.com/userupload/3719280/file/original-5d6d206acf8adf5458091206369445f1.png?compress=1&resize=752x)

### Practicle 2
#### Develop collapsing toolbar for News application
* The toolbar should initially display the app's logo and title.
* As the user scrolls down to read an article, the toolbar should collapse to provide more space for the article.
* When the user reaches the end of the article and reverse scrolls, the toolbar should re-expand and display the app's title
* Here's [UI for refrence](https://cdn.dribbble.com/users/663782/screenshots/3742414/media/67464fde751beb373b4c6fa962edf718.gif)

### Practicle 3
#### Implement Survey application
* App should ask user about shopping experience. 
* Asks at least 3 questions with 4 options each. 
* Once the survey is completed, show a pop-up message thanking the user
* Here's [UI for refrence](https://cubicleninjas.com/wp-content/uploads/2021/01/NA-2021-Web-Questionnaire-3.jpg)

# Android Activity

### Practicle 4
#### Implement LocalTune player 
* An application can play a song from local resource. 
* The player should follow the activity lifecycle, pausing when the activity goes to the background and resuming when the activity returns to the foreground. 
* The player should also release resources when the activity is no longer alive.
* Use Exoplayer or MediaPlayer to play media

### Practicle 5
#### Implement SnapCam
* App should allows users to take pictures and save them to the device's gallery.
* Show captured image preview to user

### Practicle 6
#### Implement Note-taking application
* Allow users to input text in an EditText. 
* The application should have the ability to maintain the state of the EditText field, even when the device is rotated. 
* This means that when the user rotates the device, the EditText field should retain its previous contents, and the user should be able to continue editing the note without losing any data.

# Fragment

### Practicle 7
#### Develop Travel application
*  App should have a bottom bar with 3 tabs: Destinations, Search, and Settings. 
* The Destinations tab should display a list of popular travel destinations with images and descriptions. 
* The Search tab should Aalows the user to search for destinations
* The Settings tab should allow the user to customize app settings such as language and notification preferences.
* Use dummy data for destinations

### Practicle 8
#### Develop RecipeLister application
* Add RecyclerView to display the list of recipes.
* Each list item should show the recipe name and a short description.
* Tapping a recipe should open a new fragment with the full recipe text.
* The app should use a single Activity to manage the fragments.
* The up button should be used to navigate back to the list of recipes.

### Practicle 9
#### Implement App Browser
* The app will have an input field where the user can enter a URL and a button to initiate the process of opening the URL inside the app
* Once the user enters a valid URL and clicks the button, a new fragment will slide up from the bottom of the screen, displaying the content of the URL within a web view. 
* The fragment will also have a button to close it. 
* The state of the fragment should be preserved on configuration changes such as screen rotations.

# Intent

### Practicle 10
#### Develop QuickSend application
* Allow user to send emails by entering the receiver's email address and email content. 
* The application should have a screen that contains two edit text fields: one for the receiver's email address and one for the email content.
* The user should enter the email address and content and then click on the send button to send the emai.

### Practicle 11
#### Develop TalkEasy application
* Allow users to send and receive messages between two activities. 
* The first activity should have an edit text and a send button, and when the user enters a message and clicks on the send button, the message should be sent to the second activity.
* The second activity should have an edit text and a reply button, and when the user enters a reply message and clicks on the reply button, the replied message should be sent back to the first activity and displayed in a text view. 


# Android Jetpack Compose

### Practicle 12
#### Develop an interactive onboard screen for Fitness application
* App will provide a guided introduction to the app's features and functionality
* The onboard screen should include a welcome message and an introduction to the app's primary features, such as tracking workouts, setting goals, and accessing workout routines. 
* The onboard screen should provide step-by-step instructions for using these features and include interactive elements such as buttons or sliders that allow the user to interact with the onboard screen 
* Add option to skip the onboarding process for users who are already familiar with the app's features.
* Here's [UI for refrence](https://cdn.dribbble.com/users/2321513/screenshots/13623207/media/00046acbffbf953281b06b5bf4685dfd.mp4)

### Practicle 13

#### Develop MathQuest quiz application
* Ask 10 math questions for elementary school students
* The home screen should provide a introduction to the quiz and a button to start the quiz. 
* The quiz should ask 10 questions, one at a time, and provide four answer options for each question. 
* After the user answers all 10 questions, the app should display a result screen that shows the number of correct answers and the total number of questions. 
* The result screen should also provide a button to restart the quiz so that the user can play again.Implement day/night theme in Quiz app
* Here's [UI for refrence](https://cdn.dribbble.com/users/2469034/screenshots/8210470/media/f02da6249ee8c25f187432c73d4eec27.png)

### Practicle 14
#### Implement user profile UI
* Display a user's profile picture, name, and bio. 
* Use placeholder for profile image and dummy profile data.
* Here's [UI for refrence](https://cdn.dribbble.com/userupload/5207044/file/original-ceb3338a4a693f6ab102298dd3745716.jpg?compress=1&resize=1024x768)

# Networking

### Practicle 15

#### Develop ImageSaver application
* Allow users to download an image from a given URL, display the image on the screen, and store the downloaded image file in the device's internal storage. 
* The user should enter the URL of the image in an edit text field and click on the download button to initiate the download. 
* The progress of the download should be displayed using a progress bar. 
* Once the download is complete, the image should be displayed on the screen, and the downloaded image file should be stored in the device's internal storage
* Use Retrofit for networking

### Practicle 16

#### Implement OnlineUserDirectory
* Retrieve and display a simple users list from web API  
* Show users on main screen 
  - GET Api Url : http://jsonplaceholder.typicode.com/users
* On user item click to display all albums of selected user on next screen. 
  - GET Api Url : https://jsonplaceholder.typicode.com/albums?userId=1
* On the Album item click show all photos of the selected album on the next screen.
  - GET Api Url : http://jsonplaceholder.typicode.com/photos?albumId=2
* Use Retrofit for networking

# App Architecture

### Practicle 17

#### Implement Drink Explorer
* Allow users to search for their favourite mocktail detail. The application should have a search bar that allows users to search for mocktails by name. When the user taps on a mocktail, the application should display the ingredients and directions for making the mocktail. 
  - GET Api Url : https://www.thecocktaildb.com/api/json/v1/1/search.php?i={mocktail}
* The application should also have a "favourites" section where users can save their favourite mocktails for easy access.
* Save favourite mocktail detail in the database
* Use MVVM app architecture

### Practicle 18
#### Create My Journal application
* Enable users to document their daily thoughts, feelings, experiences, and ideas. 
* Add TextField to take user input
* The application should be able to persist data even when there is a configuration change, such as a screen rotation.
* Use ViewModel to save the view state

# DataStore

### Practicle 19
#### Develop Authentify
* An application that takes user credentials on the login screen and navigates to the home screen after a successful login.
* Once the user logs in, the app should always show the home screen until the user logs out.
* Add a button on the home screen to log out and clear the user session.
* When the user clicks the logout button, the app should clear the user session and navigate back to the login screen.

# Local Storage

### Practicle 20
#### Develop EmployeeHub application
* The application should display a list of employees on the home screen, including their name and job title. 
* When a user clicks on an employee from the list, the application should display their full details, such as their contact information, job responsibilities, and other important information. 
* The user should be able to add new employees to the directory by entering their basic information and saving it locally. 
* Additionally, the user should be able to update an employee's information by selecting them from the employee list and editing their details.
* Finally, the user should be able to delete an employee from the directory by selecting them from the employee list and deleting their details.
* Use Sqlite to store data locally

### Practicle 21
#### Implement MinionSpeak application
* Allow users to translate English text to the language of the minions and display the translated text on the screen.
* The user should enter the English text in an edit text field and click on the translate button to initiate the translation. Once the translation is complete, the translated text should be displayed on the screen in the language of the minions.
   - GET Request API with query parameter- “text” https://api.funtranslations.com/translate/minion.json?text=”banana”
* Additionally, the application should store the translation history locally so that users can access their previous translations.
* Add an option to delete  history.
* Use Room database

# Dependency Injection

### Practicle 22
#### Implement University directory application
* Allow users to browse and search universities from all around the world.
* The application should have a dropdown menu that allows users to select a country.
* When a country is selected, the application should display a list of universities located in that country.
* Use Hilt for dependency injection 
* GET Request API - http://universities.hipolabs.com/search?country={country name}

### Practicle 23
#### Implement offline-first StoreMate product application
* GET API - https://fakestoreapi.com/products
* Retrieve the list of products from an API and displays it to the user. 
* The application should also allow the user to view the full details of a product by clicking on it. 
* The application should have offline functionality, allowing the user to continue browsing products even when they do not have an internet connection.
* The product data should be first fetched from the local database and then sync with remote API data.
* Add swipe-to-delete functionality to remove products from local storage
* Add swipe-to-refresh functionality to refresh the local database with remote data

# Kotlin Coroutine & Flow

### Practicle 24
#### Implement count-down timer application using Kotlin coroutine. 
* The user should be able to set the duration of the timer and start it. 
* The timer should decrement every second, and the app should display the remaining time on the screen. 
* When the timer reaches zero, the app should display a notification to indicate that the time is up.

### Practicle 25
#### Implement a VocabVault app
* Allow users to search for the definition of any word in the English language.
* Users should be able to search for a word by typing it into a search bar, and the app should display the word's definition along with pronunciations, parts of speech, examples, synonyms.
* Use Kotlin coroutine
* API - https://api.dictionaryapi.dev/api/v2/entries/en/<word>

### Practicle 26
#### Create Contact Keeper application.
* Use Firestore to store contact details.
* The app should allow users to add, update, and delete contacts.
* The app should also update contacts in real-time, so changes made by one user are reflected across all devices.
* Use Kotlin  flow to get a real-time update

# Broadcast receiver & task scheduling

### Practicle 27
#### Create Stand Up! application 
* Remind users to stand up and walk around every fifteen minutes.
* The application should display a notification when fifteen minutes have passed since the last reminder.
* The app should have a toggle button that allows users to turn the alarm on and off.
* Use the Android AlarmManager to schedule reminder notifications.

# Android Service

### Practicle 18
#### Create Music player application
*  Allow users to play multiple songs. 
* Use an Android Service to play music in the background and show a notification of the current music being played.




 
