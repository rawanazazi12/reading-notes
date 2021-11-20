# Read: 41 - Intent Filters


## Allowing Other Apps to Start Your Activity 

- If your app can perform an action that might be useful from another app, your app should be prepared to respond to action requests by specifying the appropriate intent filter in your activity.

- To allow other apps to start your activity in this way, you need to add an <intent-filter> element in your manifest file for the corresponding <activity> element.

## Add an Intent Filter

- In order to properly define which intents your activity can handle, each intent filter you add should be as specific as possible in terms of the type of action and data the activity accepts.

- The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the Intent object:

    1. Action : A string naming the action to perform. Usually one of the platform-defined values such as ACTION_SEND or ACTION_VIEW.

    2. Data :  A description of the data associated with the intent. Specify this in your intent filter with the <data> element.


    3. Category : Provides an additional way to characterize the activity handling the intent, usually related to the user gesture or location from which it's started. 


## Handle the Intent in Your Activity
  
- In order to decide what action to take in your activity, you can read the Intent that was used to start it.

- As your activity starts, call getIntent() to retrieve the Intent that started the activity. You can do so at any time during the lifecycle of the activity, but you should generally do so during early callbacks such as onCreate() or onStart().


## Return a Result

- If you want to return a result to the activity that invoked yours, simply call setResult() to specify the result code and result Intent.

- If you simply need to return an integer that indicates one of several result options, you can set the result code to any value higher than 0. If you use the result code to deliver an integer and you have no need to include the Intent, you can call setResult() and pass only a result code. 