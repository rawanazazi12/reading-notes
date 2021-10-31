# Android Tasks and the Back Stack

1. A task is a collection of activities that users interact with when trying to do something in your app. 

2. These activities are arranged in a stack—the back stack—in the order in which each activity is opened.

3. When the user selects a message, a new activity opens to view that message. This new activity is added to the back stack. 


## Lifecycle of a task and its back stack

4. The device Home screen is the starting place for most tasks. When a user touches the icon for an app or shortcut in the app launcher (or on the Home screen), that app's task comes to the foreground.

5. When the current activity starts another, the new activity is pushed on the top of the stack and takes focus. The previous activity remains in the stack, but is stopped.

6. When an activity stops, the system retains the current state of its user interface. When the user performs the back action, the current activity is popped from the top of the stack (the activity is destroyed) and the previous activity resumes (the previous state of its UI is restored).

7. Activities in the stack are never rearranged, only pushed and popped from the stack—pushed onto the stack when started by the current activity and popped off when the user leaves it using the Back button or gesture.

8. A representation of how each new activity in a task adds an item to the back stack. When the user presses or gestures Back, the current activity is destroyed and the previous activity resumes.

![img](https://developer.android.com/images/fundamentals/diagram_backstack.png)


## Back press behavior for root launcher activities
Root launcher activities are activities that declare an Intent filter with both ACTION_MAIN and CATEGORY_LAUNCHER. These activities are unique because they act as entry points into your app from the app launcher and are used to start a task.


## Background and foreground tasks

A task is a cohesive unit that can move to the background when a user begins a new task or goes to the Home screen.


## Multiple activity instances

Because the activities in the back stack are never rearranged, if your app allows users to start a particular activity from more than one activity, a new instance of that activity is created and pushed onto the stack 


## Android SharedPreferences

If you have a relatively small collection of key-values that you'd like to save, you should use the SharedPreferences APIs. A SharedPreferences object points to a file containing key-value pairs and provides simple methods to read and write them. Each SharedPreferences file is managed by the framework and can be private or shared.


### Get a handle to shared preferences

You can create a new shared preference file or access an existing one by calling one of these methods:

- getSharedPreferences() — Use this if you need multiple shared preference files identified by name, which you specify with the first parameter. You can call this from any Context in your app.
- getPreferences() — Use this from an Activity if you need to use only one shared preference file for the activity. Because this retrieves a default shared preference file that belongs to the activity, you don't need to supply a name.

- For example, the following code accesses the shared preferences file that's identified by the resource string R.string.preference_file_key and opens it using the private mode so the file is accessible by only your app:

        Context context = getActivity();
        SharedPreferences sharedPref = context.getSharedPreferences(
        getString(R.string.preference_file_key), Context.MODE_PRIVATE); 


- When naming your shared preference files, you should use a name that's uniquely identifiable to your app. An easy way to do this is prefix the file name with your application ID. For example: "com.example.myapp.PREFERENCE_FILE_KEY"


### Write to shared preferences

- To write to a shared preferences file, create a SharedPreferences.Editor by calling edit() on your SharedPreferences.

- Pass the keys and values you want to write with methods such as putInt() and putString(). Then call apply() or commit() to save the changes

- apply() changes the in-memory SharedPreferences object immediately but writes the updates to disk asynchronously. Alternatively, you can use commit() to write the data to disk synchronously. But because commit() is synchronous, you should avoid calling it from your main thread because it could pause your UI rendering.

### Read from shared preferences

To retrieve values from a shared preferences file, call methods such as getInt() and getString(), providing the key for the value you want, and optionally a default value to return if the key isn't present.