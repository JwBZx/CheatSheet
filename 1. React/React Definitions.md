<h1>Definitions:<h1>

<b>#1: React:<b>
React is “just the V in MVC” or “just the view layer”.

<b>#2: JSX:<b>
React’s HTML like syntax is called JSX. JSX allows us to write HTML like syntax which gets transformed to lightweight JavaScript objects. [The “HTML” that you’re writing in the render method isn’t actually HTML but it’s what React is calling “JSX”.] JSX simply allows us to write HTML like syntax which gets transformed to lightweight JavaScript objects. React is then able to take these JavaScript objects and from them form a “virtual DOM” or a JavaScript representation of the actual DOM. This creates a win/win situation where you get the accessibility of templates with the power of JavaScript.
(To see the definitions of (a) "render [Method]" and (a) "virtual DOM", see below/#6 and #8)

<b>#3: Components:<b>
Components are the building blocks of React. If you’re coming from a different background, they’re essentially widgets or modules. You can think of a component as a collection of HTML, CSS, JS, and some internal data specific to that component. These components are defined either in pure JavaScript or they can be defined in what the React team calls “JSX”.

<b>#4: Parent/Child Component:<b>
What makes React so convenient for building user interfaces is that data is either received from a component’s parent component, or it’s contained in the component itself.
Above we have a picture of my Twitter profile (To see the image of the Twitter profile, see I#1). If we were going to re-create this page in React, we would break different sections up into different components (highlighted). Notice that components can have nested components inside of them. We might name the left component (pink) the “UserInfo” component. Inside the UserInfo component we have another component (orange), that we could call the “UserImages” component. The way this parent/child relationship works is our UserInfo component, or the parent component, is where the ‘state’ of the data for both itself and the UserImage component (child component) lives. If we wanted to use any part of the parent component’s data in the child
component, which we do, we would pass that data to the child component as an attribute. In this example, we pass the UserImage component all of the images that the user has (which currently live in the UserInfo component).relationship works is our UserInfo component, or the parent component, is where the ‘state’ of the data for both itself and the UserImage component (child component) lives. If we wanted to use any part of the parent component’s data in the child
 component, which we do, we would pass that data to the child component as an attribute. In this example, we pass the UserImage component all of the images that the user has (which currently live in the UserInfo component).

<b>#5: createClass (Method):<b>
First, let’s go ahead and create our very first HelloWorld component so you can visualize how we use createClass to create a component. createClass takes in an object and this object is
what will specify the different properties (render, getInitialState, propTypes) of the component. The only method on the object we’re passing to createClass is the render method. React.createClass is the way in which you create a new component.

<b>#6: render (Method):<b>
Every component is required to have a render method. (The reason for that is) render is essentially the template for our component. So in this example the text that will show on the screen where this component is rendered is Hello World! Render (Method) is (what we use to show/set) what we would like our HTML Template to look like.

<b>#7: ReactDOM.render (Method):<b>
[We’ve saved the result of calling our React.createClass constructor into a variable called HelloWorld. We do this because later on we’ll need to tell React to which element our component should be rendered.] This is where ReactDOM.render comes into play. ReactDOM.render takes in two arguments. The first argument is the component you want to render, the second argument is the DOM node where you want to render the component. In the example above we’re telling React to take our HelloWorld component and render it to the element with an ID of app. Because of the parent/child relations of React we talked about earlier, you usually only have to use ReactDOM.render once in your application because by rendering the most parent component, all child components will be rendered as well. ReactDOM.render renders a React component to a DOM node.

<b>#8: virtual DOM:<b>
The Virtual DOM is a JavaScript representation of the actual DOM. Since the virtual DOM is a JavaScript representation of the actual DOM, React can keep track of the difference between the current virtual DOM (computed after some data changes), with the previous virtual DOM (computed before some data changes). Because manipulating the actual DOM is slow, React is able to minimize manipulations to the
actual DOM by keeping track of a virtual DOM and only updating the real DOM when necessary and with only the necessary changes. By re-rendering the virtual DOM every time any state change occurs, React makes it easier to think about what state your application is in.
difference between the current virtual DOM (computed after some data changes),
with the previous virtual DOM (computed before some data changes). Because manipulating the actual DOM is slow, React is able to minimize manipulations to the
actual DOM by keeping track of a virtual DOM and only updating the real DOM when necessary and with only the necessary changes. By re-rendering the virtual DOM every time any state change occurs, React makes it easier to think about what state your application is in.

<b>#9: state:<b>
state is the internal data store (object) of a component.
Earlier we talked about how managing user interfaces is difficult because they typically have lots of different states. Each component has the ability to manage its own state and pass its state down to child components if needed.
If another component also needed this state/data but that state wasn’t a direct child of the UserInfo component, then you would create another component that would be the direct parent of the UserInfo and the other component (or both components which required that state), then you would pass the state down as props into the child components. In other words, if you have a multi component hierarchy, a common parent component should manage the state and pass it down to its children components via props.

<b>#10: getInitialState (Method):<b>
The getInitialState method is “The way in which you set the state of a component”. In other terms, getInitialState returns an object which contains the state or data for our component. [In the code above we’re telling our component that we want it to keep track of a username. This username can now be used inside our component by {this.state.username}, which is exactly what we do in our render method.]

<b>#11: setState (Method):<b>
setState is a helper method for altering the state of a component. Our component needs the ability to modify its own internal state. We do this with a method called setState. Whenever setState is called, the virtual DOM re- renders, the diff algorithm runs, and the real DOM is updated with the necessary changes.
[So in the next code sample, we’re going to now have an input box that whenever someone types into it, it will automatically update our state and change the username.]

<b>#12: handleChange (Method):<b>
The handleChange method is going to get called every time a user types in the input box. When handleChange is called, it’s going to call setState to re-define our username with whatever was typed into the input box (e.target.value).
 our getInitialState method and will be updated in the handleChange method.]

<b>#13: onChange (Method):<b>
onChange is a React thing and it will call whatever method you specify every time the value in the input box changes, in this case the method we specified was handleChange.
[A user types into the input box → handleChange is invoked → the state of our component is set to a new value → React rerenders the virtual DOM → React Diffs the change → Real DOM is updated.]

<b>#14: props:<b>
props is the data which is passed to the child component from the parent component. This allows for our React architecture to stay pretty straight forward. Handle state in the highest most parent component which needs to use the specific data, and if you have a child component that also needs that data, pass that data down as props.
All getter/setter method for a certain piece of data will always be in the same component where that data was defined. If you needed to manipulate some piece of data outside where the data lives, you’d pass the getter/setter method into that component as props.
[The reason for this is because the parent component (FriendContainer) doesn’t care about the new friend you’re adding, it only cares about all of your friends as a whole (the friends array). However, because we’re sticking with the rule of only manipulate your data from the component that cares about it, we’ve passed the addFriend method down into our AddFriend component as a prop and we call it with the new friend once the handleAddNew method is called.]

<b>#15: map (Method):<b>
All map does is it creates a new array, calls our callback function on each item in the array, and fills the new array with the result of calling the callback function on each item.
[Notice all that happened was we made a new array and added <li> </li> to each item in the original array.
So in our child component above, we’re mapping over names, wrapping each name in a pair of <li> tags, and saving that to our listItems variable. Then, our render method returns an unordered list with all of our friends.]

<b>#16: propTypes:<b>
propTypes allow you to control the presence, or types of certain props passed to the child component. With propTypes you can specify that certain props are required or that certain props be a specific type.
returns an unordered list with all of our friends.]

