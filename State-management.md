# State management Questions

- Why do we use a global state instead of props?
- How can we get and update data anywhere in our app without using props?
- What is the react hook we use to manage the global state in one place?
- What is useReducer used for?
- What is the difference between useReducer and useState?
- What is useReducer return and what are the arguments it takes?
- What is dispatch do in useReducer?
- The dispatch function got two arguments what should be it?
- What is the benefit of using the dispatch function rather than setState function in useState?
- Why do we pass action arguments to dispatch?
- What action do in the dispatch function?
- What arguments does the reducer take?
- What does the reducer have to return?
- Can we change the initial state starucure when we return it inside the reducer?
- How React checks if the state has been updated? React checks the difference between the new and the current state to determine whether the state has been updated
- What is the difference between useContext and useReducer?
- How can we make the useRducer state as a global state?

```js
	<GrandComponent>
	    <ParentContext.Provider value={reducerState}>
	    	<childComponent/>
	    </ParentContext.Provider>
    	<Grand/>
```
- Look at the above code and answer the questions.	
	* What is React context?
	* When should we use React context?
	* What is the difference between useContext and createContext ?
	* Can the GrandComponent access the value?
	* What should we do to use the reducerState inside GrandComponent?
	* How can we use the reducerState inside the childComponent?
	* How can we update reducerState inside childComponent and how can we re-render childComponent when reducerState changes?
	* What is the best file to put the ParentContext.Provider to use all states in any component of our project?
- What does useContext return?
- Can we use more than one context in on project?
