---
title: Send Action Data to the Store
---
## Send Action Data to the Store

1. Return an action object with type and text data by the action creator.
```
const addNoteText = (note) => {
  // change code below this line
  return {
    type: ADD_NOTE,
    text: note
  };
  // change code above this line
};
```

2. Return the text property on the incoming action as the new state when triggered by the ADD_NOTE action.

```
const notesReducer = (state = 'Initial State', action) => {
  switch(action.type) {
    // change code below this line
    case ADD_NOTE:
      return action.text;
    // change code above this line
    default:
      return state;
  }
};
```
