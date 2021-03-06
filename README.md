# REDDIT VIEWER

Reddit Viewer is a cross-platform React Native App for Android and iOS that fetches posts from Reddit and displays information about each post. Tabs allow the user to fetch posts from hot, new, rising, controversial and top. Clicking a post takes the user to a 'Post Details' page which shows basic information about the post.

![IndexScene](./RedditViewer/app/images/postIndex.png) ![DetailScene](./RedditViewer/app/images/postDetails.png)

##TESTING INSTRUCTIONS

- Make sure you've followed the React Native
[setup instructions](https://facebook.github.io/react-native/docs/getting-started.html) provided by our friends at Facebook.
- Clone this repo to your machine
- Navigate to RedditViewer in terminal and run `npm install`
- (Android Studio)
    - Open the RedditViewer folder with Android Studio.
    - Check the event log. If prompted, __Add Root__ and also __Configure__ your Android framework.
    - Start an emulator.
    - in your terminal run `react-native start`
    - in your terminal run `react-native run-android`
- (XCode)
    - In your terminal enter `react-native run-ios`.
- NOTE: If the emulator's time drifts more than a minute, changing the emulators time to the current time using the emulator's UI should fix that. The PostDetail component will not render if your emulator's time is wrong.

##FEATURES
  - Cross-platform Android/iOS
  - Caches the redux store to the phones storage using `redux-persist`

##TECHNOLOGIES

- React Native
- Redux

##FUTURE DIRECTION

Currently this app only displays a thumbnail on the post details page. I also added support for gif playback on Android, but loading is slow. Eventually I'd like to improve the details page to handle virtually all types of media so that things like video and articles display properly. 
