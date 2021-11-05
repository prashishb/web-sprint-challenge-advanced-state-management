# Interview Answers

Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?

   - Data sharing down a component tree without prop drilling to keep your state relatively clean.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

   - Actions: Objects that holds information needed for the store to modify state.
   - Reducers: Takes the current state and action as an argument and returns a new state according to the action.
   - Store: A container that holds the state of our application.

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?

   - thunk is a redux middleware that allows you to write action creators which returns a function. When action creator is called, thunk intercepts it. If the return is an action, it will send it to the reducer. But if the return is a function, it invokes it and passes the dispatch function as an argument.

4. What is your favorite state management system you've learned and this sprint? Please explain why!

   - Context. It's easier to setup and looks cleaner in my opinion. Makes sharing state easy without having to prop drill through so many levels.
