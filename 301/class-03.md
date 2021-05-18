# Passing Functions as Props

## Lists and Keys

* What does .map() return?
**Looping over an array and return a new one.**

* If I want to loop through an array and display each value in JSX, how do I do that in React?

        ReactDOM.render(
        < ul >{listItems}< /ul >,
        document.getElementById('root')
        );

* Each list item needs a unique **key**.

* What is the purpose of a key?
**To give the elements a stable identity.**



## The Spread Operator

* What is the spread operator?
**Quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.**


* List 4 things that the spread operator can do.
    * **Adding items to arrays.**
    * **Combining arrays or objects.** 
    * **Spreading an array out into a function’s arguments.**
    * **Converting NodeList to an array.**

* Give an example of using the spread operator to combine two arrays.

        const firstArray = [1,2,3]
        const secondArray = [4,5,6]
        const resultArray = [...firstArray ,...secondArray]

* Give an example of using the spread operator to add a new item to an array.

        const firstArray = [1,2,3]
        const secondArray = [...firstArray,4,5,6,]

* Give an example of using the spread operator to combine two objects into one.

        const objectOne = {hello: 1}
        const objectTwo = {world: 2}
        const objectThree = {...objectOne, ...objectTwo}

