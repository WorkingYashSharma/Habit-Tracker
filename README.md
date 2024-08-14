<h1 align="center" id="title">Habit Tracker</h1>

<p id="description">Achieve your goals and build positive habits with ease using our Habit Tracker app. Designed to help you stay motivated and organized our app allows you to set monitor and review your daily habits and routines. With intuitive tracking customizable reminders and insightful analytics you'll be empowered to make lasting changes and reach your personal milestones. Start your journey to a better you today!</p>

<h2>🚀 Demo</h2>

[https://drive.google.com/file/d/1g9TqJa1O5\_g9tLw0p5Zj-BPAxGsi2-pg/view?usp=sharing](https://drive.google.com/file/d/1g9TqJa1O5_g9tLw0p5Zj-BPAxGsi2-pg/view?usp=sharing)
[https://github.com/WorkingYashSharma/Habit-Tracker/blob/main/app-release.apk](https://github.com/WorkingYashSharma/Habit-Tracker/blob/main/app-release.apk)


  
  
<h2>🧐 Features</h2>

Here're some of the project's best features:

*   Login and Registration functionalities were implemented using the Firebase Authentication API. The app handles API responses related to incorrect passwords invalid emails weak passwords network errors etc.
*   Implemented Auto-Login. The user doesn't need to authenticate everytime the app is restarted. Their authentication state is checked everytime the app is opened and they are auto-logged in depending on the AuthState.
*   The user can sign out of his account from the Profile page of the app.
*   A habit can simply be created by clicking the plus button filling in the Habit name and the number of Days the user wishes to take up that habit(Goal Days).
*   Every habit must have a unique name and unique colour. The app wouldn't allow the user to create a habit with the same name and colour.
*   The user can select the check box linked with every habit to mark its completion for the day. The checkbox resets every single day.
*   Any habit can be deleted by simply clicking the bin icon.
*   Every Habit is tappable and supports two types of tap gestures:
*   Single Tap: The user can now view every metric associated with each habit.
*   Success Rate: Measures how deligently the user completes his habits. Progress Rate: Measures how far in the user is towards his goal. Streaks: The calendar highlights all the streaks completed by the user. The habit's Current and Best Streaks are also mentioned along with their start dates.
*   Long Press: The user can quickly glance through the most important metrics of any habit its Success Rate and Progreess Rate.
*   The app keeps track of the 'Goal Days' for every ongoing habit and moves them to the Completed Habit Section after the stipulated time. On selecting Stats from the bottom navigation bar the combined stats of all habits can be viewed in the form of concentric rings horizontal bar charts and tables.
*   After every Habit is completed it is moved to the Completed Habits section in the Profile page. The stats of the completed habits can also be viewed.
*   Everytime the user signs into his account data is loaded from Realtime Firebase Database into Hive. Any further addition or deletion of Habits are updated locally only in hive and not on Firebase. On signing out of the account all the data from Hive is backed up to Firebase and the local storage (Hive) is cleared. Clearing Hive prevents the leakage of the prior users data into the account of the newly logged in user from the same device. Accessing Firebase only once during login to retrieve data and then switching to Hive for all other operations improves performance.

<h2>🛠️ Installation Steps:</h2>

<p>1. Clone the repository by running the following command in your terminal</p>

```
git clone https://github.com/WorkingYashSharma/Habit-Tracker.git
```

<p>2. Go to Firebase and make a new project and add it's package name</p>

<p>3. Add Firebase Database and in Firebase Auth enable Email/Pass Auth</p>

<p>4. Now place google-services.json file in android/app</p>

<p>5. Get the packages</p>

```
flutter pub get
```

<p>6. Run the app</p>

```
flutter run
```

  
  
<h2>💻 Built with</h2>

Technologies used in the project:

*   Flutter
*   Firebase Database
*   Firebase Auth
*   Hive
