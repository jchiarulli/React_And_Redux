# Component State
* JavaScript Object
* Describes the current state of the component
  * data, UI-state
* The state of a component can be updated over time
  * a modal could close
  * the data we output could change

## Shopping Cart Component
* Here, we're storing the local data or state of the component
* Initial state of the component:
* { items: [{ name: "navy jumper", price: 9.99 }, { name: "ninja mask", price: 20.00 }]}
* If we add an item then the state will update to reflect the change:
* { items: [{ name: "navy jumper", price: 9.99 }, { name: "ninja mask", price: 20.00 }, { name: "black coat", price: 15.00 }]}
* Take the state of the component which we use to dynamically output the content inside of the component
* Keep the state and the ouput on the screen in sync

## Popup Component
* { showPopup: true } 
* { showPopup: false }