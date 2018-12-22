---
title: Use Provider to Connect Redux to React
---
## Use Provider to Connect Redux to React
```
class AppWrapper extends React.Component {
  // render the Provider here
  render() {
      return (
    <Provider store={store}>
        <DisplayMessages />
    </Provider>
      );
  }
  // change code above this line
};
```
