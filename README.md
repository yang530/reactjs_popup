# Reactjs Popup Component
This is a popup component for React.js. It is modularized and easily scalable.

# Documentation:

## Required Props

1. pState: must be a state variable of boolean such as: "const [popup_state, setPopupState] = useState(false)".
2. setPState: must be a set state function for pState, so that the "X" button may close the popup when clicked.
3. props.children: contents enclosed between <Popup></Popup> will be displayed inside popup window.

## Example

```
import Popup from "./Popup.js";
import "./Popup.css";

function Home(){
  
  const [popup_state, setPopupState] = useState(false);
  
  return(
    <Popup pState={popup_state} setPState={setPopupState}>
        <h1>This is a Test modal</h1>
    </Popup>
  );
  
  function func(){
    //some code to control popup_state
  }
  
}

```
