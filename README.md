This repository is meant to contain logs and references to the assignment work that I've done for [Centauri React Native Cohort by Real Dev Squad](https://github.com/Real-Dev-Squad/Centauri-React-Native-Cohort).

Projects
- [Tweeter](https://github.com/lyqht/centauri-tweeter): Exercises 1-3
  - [Snack](https://snack.expo.dev/@lyqht/tweeter)
- [Sencha Teahouse](https://github.com/lyqht/sencha-teahouse): Exercises 4
  - [Snack](https://snack.expo.dev/@lyqht/sencha-teahouse-v2)

Exercises
- [Exercise 1: Characters Remaining](#exercise-1-characters-remaining)
  - [Task](#task)
  - [Demo](#demo)
  - [Lessons Learnt](#lessons-learnt)
- [Exercise 2: Navigation](#exercise-2-navigation)
  - [Task](#task-1)
  - [Demo](#demo-1)
  - [Lessons Learnt](#lessons-learnt-1)
- [Exercise 3: Swipeable](#exercise-3-swipeable)
  - [Task](#task-2)
  - [Demo](#demo-2)
  - [Lessons Learnt](#lessons-learnt-2)
- [Exercise 4: Cart](#exercise-4-cart)
  - [Task](#task-3)
  - [Thinking Process](#thinking-process)
  - [Demo](#demo-3)
  - [Lessons Learnt](#lessons-learnt-3)


---

## Exercise 1: Characters Remaining

### Task

> Source of instructions can be found [here](https://github.com/Real-Dev-Squad/Centauri-React-Native-Cohort/blob/main/react-native/action-items/2022-01/2022-01-04.md). 

Create a simple textbox that displays how many characters are remaining in the "tweet" to send out (Tweets are 280 characters).

If the characters remaining are equal or more than 10, make the info text light gray. If the characters remaining are less than 10, make it Yellow. If you exceed the character limit, make the details Red.

### Demo

https://user-images.githubusercontent.com/35736525/148542454-e93cc50b-ade2-449b-883b-7c17cd0db115.mp4

### Lessons Learnt
- This was pretty simple to do since I had React knowledge.
- I find it interesting how the TextInput component still keeps the bold formatting that I copied elsewhere 😃

## Exercise 2: Navigation

### Task

> Source of instructions can be found [here](https://github.com/Real-Dev-Squad/Centauri-React-Native-Cohort/blob/main/react-native/action-items/2022-01/2022-01-13.md).

Implement a simple 2-screen app, where you have button "Go to details screen", clicking which takes you to the "details" screen and hitting "back" takes you back to the first screen.


### Demo

https://user-images.githubusercontent.com/35736525/149714329-1018b6ba-7dc3-47fb-96a8-3a82c79a0e0f.mp4

### Lessons Learnt

Some extra things I tried and learnt about:
- Local storage using [React Native Async Storage](https://github.com/react-native-async-storage/async-storage). The `useAsyncStorage` hook is really easy to use.
- [Flipper](https://github.com/facebook/flipper) for debugging and [Flipper Advanced Async Storage Plugin](https://github.com/lbaldy/flipper-plugin-async-storage-advanced) for CRUD actions on local storage.
- State management using React context still works as intended on React Native.

## Exercise 3: Swipeable

### Task

> Source of instructions can be found [here](https://github.com/Real-Dev-Squad/Centauri-React-Native-Cohort/blob/main/react-native/action-items/2022-01/2022-01-15.md).

Upon rendering a list of emails in an inbox, swipe left to delete an email from the list.

**Additional Task**
How can you add an "Undo" feature?


### Demo

https://user-images.githubusercontent.com/35736525/149978363-8b2c1ee8-ee81-45f8-a8aa-4706a5ed11ba.mp4

### Lessons Learnt

- Learnt how to use Native Base library components e.g. Box, Button, Pressable, Toast.
- The Swipeable component involves having to think about how to render the component that is shown after swiping the list item. 
- Learnt how to use React Native Gesture Handler Library's Swipeable API.

Ideally, I would want to replicate how Grab does the "undo order" UX with a proper countdown. 

## Exercise 4: Cart

### Task

Create the two screens with the little information you can understand from these screens. (Missing Requirements on purpose). Feel free to make it look pretty.

**New Requirement**

You cannot pass data as argument when navigating to the second screen.

- navigation.navigate('CheckoutSummary', { numItems }) ❌
- navigation.navigate('CheckoutSummary') ✅

### Thinking Process

[Figma with comments on my initial thoughts on this task](https://www.figma.com/file/B9xFGETTLUbDy28AXSiS4n/Cart-Assignment?node-id=0%3A1)

### Demo

https://user-images.githubusercontent.com/35736525/151750291-a4566e2e-ed7f-4ed2-9db6-baedc5082667.mp4


### Lessons Learnt

- Learnt how to use GraphCMS to add items via their interface & retrieve items using GraphQL in RN app.
- Learnt how to use Zustand for state management and Zustand Flipper plugin for debugging.
- Learnt how to use Expo Cli to make a bare RN project expo-compatible
- It's pretty interesting how I didn't think about passing the number of items using the navigation props at all from the beginning, so I just completed the additional task by chance. 
