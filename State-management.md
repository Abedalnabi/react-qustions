- Why do we use a global state instead of props?
- How can we get and update data anywhere in our app without using props?
- what is the react hook we use to manage the global state in one place?
- what is useReducer used for?
- what is the difference between useReducer and useState?
- what is useReducer return and what are the arguments it takes?
- what is dispatch do in useReducer?
- the dispatch function got two arguments what should be it?
- what is the benefit of using the dispatch function rather than setState function in useState?
- why do we pass action arguments to dispatch?
- what action do in the dispatch function?
- What arguments does the reducer take?
- what does the reducer have to return?
- can we change the initial state starucure when we return it inside the reducer?
- how React checks if the state has been updated? React checks the difference between the new and the current state to determine whether the state has been updated
- What is the difference between useContext and useReducer?



- how can we make the useRducer state as a global state?
- look at the below code and answer the questions 
	
	<GrandComponent>
	    <ParentContext.Provider value={reducerState}>
	    	<childComponent/>
	    </ParentContext.Provider>
    	<Grand/>
    	
* What is React context?
* When should we use React context?
* What is the difference between useContext and createContext ?
* Can the GrandComponent access the value?
* what should we do to use the reducerState inside GrandComponent?
* how can we use the reducerState inside the childComponent?
* how can we update reducerState inside childComponent and how can we re-render childComponent when reducerState changes?
* What is the best file to put the ParentContext.Provider to use all states in any component of our project?

- What does useContext return?
- can we use more than one context in on project?
