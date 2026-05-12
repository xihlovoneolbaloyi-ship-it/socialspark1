
# Social Spark App

## Overview

Social Spark is a native Android application developed using Kotlin in Android Studio.

The app helps users maintain meaningful social interactions during busy days by suggesting simple social “sparks” based on the time of day entered by the user.

The application was designed for simplicity, usability, and engagement while demonstrating Android development concepts such as conditional logic, error handling, logging, version control, and GitHub Actions automation.

---

# Features

## User Input

Users can enter a time of day such as:

* Morning
* Mid-morning
* Afternoon
* Afternoon Snack Time
* Dinner
* Night


## Social Suggestions

The application displays social interaction suggestions based on the entered time.

### Example Suggestions

| Time of Day          | Suggestion                                        |
| -------------------- | ------------------------------------------------- |
| Morning              | Send a “Good Morning” text to a family member     |
| Mid-morning          | Reach out to a colleague with a quick “Thank You” |
| Afternoon            | Share a funny meme or interesting link            |
| Afternoon Snack Time | Send a “Thinking of You” message                  |
| Dinner               | Call a friend or relative                         |
| Night                | Leave a thoughtful comment on a friend’s post     |



## Reset Functionality

The Reset button:

* Clears the text input
* Clears the displayed suggestion



## Error Handling

The application validates user input and displays motivational error messages when invalid information is entered.

Example:

```text
Please enter a valid time of day such as Morning or Dinner.
```


# Technologies Used

| Technology     | Purpose                 |
| -------------- | ----------------------- |
| Kotlin         | App development         |
| Android Studio | IDE                     |
| GitHub         | Version control         |
| GitHub Actions | Automated build testing |

---

# User Interface Design

The app was designed with:

* Large readable text
* Simple navigation
* User-friendly layout
* Attractive colours
* Responsive controls

The interface is clean and easy to use for all users.


# Application Logic

The app uses Kotlin `if` and `else-if` statements to:

* Compare user input
* Determine the correct social spark suggestion
* Display the result dynamically

Example:

```kotlin
if (userInput == "morning") {
    resultText.text = "Send a Good Morning text to a family member"
}
```



# Logging

The application uses Logcat logging for debugging and testing.

### Logging Implemented

```kotlin
Log.d()
Log.i()
Log.w()
```

### Purpose of Logging

* Track button clicks
* Monitor user input
* Display debugging information
* Assist during testing



# GitHub Version Control

The project was uploaded to [GitHub](https://github.com?utm_source=chatgpt.com) for:

* Version control
* Backup
* Progress tracking
* Collaboration readiness

Regular commits were made throughout development.



# GitHub Actions

This project uses GitHub Actions for automated building.

Whenever code is pushed to the repository:

* The project automatically builds
* The workflow checks for errors
* Build reliability is improved



# GitHub Actions Workflow

File location:

```text
.github/workflows/build.yml
```

Example workflow:

```yaml
name: Android Build

on:
  push:
    branches: [ main ]

jobs:
  build:

    runs-on: ubuntu-latest

    steps:
      - name: Checkout Repository
        uses: actions/checkout@v4

      - name: Set Up JDK
        uses: actions/setup-java@v4
        with:
          distribution: 'temurin'
          java-version: '17'

      - name: Grant Execute Permission
        run: chmod +x gradlew

      - name: Build Project
        run: ./gradlew build


# Testing

Manual testing was conducted to verify:

* Correct suggestions
* Error handling
* Reset functionality
* Application stability
* User interface responsiveness


# Installation

## Requirements

* Android Studio
* Android SDK
* Kotlin support



## Steps to Run

1. Clone the repository
2. Open the project in Android Studio
3. Allow Gradle to sync
4. Run the application on an emulator or Android device



# Learning Outcomes

This project improved understanding of:

* Kotlin programming
* Android Studio
* Conditional statements
* Error handling
* Logging
* GitHub version control
* GitHub Actions automation

---

# Author

## Developed By
st10536956
neol baloyi

---

# Conclusion

The Social Spark application successfully demonstrates native Android development using Kotlin while providing users with engaging and meaningful social interaction suggestions based on the time of day.
# SOCIALSPARK