<b>#17: getDefaultProps:<b>
getDefaultProps allows you to set default props for your component. getDefaultProps allow you to specify a default (or a backup) value for certain props just in case those props are never passed into the component.

<b>#18: Component LifeCycle:<b>

<b>#19: componentWillMount:<b>
componentWillMount is fired before the component will mount and is invoked once before the initial render.
[If you were to call setState here, no re-render would be invoked. An example of this would be if you’re using a service like firebase, you’d set up your reference to your firebase database here since it’s only invoked once on the initial render.]

<b>#20: componentDidMount:<b>
componentDidMount is fired after the component mounted and is invoked once after the initial render.
[Because the component has already been invoked when this method is invoked, you have access to the virtual DOM if you need it. You do that by calling this.getDOMNode().]

<b>#21: componentWillReceiveProps:<b>
componentWillReceiveProps is fired whenever there is a change to props and this life cycle is not called on the initial render, but is instead called whenever there is a change to props.
[Use this method as a way to react to a prop change before render() is called by updating the state with setState.]

<b>#22: componentWillUnmount:<b>
componentWillUnmount is fired before the component will unmount and this life cycle is invoked immediately before a component is unmounted from the DOM. This is where you can do necessary clean up. [For example, going back to our firebase example this is the life cycle event where you would clean up your firebase reference you set in componentWillMount.]
[There are a few more life cycle methods, but the ones I’ve covered are the ones that
I’ve seen which are the most useful.] #?1: onClick (Event):
[For example, going back to our firebase example this is the life cycle event where you
would clean up your firebase reference you set in componentWillMount.]
[There are a few more life cycle methods, but the ones I’ve covered are the ones that
I’ve seen which are the most useful.]
