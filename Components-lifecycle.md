# Components lifecycle Questions

- Could we send props from child to parent?
- How can we send props from parents to child?
- How can we edit some data(props) we catch in the child component from the parent component and show the modification we made in the parent?
- What type of props are in React? 
  - array 
  - object 
  - string 
  - Number

- Chose the correct answer => if we need to send data from child to parent we should do?
  - send function with parameters to child component 
  - send props from child to parent directly
  
- Mention the types of components in react?
- Mention the react functional component lifecycle phases and explain each one
  - which one is responsible of insert elements in Dom and which one removes the component from the Dom
  - when updating life cycle work?
  - How can we write code that runs after the component is mountd in react functional component?
  - When does the component re-render in React?

- Which hook do we use to run code after the component mounted ?
- How can we run code when the component is unmounted in functional component?
- What is the empty array meaning in useEffect hook?
- Which line of code means that component will re-render after any state changes?
  - useEffect(() => { console.log('hello world') }, []);
  - useEffect(() => { console.log('hello world') });
  - useEffect(() => { console.log('hello world') }, [state]);
- Which line of code means that the component will re-render once?
  - useEffect(() => { console.log('hello world') }, []);
  - useEffect(() => { console.log('hello world') });
  - useEffect(() => { console.log('hello world') }, [state]);
- how can we re-render the component when a specific state changes?
- When the state changes the life cycle will be
  - unmounting, mounting -updating
  - mounting, updating -unmounting
  - updating, mounting -unmounting
- In which phases will JSX element will render?
- Why do we use key attribute for each element in react when we use for loop
- If the parent mounting or re-render , will child component mounting also? 
- If the state changes in the child component, will is parent component be re-mounting also?
- Why do we have an infinite loop when trying to change the state inside useEffic without detrimines dependence array?
- What's the difference between Real DOM and Virtual DOM?
- Which will run before, return JSX codes or UseEffect codes?
- Why do we return <></> or <React.Fragment><React.Fragment/> insted of return div tag when we return JSX code in react ?
- Colud we define useState in UseEffect ? if now why do we cant?
- We have two additional react hook functions useCallback and useMemo
- What are the differences between useCallback and useMemo?
* Which one can we use to memoize a function that will not automatically run on every render?
* What dependence array means in useCallback function ? 
* How can we stop the child component re-render when his parent re-renders?
