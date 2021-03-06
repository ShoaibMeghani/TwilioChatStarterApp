# Android ChatLib
ChatLib is a helper library to add chat functionality in Android app. The library provides all features that are essential in developing chat module in an application.

### Background
In recent past, I came across many clients who wanted to have chat like feature in their apps. The goal was to develop a helper library that allows following:
- A library that can be quickly added for chat based requirement (plug and play)
- Easy to understand code and seamless integration
- Enable integration with third party chat frameworks without changing much code
- Ensure extensibility

### What it includes?
The library has follwing items that are required in any chat module:
  - Chat Bubbles
  - General screen for chat list and messages
  - Support for textual chat and media (images).
  - Chat list sorting based on recent time

### Usage
##### Chat List screen
In order to add chat list screen to your app extend your fragment with `ChatListBaseFragment` and override methods to provide your own customised views/implementaiton.
  - Return layout resource id of your fragment in `getChatLayoutResource()`.
  - To show chat list in listview, return listview id in `getListviewId()`
  - You can also provide custom implementation of chat list adapter by extending your adapter with `ChatListBaseAdap`

##### Chat Conversation screen
To add message screen to your app extend your fragment with `ChatBaseFragment` and overried methods to provide customised implementation.
  - Return layout resource id of your fragment in `getChatLayoutResource()`
  - Message screen uses recycler view to show messages. Pass recycler view id in `getRecyclerViewId()`
  - Extend your message adapter with `MessageListBaseAdap` for basic message list implementation.

### Todo
 - Allowing customization using a config file instead of overriding whole adapters and methods.




