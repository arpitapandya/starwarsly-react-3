### Conceptual Exercise

Answer the following questions below:

- What is Redux? Why might you use it?
    Redux is used mostly for application state management. Redux maintains the state of an entire application in a single immutable state tree(object), which can't be changed directly. When something changes, a new object is created (using actions and reducers).

- What are three features of the Redux developer tool in Chrome?
.   Trace
.   Actions
.   State

- What is a store?
    A store is basically just a plain JavaScript object that allows components to share state.

- What is a reducer?
    A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change.

- What is an action?
    An action is a plain JavaScript object that has a type field. An action is an event that describes something that happened in the application.

- What is an action creator?
    An action creator is a plain function that returns an action objet.

- How does data flow in a React/Redux application?
    Redux follows the unidirectional data flow. It means that your application data will follow in one-way binding data flow. As the application grows & becomes complex, it is hard to reproduce issues and add new features if you have no control over the state of your application.Redux reduces the complexity of the code, by enforcing the restriction on how and when state update can happen.

- What is the purpose of the `<Provider>` component?
    The <Provider /> makes the Redux store available to any nested components that have been wrapped in the connect() function. Since any React component in a React Redux app can be connected, most applications will render a <Provider> at the top level, with the entire app's component tree inside of it.

- What is the purpose of the `useSelector` hook? What does it return?
    The useSelector hook takes a selector function to select data from the store and another function equalityFn to compare them before returning the results and determine when to render if the data from the previous and current state are different.

- Describe the `useDispatch` hook. What do you use it for?
    useDispatch() hook returns a reference to the dispatch function from the redux store. You may use it to dispatch actions as needed.

- What is redux-thunk and why would you use it?
    Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store's dispatch method, which is then used to dispatch regular synchronous actions inside the function's body once the asynchronous operations have been completed.

- What are propTypes?
    A prototype is an early sample, model or release of a product created to test a concept or process.

- Describe the `useCallback` hook.  What is it used for?
    `useCallback` will return a memoized version of the callback that only changes if one of the dependencies has changed.

- Compare and contrast the `useReducer` hook with Redux (including react-redux). Why would you choose one over the other?
    `useReducer` is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.