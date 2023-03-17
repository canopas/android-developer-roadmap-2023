<h1 align="center">Android Developer Roadmap 2023</h1>

![alt text](https://github.com/cp-radhika-s/Android-Roadmap/blob/main/image/og_image.png)


The Android Developer Roadmap 2023 includes **29 practical exercises** that cover all the essential concepts used in day-to-day development.
# Guidelines

- Before starting any practical, it's important to conduct research and learn the necessary concepts.

- As you progress through the practical exercises, make sure to apply the new knowledge you've gained in subsequent exercises. Try to allocate no more than 3-4 days to each practical.

- To keep track of your progress and share your work with your team lead, create a repository on GitLab where you can upload your completed exercises for review.

- To stay organized and track your progress, create tickets on ClickUp for each practical exercise. Each ticket should include a detailed description of the exercise, as well as an estimate of story points.

- As you work on each practical exercise, move the corresponding ticket from the "To-Do" queue to the "Done" queue to keep track of your progress. This will help you stay focused and motivated as you work through the roadmap.

- Follow android [material guideline](https://m2.material.io/design/guidelines-overview) for the best practices of user interface design
- Follow the [recommendations for Android architecture](https://developer.android.com/topic/architecture/recommendations)

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
* App will have 3 Activities - Onboard, signIn and Home activity
* The onboard screen should provide a brief introduction to the app's features, such as messaging, voice and video calls, and file sharing.
  - Show images, title and subtitle to introduce app functionality.
  - Add button to check next/previous features. Also skip button to skip onboarding flow.
* The sign-in screen should allow the user to enter their email and password, and validation should be added to ensure the user enters a valid email address and password.
* After a successful login, the user should be redirected to the Home screen.
  - On Home screen should show list of chat which sender detail,latest message and message time.
  - The user should not be able to go back to the login screen once redirected to the Home screen.
* App should responsive for different resolutions.
* Add support for day/night theme.
* You can use any images or placeholder to make UI eyecatchy
* Add should follow material guildlines
* Here's [UI for refrence](https://cdn.dribbble.com/userupload/3719280/file/original-5d6d206acf8adf5458091206369445f1.png?compress=1&resize=752x)

### Practicle 2
#### Develop collapsing toolbar for News application
* App will have one activity
* The toolbar on screen should initially display the app's logo and title.
* As the user scrolls down to read an article, the toolbar should collapse to provide more space for the article.
  - You can use any dummy text/images as article content.
* When the user reaches the end of the article and reverse scrolls, the toolbar should re-expand and display the app's logo & title
* You can use any images or placeholder to make UI eyecatchy
* Add should follow material guildlines
* Here's [UI for refrence](https://cdn.dribbble.com/users/663782/screenshots/3742414/media/67464fde751beb373b4c6fa962edf718.gif)

### Practicle 3
#### Implement Survey application
* App will have one activity
* On Home screen display survey form
  - Survey form should show question, 4 options and button for next question.
  - Show progress as user answer the question
* Once the survey is completed, show a pop-up message thanking the user
  - Use custom dialog to thanks user.
  - Dialog will have UI to show thanks message, image and button to complete servey
* Asks at least 3 questions with 4 options each. 
* App should ask user about shopping experience. 
* You can use any images or placeholder to make UI eyecatchy
* Add should follow material guildlines
* Here's [UI for refrence](https://cubicleninjas.com/wp-content/uploads/2021/01/NA-2021-Web-Questionnaire-3.jpg)

# Android Activity

### Practicle 4
#### Implement Video player 
* This will be single Activity app
  - App should have a view to show Video
  - One button to play and pause vide
* The player should follow the activity lifecycle, pausing when the activity goes to the background and resuming when the activity returns to the foreground. 
* The player should also release resources when the activity is no longer alive.
* An application can play a video from local resource. 
* Use Exoplayer or MediaPlayer to play media

### Practicle 5
#### Implement SnapCam
* This will be Two Activity app - One to capture picture and another to show preview on image
  - Which has PreviewView to show camera
  - It should have button to capture image
  - Also button to show captured image preview
* On Preview Screen show image in fullscreen
  - Use Glide or coin for image preview
  - Add button to go back to camera screen
* Save capture image to the device's gallery.
* The camera resources should be release when the activity is no longer alive.

### Practicle 6
#### Implement Note-taking application
* A single activity app
  - Which allow user to enter a note 
  - Use EditText to take input from user.
  - Add button to reset the note
* The application should have the ability to maintain the state of the EditText field, even when the device is rotated. 
* This means that when the user rotates the device, the EditText field should retain its previous contents, and the user should be able to continue editing the note without losing any data.

# Fragment

### Practicle 7
#### Develop Travel application
* Implement app using one activity only
* Home screen should have bottom bar with 3 tabs: Destinations, Search, and Settings. 
* The Destinations tab should display a list of popular travel destinations with images and descriptions. 
* The Search tab should Aalows the user to search for destinations
  - Add search view to search different destination
  - Show message to notify user when searched destination is not available
* The Settings tab should allow the user to customize app settings
  -  Add toggle button for notification and day/night theme settings.
* App should preserve the state on tab change
  - If user scrolled to the bottom in destinations screen, it should preserve scroll state when tab change.
  - If user searched something on search screen, searched result should be there when navigate to seach tab from other tabs..
  - If user changed setting's toggle, it should be stay as it is when user navigate between the tabs
* Use dummy data for destinations

### Practicle 8
#### Develop RecipeLister application
* The app should use a single Activity to manage the fragments.
* App should have two fragments - Home & detail fragments
* On Home fragment add RecyclerView to display the list of recipes.
  - Each list item should show the recipe name and a short description.
  - Tapping a recipe should open Detail Fragment.
* On Detail fragment show full recipe detail with recipe image and description
  - Add back button to navigate back to the list of recipes.
* Use dummy data for recipes

### Practicle 9
#### Implement App Browser
* The app should use a single Activity to manage the fragments.
* App should have two fragments - Home & browser fragments
* On Home fragment add an input field where the user can enter a URL and a button to open url inside app.
* Once the user enters a valid URL and clicks the button, slide up Browser fragment from the bottom of the screen
  - This fragment will show the content of the URL within a web view. 
  - The fragment will also have a button to close it. 
  - Add a menu in action bar, which will have two option- copy and share the link
    - Copy option should copy the link to the clipboard
    - Share option should allow user to share link in other application
* The state of the fragment should be preserved on configuration changes such as screen rotations.

# Intent

### Practicle 10
#### Develop QuickSend application
* This will be single Activity app - QuickSendActivity
* QuickSendActivity allow user to send emails
  - Add EditTextxs to input the receiver's email address and email content.
  - Add button to send email
    - On click of it, app should ask for app to choose to send mail on. 

### Practicle 11
#### Develop TalkEasy application
* Allow users to send and receive messages between two activities. 
* The app will use a two Activity- Sender & Receiver Activity.
* The Sender activity should have an edit text and a send button
  - When user enters a message and clicks on the send button, the message should be sent to the Receiver activity.
* The Receiver activity should have an edit text and a reply button
  - When the user enters a reply message and clicks on the reply button, the replied message should be sent back to the Sender activity and displayed in a text view. 

### Practicle 12
#### Create Deep Links to App Content
* Implement app that handle incoming link
* The app will use a one Activity- Home Activity
* On Click of this link https://open.my.app?message={anymessage} from anywhere, system should open Home Activity and show the message from link
* Use intent-filter in manifest to handle deep link

# Android Jetpack Compose

### Practicle 13
#### Develop an interactive onboard screen for Fitness application
* App will provide a guided introduction to the app's features and functionality
* The app will use a one Activity- onboard Activity
* The onboard composable should include a welcome message and an introduction to the app's primary features, such as tracking workouts, setting goals, and accessing workout routines. 
  - The onboard screen should have interactive elements such as buttons or sliders that allow the user to interact with the onboard screen 
    - There should be next & previous button to go through features
    - Add indicator to show pages
    - Add option to skip the onboarding process.
* After onboard flow completion navigate user to Home composable
  - Home composable should show basic tips & tricks related to fitness
  - Add option to logout, on logout show onboard view.
* Here's [UI for refrence](https://cdn.dribbble.com/users/2321513/screenshots/13623207/media/00046acbffbf953281b06b5bf4685dfd.mp4)

### Practicle 14

#### Develop MathQuest quiz application
* The app will use a one Activity- quiz Activity
* The home composable should be entry point of app
  - Which should provide a introduction to the quiz and a button to start the quiz. 
* The quiz should ask 10 questions, one at a time, and provide four answer options for each question. 
  - On click of next button highlight the correct/wrong answer and show next question
  - Show progress as user answer the questions
* After the user answers all 10 questions, the app should display a result view
  - Which shows the number of correct answers and the total number of questions. 
  - Show the excellence level based on the score such as poor, good and very good. 
  - Add a button to restart the quiz so that the user can play again.
* Implement day/night theme in Quiz app
* You can use images and placeholder to build eye-catchy UI
* Here's [UI for refrence](https://cdn.dribbble.com/users/2469034/screenshots/8210470/media/f02da6249ee8c25f187432c73d4eec27.png)

### Practicle 15
#### Implement user profile UI
* The app will use a one Activity
* Display a user's profile picture, name, and bio. 
* Use placeholder for profile image and dummy profile data.
* Add day/night theme support
* Here's [UI for refrence](https://cdn.dribbble.com/userupload/5207044/file/original-ceb3338a4a693f6ab102298dd3745716.jpg?compress=1&resize=1024x768)


# Networking

### Practicle 16

#### Develop ImageSaver application
* Allow users to download an image from a given URL, display the image on the screen, and store the downloaded image file in the device's internal storage. 
* The app will use a one Activity
  - Screen will have one Text field to enter URL
  - Buttons to download image and cancel downloads
  - Show download progress in progress bar
  - Show download progress in notification
  - Show downloaded image on full screen, once download succeed
  - Add button to save downloaded image in Gallery.
* Use Retrofit for networking

### Practicle 17

#### Implement OnlineUserDirectory
* The app will use a one Activity
  - Main composable should show list of users retrived from API.
  - Use LazyColumn to show user
  - Show summary of user in list including name, image and email
  - GET Api Url : http://jsonplaceholder.typicode.com/users
* On user item click to display all albums of selected user on next screen. 
  - Use GridView to show albums
  - Show placeholder image for album to make UI eyecatchy
  - GET Api Url : https://jsonplaceholder.typicode.com/albums?userId=1
* On the Album item click show all photos of the selected album on the next screen.
  - Use GridView to show photos
  - Show thumb image in Grid
  - Use glide or coil to show image
  - On click of items show image in full screen
  - GET Api Url : http://jsonplaceholder.typicode.com/photos?albumId=2
* Use Retrofit for networking

# App Architecture

### Practicle 18
#### Create My Journal application
* Enable users to document their daily thoughts, feelings, experiences, and ideas. 
* The app will have a one Activity
  - Show user's thoughts in Grid
  - Add TextField to take user input
  - Add button to save user's thought
  - Store inputs in Viewmodel as state
* User should be able to add multiple thoughts
* The application should be able to persist data even when there is a configuration change, such as a screen rotation.
* Use MVVM app architecture


### Practicle 19
#### Implement Drink Explorer
* Allow users to search for their favourite mocktail detail.
* The app will have a one Activity
  - Add search bar that allows users to search for mocktails by name
  - GET Api Url : https://www.thecocktaildb.com/api/json/v1/1/search.php?i={mocktail}
  - Default search text should be `mocktail`. That means initialy show `Mocktail` in search bar and fetch `mocktail` using API
* When the user taps on a mocktail, the application should display the ingredients and directions for making the mocktail. 
  - Use place holder and dummy data if required
* Use MVVM app architecture



# DataStore

### Practicle 20
#### Develop Authentify
* An application that takes user credentials and basic information of user and navigates to the home screen after a successful login.
* The app will have a one Activity
  - First app should show register form
    - Take user's name, email and password for login
    - Other basic information such as address, DOB, blood group and gender etc.
    - Add validation for email and password
    - Save user detail in DataStore
  - After register, show login form
    - Take email and password
    - Check the user is available or not. If user not exist, notify use to do registration
    - Add validation for email
* Once the user logs in, the app should always show the home screen
  - It will show user details
  - Add logout & delete user option in toolbar
  - Clear user session on logout
  - Until the user logs out app should show home screen.
  - When the user clicks the logout/delete user button, the app should clear/delete the user session and navigate back to the login screen.

# Local Storage

### Practicle 21
#### Develop EmployeeHub application
* The app will have a one Activity
* The application should display a list of employees on the home screen 
  - Show basic details including their name and job title. 
* When a user clicks on an employee from the list, the application should display their full details
  - including their contact information, job title, and other important information. 
* The user should be able to add new employees to the directory by entering their basic information and saving it locally. 
  - Save employee name, email, contact info, job title, address, DOB and blood group etc.
* Additionally, the user should be able to update an employee's information by selecting them from the employee list and editing their details.
* Finally, employee should be delete by swipe to delete from home screen
* Use Sqlite to store data locally
* Use MVVM app architecture

### Practicle 22
#### Implement MinionSpeak application
* The app will have a one Activity
* Allow users to translate English text to the language of the minions and display the translated text on the screen.
* On Home screen
  - Add text field tpenter the English text.
  - Add button to translate. On click of button make API call.
  - Once the translation is complete, the translated text should be displayed on the screen in the language of the minions.
  - GET Request API with query parameter- “text” https://api.funtranslations.com/translate/minion.json?text=”banana”
* Additionally, the application should store the translation history locally so that users can access their previous translations.
* Add fab button to check history on home screen
* Add an option to delete  history
* Use Room database

# Dependency Injection

### Practicle 23
#### Implement University directory application
* Allow users to browse and search universities from all around the world.
* The app will have a one Activity
  - Add dropdown to select the country
  - When a country is selected, display a list of universities located in that country from API.
* Use Hilt for dependency injection 
* GET Request API - http://universities.hipolabs.com/search?country={country name}
* Write Unit test for viewmodel

### Practicle 24
#### Implement offline-first StoreMate product application
* GET API - https://fakestoreapi.com/products
* The app will have a one Activity
  - Retrieve the list of products from an API and displays it to the user using LazyGrid. 
  - Show product name, image and button to favourite/unfavourite product
* Allow the user to view the product by clicking on it. 
  - Show all detail of product
  - Add option to favourite/unfavourite the product
* Add option on home screen to view favoutie products
  - Show all favourite products
  - Add option to remove from favourite
  - Add option to remove all favourite item
  - Use can select multiple item on long click and can remove all selected products from favourite.
* The application should have offline functionality, allowing the user to continue browsing products even when they do not have an internet connection.
* The product data should be first fetched from the local database and then sync with remote API data.
* Add swipe-to-delete functionality to remove products from local storage
* Add swipe-to-refresh functionality to refresh the local database with remote data
* Write Unit test for viewmodel

# Kotlin Coroutine & Flow

### Practicle 25
#### Implement count-down timer application using Kotlin coroutine. 
* The app will have a one Activity
  - Add textfields to take user input for hour, minute and second
  - Button to start/stop the timer
  - Show remining & elapsed time 
* The user should be able to set the duration of the timer and start it. 
* When the timer ends, the app should display a notification to indicate that the time is up.
* Also play sound and vibrate device on timer completes
* Write Unit test for viewmodel

### Practicle 26
#### Implement a VocabVault app
* Allow users to search for the definition of any word in the English language.
* The app will have a one Activity
  - Users should be able to search for a word by typing it into a search bar
  - App should display as user type in search view
  - The app should display the word's definition along with pronunciations, parts of speech, examples, synonyms.
  - Add option to play pronounciations of word
* Make sure app will not make unneccessary API calls while typing in searchview
  - Use debounce using kotlin coroutine to avoid extra API calls
* Use Kotlin coroutine
* API - https://api.dictionaryapi.dev/api/v2/entries/en/<word>
* Write Unit test for viewmodel

### Practicle 27
#### Create Contact Keeper application.
* The app will have a one Activity
  - Add option to add contact with person name, multiple phone numbers, profile image, blood group and address
  - Show all contancts on home screen
    - Show name, phone number and profile
    - On click of contact show contact profile
  - Add option to update contact detail
  - Add option to delete user by swipe to delete
* Add screen to edit/show contact detail
  - Add option to delete contact
* The app should also update contacts in real-time, so changes made by one user are reflected across all devices.
* Use Firestore to store contact details.
* Use Kotlin  flow to get a real-time update
* Write Unit test for viewmodel

# Broadcast receiver & task scheduling

### Practicle 28
#### Create Stand Up! application 
* Remind users to stand up and walk around every fifteen minutes.
* The app will have a one Activity
  - Add Toggle button to turn alarm on and off
  - Add option to set reminder start time 
    - Open Timepicker to select reminder start time
* The application should display a notification when fifteen minutes have passed since the last reminder.
* Use the Android AlarmManager to schedule reminder notifications.

# Android Service

### Practicle 29
#### Create Music player application
*  Allow users to play multiple songs. 
* The app will have a one Activity
  - Show list of songs from device
  - On click of song, open player from bottom
  - Show play indicator for current playing song
* On Player screen
  - Show song thumb image if available or use placeholder
  - show song name
  - Add option to play/pause song
  - Add options to play next/prevous song
  - Add options to forward/backword song by 10 sec
* Use an Android Service to play music in the background and show a notification of the current music being played.
