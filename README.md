# A typical page

A typical page that display a form to type email and password, built while learning React on Udemy.

# Feature

- The home page display a form to type in email and password. Simple validation of the input will be carried out.

- If both inputs are valid, it will display a "Welcome Page" with changes in the navigation bar.

# What I Learned

- Used `useEffect` hook to store data in browser storage and learned about the dependencies array.
- Used `useReducer` hook for state management on some of the states. (Replace `useState` in some cases).
- Used React Context API to avoid long prop chain:
  - In `store` folder, use `React.createContext()` and export a functional component named `ContextNameProvider` which return `<ContextName.Provider>`.
  - Add `<ContextName.Consumer>` as wrapper OR use `useContext` hook in the target component.
  - In `index.js`, wrap `<App/>` with `<ContextNameProvider> `.
  - _Limitation: not optimized for high frequency changes_
