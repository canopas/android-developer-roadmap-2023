<h1 align="center">Android Developer Roadmap 2023</h1>

![alt text](https://github.com/cp-radhika-s/Android-Roadmap/blob/main/image/og_image.png)

The Android Developer Roadmap 2023 includes **29 practical exercises** that cover all the essential concepts used in day-to-day development.
# Guidelines

- Before starting any practical it's important to conduct research and learn the necessary concepts.

- As you progress through the practical exercises, make sure to apply the new knowledge you've gained in subsequent exercises. Try to allocate no more than 3-4 days to each practical.

- To keep track of your progress and share your work with your team lead, create a repository on GitLab where you can upload your completed exercises for review.

- To stay organized and track your progress, create tickets on ClickUp for each practical exercise. Each ticket should include a detailed description of the exercise, as well as an estimate of story points.

- As you work on each practical exercise, move the corresponding ticket from the "To-Do" queue to the "Done" queue to keep track of your progress. This will help you stay focused and motivated as you work through the roadmap.

- Follow android [material guideline](https://m2.material.io/design/guidelines-overview) for the best practices of user interface design
- Follow the [recommendations for Android architecture](https://developer.android.com/topic/architecture/recommendations)

# Table of contents
* [Useful references](https://github.com/canopas/android-developer-roadmap-2023#useful-references)
* [Android XML](https://github.com/canopas/android-developer-roadmap-2023#android-xml)
* [Android Activity](https://github.com/canopas/android-developer-roadmap-2023#android-activity)
* [Fragment](https://github.com/canopas/android-developer-roadmap-2023#fragment)
* [Intent](https://github.com/canopas/android-developer-roadmap-2023#intent)
* [Jetpack Compose](https://github.com/canopas/android-developer-roadmap-2023#jetpack-compose)
* [Networking](https://github.com/canopas/android-developer-roadmap-2023#networking)
* [App Architecture](https://github.com/canopas/android-developer-roadmap#app-architecture)
* [Datastore](https://github.com/canopas/android-developer-roadmap-2023#datastore)
* [Database](https://github.com/canopas/android-developer-roadmap-2023#local-storage)
* [Dependency Injection](https://github.com/canopas/android-developer-roadmap-2023#dependency-injection)
* [Kotlin Coroutine & Flow](https://github.com/canopas/android-developer-roadmap-2023#kotlin-coroutine--flow)
* [Broadcast Receiver](https://github.com/canopas/android-developer-roadmap-2023#broadcast-receiver--task-scheduling)
* [Android Service](https://github.com/canopas/android-developer-roadmap-2023#android-service)

## Useful references
The references provided are aimed at individuals who have no prior knowledge or experience in developing Android apps. They serve as a starting point for beginners in the field, providing basic knowledge that is necessary before diving into Android development. 
If you already have knowledge and experience in Android development, you may not need to refer to the provided resources. 
* [Develop your app's layout](https://developer.android.com/develop/ui/views/layout/declaring-layout)
* [Introduction to activities](https://developer.android.com/guide/components/activities/intro-activities)
  * [The activity lifecycle](https://developer.android.com/guide/components/activities/activity-lifecycle)
* [Jetpack compose](https://developer.android.com/jetpack/compose/tutorial)
* App Architecture
  * [Guide to app architecture](https://developer.android.com/topic/architecture)
  * [Best practices and recommended Architecture](https://developer.android.com/courses/pathways/android-architecture)
* Udemy courses - [Android App Development Masterclass](https://www.udemy.com/course/android-oreo-kotlin-app-masterclass/)
* [Version control Guideline](https://github.com/canopas/android-developer-roadmap-2023/blob/main/GitGuideline.md)
* [Kotlin style guide](https://developer.android.com/kotlin/style-guide)

# Android XML
### Practical 1

#### Develop UI for a Messaging application
* Implement an app using 3 Activities - Onboard, signIn and Home Activity
* On the onboard screen, show brief introduction to the app's features, such as messaging, voice and video calls, and file sharing.
  - Show images, titles and subtitles to introduce app functionality.
  - Add a button to check the next/previous features. Also, the skip button to skip the onboarding flow.
* On the sign-in screen, allow the user to enter their email and password, and add validation to ensure the user enters a valid email address and password.
  - Use dummy email/password to verify user input.
* After a successful login, the user should be redirected to the Home screen.
  - On the Home screen, show a list of chats with sender name, profile, latest message and message time.
  - The user should not be able to go back to the login screen once redirected to the Home screen.
  - Use dummy data for chats
  - Add toggle button on Home screen to change the day/night theme
* App should responsive for different resolutions.
* Add support for day/night theme.
* You can use any images or placeholder to make UI eye-catchy
* App should follow material guidelines
* Here's [UI for refrence](https://cdn.dribbble.com/userupload/3719280/file/original-5d6d206acf8adf5458091206369445f1.png?compress=1&resize=752x)

### Practical 2
#### Develop collapsing toolbar for the News application
* Home screen should show toolbar and news content
* The toolbar on screen should initially display the app's logo and title.
* As the user scrolls down to read news, the toolbar should collapse to provide more space for the content.
  - You can use any dummy text/images as article content.
* When the user reaches the end of the news and reverses scrolls, the toolbar should re-expand and display the app's logo & title
* You can use any images or placeholder to make UI eyecatchy
* App should follow material guidelines
* Here's [UI for reference](https://cdn.dribbble.com/users/663782/screenshots/3742414/media/67464fde751beb373b4c6fa962edf718.gif)

### Practical 3
#### Implement Survey application
* App will have one activity
* On the Home screen display a survey form
  - Survey form should show questions, 4 options and a button for next question.
  - Show progress as user answers the question
* Once the survey is completed, show a pop-up message thanking the user
  - Use the custom dialog to thank the user.
  - Dialog will have UI to show a thanks message, image and button to complete survey
* Asks at least 3 questions with 4 options each. 
* App should ask users about the shopping experience. 
* You can use any images or placeholder to make UI eye-catchy
* App should follow material guidelines
* Here's [UI for reference](https://cubicleninjas.com/wp-content/uploads/2021/01/NA-2021-Web-Questionnaire-3.jpg)

# Android Activity

### Practical 4
#### Implement Video player 
* This will be single Activity app
  - App should have a view to show Video
  - One button to play and pause video
* The player should follow the activity lifecycle, pause the player when the activity goes to the background and resume it when the activity returns to the foreground. 
* The player should also release resources when the app is no longer alive.
* An application can play a video from local resource. 
* Use Exoplayer or MediaPlayer to play media

### Practical 5
#### Implement SnapCam
* This will be Two Activity app 
* Home screen should have PreviewView to show camera
  - It should have button to capture image
  - Button to show captured image preview
  - Save button on Toolbar to save captured image to the device's gallery.
* On Preview Screen show image in fullscreen
  - Use Glide or coin for image preview
  - Add button to go back to camera screen
* The camera resources should be release when the activity is no longer alive.


### Practical 6
#### Implement Note-taking application
* Single activity app
  - Which allows the user to enter a note 
  - Use EditText to take input from the user.
  - Add a button to reset the note.
* The application should have the ability to maintain the state of the EditText field, even after the device is rotated. 
* This means that when the user rotates the device, the EditText field should retain its previous contents, and the user should be able to continue editing the note without losing any data.

# Fragment


### Practical 7
#### Develop a Travel application
* Implement the app using one activity only
* Home screen should have a bottom bar with 3 tabs: Destinations, Search, and Settings. 
* The Destinations tab should display a list of popular travel destinations with images and descriptions. 
* The Search tab should Allow the user to search for destinations
  - Add search view to search different destination
  - Show a message in TextView to notify the user when the searched destination is not available
  - Use dummy data for destinations
* The Settings tab should allow the user to customize app settings
  -  Add a toggle button for notification and day/night theme settings.
* App should preserve the state on tab change
  - If the user scrolled to the bottom of the destinations screen, it should preserve the scroll state across the tab change.
  - If a user searches for something on the search screen, the search result should be there when navigating to the search tab from other tabs.
  - If the user changed the setting's toggle, it should stay as it is when the user navigate between the tabs

### Practical 8
#### Develop RecipeLister application
* Single Activity app with two fragments - Home & detail fragment
* On the Home fragment add RecyclerView to display the list of recipes.
  - Each list item should show the recipe name and a short description.
  - Tapping a recipe should open Detail Fragment.
* On the Detail fragment show full recipe detail with recipe image and description
  - Add a back button to navigate back to the list of recipes.
* Use dummy data for recipes


### Practical 9
#### Implement App Browser
* Single Activity app with two fragments - Home & browser fragment
* On the Home fragment add an input field where the user can enter a URL and a button to open URL inside the app.
* Once the user enters a valid URL and clicks the button, slide up the Browser fragment from the bottom of the screen
  - This fragment will show the content of the URL within a web view. 
  - The fragment will also have a button to close it. 
  - Add a menu in the action bar, which will have two options- copy and share the link
    - Copy option should copy the link to the clipboard
    - The share option should allow users to share links in other applications
* The state of the fragment should be preserved on configuration changes such as screen rotation.

# Intent

### Practical 10
#### Develop QuickSend application
* This will be single Activity app - QuickSendActivity
* QuickSendActivity allows users to send emails
  - Add EditTextxs to input the receiver's email address and email content.
  - Add a button to send email
    - On click of it, the app should ask for the app to choose to send mail on. 

### Practical 11
#### Develop the TalkEasy application
* The app will send and receive messages between two activities. 
* The app will use two Activities - Sender & Receiver Activities.
* The Sender activity should have an edit text and a send button
  - When the user enters a message and clicks on the send button, open Receiver activity and show the message recieved from Sender Activity.
* The Receiver activity should have an edit text and a reply button
  - When the user enters a reply message and clicks on the reply button, the replied message should be sent back to the Sender activity and displayed in a text view. 


### Practical 12
#### Create Deep Links to App Content
* Implement an app that handles incoming link
* The app will use one Activity- Home Activity
* On Click of this link https://open.my.app?message={anymessage} from anywhere, the system should open Home Activity and show the message from a link
* Use intent filter in manifest to handle deep link

# Android Jetpack Compose

### Practical 13
#### Develop an interactive UI for the Fitness application
* App will provide a guided introduction to the app's features and functionality
* The app will use one Activity
* The onboard composable should include a welcome message and an introduction to the app's primary features, such as tracking workouts, setting goals, and accessing workout routines. 
  - The onboard screen should have interactive elements such as buttons or sliders that allow the user to interact with the onboard screen 
    - There should be next & previous buttons to go through features
    - Add an indicator to show pages
    - Add an option to skip the onboarding process.
* After onboard flow completion navigate user to the Home composable
  - Home composable should show basic tips & tricks related to fitness
  - Add option to log out, on logout show onboard view.
* Here's [UI for reference](https://cdn.dribbble.com/users/2321513/screenshots/13623207/media/00046acbffbf953281b06b5bf4685dfd.mp4)

### Practical 14
#### Develop MathQuest quiz application
* The app will have one quiz Activity
* The home composable should be an entry point of the app
  - This should provide an introduction to the quiz and a button to start the quiz. 
* The quiz should ask 10 questions, one at a time, and provide four answer options for each question. 
  - On click of the next button highlight the correct/wrong answer and show the next question
  - Show progress as the user answers the questions
* After the user answers all questions, the app should display a result view
  - Which shows the number of correct answers and the total number of questions. 
  - Show the excellence level based on the score such as poor, good and very good. 
  - Add a button to restart the quiz so that the user can play again.
* Implement  day/night theme in the Quiz app
* You can use images and placeholders to build eye-catchy UI
* Here's [UI for reference](https://cdn.dribbble.com/users/2469034/screenshots/8210470/media/f02da6249ee8c25f187432c73d4eec27.png)


### Practical 15
#### Implement user profile UI
* The app will use a one Activity
* Display a user's profile picture, name, and bio. 
* Use a placeholder for the image and  profile data.
* Add day/night theme support
* Here's [UI for reference](https://cdn.dribbble.com/userupload/5207044/file/original-ceb3338a4a693f6ab102298dd3745716.jpg?compress=1&resize=1024x768)

# Networking

### Practical 16
#### Develop ImageSaver application
* Allow users to download an image from a given URL, display the image on the screen, and store the downloaded image file in the device's internal storage. 
* The app will use a one Activity
  - Screen will have one Text field to enter the URL
  - Buttons to download images and cancel downloads
  - Show download progress in the progress bar
  - Show download progress in the notification
  - Show the downloaded image on full screen, once the download succeed
  - Add a button to save downloaded images in Gallery.
* Use Retrofit for networking


### Practical 17
#### Implement OnlineUserDirectory
* The app will use one Activity
  - Main composable should show list of users, retrieved from API.
  - Use LazyColumn to show users
  - Show summary of user in the list including name, image and email
  - GET Api Url : http://jsonplaceholder.typicode.com/users
* On the user item click, display all albums of user on the next screen. 
  - Use GridView to show albums
  - Show placeholder image for an album to make UI eye-catchy
  - GET Api Url : https://jsonplaceholder.typicode.com/albums?userId=1
* On the Album item click, show all photos of album on the next screen.
  - Use GridView to show photos
  - Show thumb image in Grid
  - Use glide or coil to show the image
  - On click of items show image in full screen
  - GET Api Url : http://jsonplaceholder.typicode.com/photos?albumId=2
* Use Retrofit for networking



# App Architecture

### Practical 18
#### Create My Journal application
* Enable users to Add their daily thoughts, feelings, experiences, and ideas. 
* The app will have a one Activity
  - Show user's thoughts in Grid
  - Add TextField to take user input
  - Add a button to save the user's thought
  - Store inputs in ViewModel as state
* User should be able to add multiple thoughts
* The application should be able to persist data even when there is a configuration change, such as screen rotation.
* Use MVVM app architecture


### Practical 19
#### Implement Drink Explorer
* Allow users to search for their favourite mocktail detail.
* The app will have one Activity
  - Add a search bar that allows users to search for mocktails by name
  - GET Api Url : https://www.thecocktaildb.com/api/json/v1/1/search.php?i={mocktail}
  - Default search text should be `mocktail`. That means initially showing `Mocktail` in the search bar and fetching `mocktail` using API
* When the user taps on a mocktail, the application should display the ingredients and detail of mocktail. 
  - Use placeholder and dummy data if required
* Use MVVM app architecture


# DataStore

### Practical 20
#### Develop Authentify
* An application that takes user credentials and basic information of a user and navigates to the home screen after a successful login.
* The app will have one Activity
  - First, the app will show the register form
    - Take the user's name, email and password for login
    - Other basic information such as an address, DOB, blood group and gender etc.
    - Add validation for email and password
    - Save user detail in DataStore
  - After registering, show a login form
    - Take email and password
    - Check whether the user is available or not. If the user does not exist, notify user to do registration
    - Add validation for email
* Once the user logs in, the app should always show the home screen
  - It will show user details
  - Add logout & delete user option in the toolbar
  - Clear user session on logout
  - Until the user logs out app should show the home screen.
  - When the user clicks the logout/delete user button, the app should clear/delete the user session and navigate back to the login screen.


# Local Storage

### Practical 21
#### Develop EmployeeHub application
* Build app using one activity
* The application should display a list of employees on the home screen 
  - Show basic details including their name and job title. 
* When a user clicks on an employee from the list, the application should display their full details
  - including their contact information, job title, and other important information. 
* The user should be able to add new employees to the directory by entering their basic information and saving it locally. 
  - Save employee name, email, contact info, job title, address, DOB and blood group etc.
* Additionally, the user should be able to update an employee's information by selecting them from the employee list and editing their details.
* Finally, an employee should be deleted by swiping to delete from the home screen
* Use SQLite to store data locally
* Use MVVM app architecture

### Practical 22
#### Implement MinionSpeak application
* Allow users to translate English text to the language of the minions and display the translated text on the screen.
* Build app using one activity
* On the Home screen
  - Add a text field to enter the English text.
  - Add a button to translate. On click of a button make an API call.
  - Once the translation is complete, the translated text should be displayed on the screen in the language of the minions.
  - GET Request API with query parameter- “text” https://api.funtranslations.com/translate/minion.json?text=”banana”
* Additionally, the application should store the translation history locally so that users can access their previous translations.
* Add fab button to check history on the home screen
* Add an option to delete the history
* Use Room database

# Dependency Injection

### Practical 23
#### Implement University directory application
* Allow users to browse and search universities from all around the world.
* On Home screen
  - Add a dropdown to select the country
  - When a country is selected, display a list of universities located in that country from API.
* Use Hilt for dependency injection 
* GET Request API - http://universities.hipolabs.com/search?country={country name}
* Write Unit test for viewModel


### Practical 24
#### Implement offline-first StoreMate product application
* GET API - https://fakestoreapi.com/products
* Build app using one activity
* On Home screen
  - Retrieve the list of products from an API and displays it to the user using LazyGrid. 
  - Show product name, image and button to favourite/unfavourite product
* Allow the user to view the product by clicking on it. 
  - Show all detail of the product
  - Add option to favourite/unfavourite the product
* Add an option on the home screen to view favourite products
  - Show all favourite products
  - Add option to remove from favourite
  - Add option to remove all favourite item
  - Use can select multiple items with a long click and can remove all selected products from their favourite.
* The application should have offline functionality, allowing the user to continue browsing products even when they do not have an internet connection.
* The product data should be first fetched from the local database and then sync with remote API data.
* Add swipe-to-delete functionality to remove products from local storage
* Add swipe-to-refresh functionality to refresh the local database with remote data
* Write Unit test for viewModel


# Kotlin Coroutine & Flow

### Practical 25
#### Implement count-down timer application using Kotlin coroutine. 
* Build app using one activity
* On Home screen
  - Add text fields to take user input for hours, minutes and second
  - Button to start/stop the timer
  - Show remaining & elapsed time 
* The user should be able to set the duration of the timer and start it. 
* When the timer ends, the app should display a notification to indicate that the time is up.
* Also play sound and vibrate device on timer completes
* Write Unit test for viewModel


### Practical 26
#### Implement a VocabVault app
* Allow users to search for the definition of any word in the English language.
* Build an app using one activity
* On the Home screen
  - Users should be able to search for a word by typing it into a search bar
  - App should display as user type in the search view
  - The app should display the word's definition along with pronunciations, parts of speech, examples, and synonyms.
  - Add option to play pronunciations of word
* Make sure the app will not make unnecessary API calls while typing in search view
  - Use debounce using Kotlin coroutine to avoid extra API calls
* Use Kotlin coroutine
* API - https://api.dictionaryapi.dev/api/v2/entries/en/<word>
* Write Unit test for viewModel

### Practical 27
#### Create a Contact Keeper application.
* Build an app using one activity
* On the Home screen
  - Show all Contacts on the home screen
    - Show name, phone number and profile
    - On click of contact show the contact profile
  - Add option to update contact detail
  - Add an option to delete a user by swiping to delete
  - Add option to add contact with person name, multiple phone numbers, profile image, blood group and address
* Add screen to edit/show contact detail
  - Add option to delete contact
* The app should also update contacts in real-time, so changes made by one user are reflected across all devices.
* Use Firestore to store contact details.
* Use Kotlin  flow to get a real-time update
* Write Unit test for viewmodel

# Broadcast receiver & task scheduling

### Practical 28
#### Create Stand Up! application 
* Remind users to stand up and walk around every fifteen minutes.
* Build an app using one activity
* On the Home screen
  - Add a Toggle button to turn alarm on and off
  - Add option to set reminder start time 
    - Open Timepicker to select reminder start time
* The application should display a notification when fifteen minutes have passed since the last reminder.
* Use the Android AlarmManager to schedule reminder notifications.


# Android Service

### Practical 29
#### Create a Music player application
*  Allow users to play multiple songs. 
* Build an app using one activity
* On the Home screen
  - Show a list of songs from the device
  - On click of the song  open player from the bottom
  - Show play indicator for current playing song
* On the Player screen
  - Show song thumb image if available or use placeholder
  - show song name
  - Add option to play/pause the song
  - Add options to play the next/previous song
  - Add options to forward/backwards song by 10 sec
* Use an Android Service to play music in the background and show a notification of the current music being played.
