# How React Works
* Components, components, COMPONENTS!
* We create components in React for different parts of our application
  * E.g., components for Navbar, Search Box, & a Footer
  * It's then Readt's job to inject them into the DOM
  * It does this by taking the components and creating a JS representation of the DOM, i.e., the Virtual DOM

## The Virtual DOM
* React takes the Virtual DOM and renders it to the browser and creates the actual DOM based on the Virtual DOM
* Every time we make a change to the data or the UI state in a component then React looks at the change and shows it in the browser
* The Virtual DOM makes React fast... 
* So, when we first start up the application React creates the Virtual DOM based on all of the components and then renders it to the browser
* When the data or the UI state gets updated in a component React creates a new Virtual DOM in the background which is then compared to the old one that was initially created
* From the comparison between the old and new virtual DOMS we can see where the DOM needs to be updated and it only needs to update the component that has changed

## Components & Templates
* Components look like HTML templates actually JavaScript XML (JSX)
* They contain "state" (data or UI state)
* They also contain JavaScript for functionality