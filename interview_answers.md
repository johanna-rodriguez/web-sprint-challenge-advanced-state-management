# Interview Answers
Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?


The Context API is a React structure that enables you to exchange unique details and assists in solving prop-drilling from all levels of your application.


2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?


An action, is an object that contains the payload of information. They are the only source of information for the Redux store to be updated.
Reducers update store based on the value of the action.
A store is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer. Let us see how we can create a store using the createStore method from Redux.
The global state of your application is stored in an object tree within a single store.
This makes it easy to create universal apps, as the state from your server can be serialized and hydrated into the client with no extra coding effort. A single state tree also makes it easier to debug or inspect an application; it also enables you to persist your app's state in development, for a faster development cycle. 
Some functionality which has been traditionally difficult to implement - Undo/Redo, for example - can suddenly become trivial to implement, if all of your state is stored in a single tree.


3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?


Redux Thunk is a middleware that allows you to call the action creators that return a function(thunk) which takes the store's dispatch method as the argument and which is afterwards used to dispatch the synchronous action after the API or side effects has been finished.
Redux Thunk middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. 
The inner function receives the store methods dispatch and getState as parameters.



4. What is your favorite state management system you've learned and this sprint? Please explain why!

My favorite state management is Reducer function because are the perfect fit for managing changes in state while maintaining the immutability we want in our components.