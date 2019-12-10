## In App.js covered classes vs. functions and state:

class -> properties -> functions

state is the source of all the information in React (central data management)

when you use this in a method in a class it refers back to the original class

## What you don't want to do in React
 Each componoent is going to get their data from where the data lives.  Props are what they will be using that is passed down from one component to another.
 You should not call the data (state) within the component
 

 ## New Note Topic

 When you call the function to create the html looking element it will have to be in Capital letters and not camelCase

 When exporting the function you will not place it in the object curly brackets.  If you do it will not return the correct function.

 - props are when you take state from the parent component and pass it down to the child component

 - a component has state a component is given props

 - left hand side "goats" matches right side of props in the component (replaced with butts below to see better)
```
  render() {
    return (
      <div className="App">
        <button className="btn btn-danger">Bootstrap Button</button>
        <GoatCorral butts={this.state.goats} />
      </div>
    );
  }
```

 ```
class GoatCorral extends React.Component {
  render() {
    const myGoats = this.props.butts;

    return (
      <div className="goatCorral">
        Goat Corral
      </div>
    );
  }
}
 ```
 - Props is the Goat Corral

 ## LifeCycle Methods

 - componentDidMount and render are examples
 - will start using map from here on our instead of forEach method, map returns out the information you need so skips a step that forEach would require.

 ## JSX 

 - Used on all components and areas of application

## Prop Types
- Good developers do this:
 `npm install prop-types --save`

 ```
 const goatShape = PropTypes.shape({
  id: PropTypes.string.isRequired,
  name: PropTypes.string.isRequired,
  age: PropTypes.number.isRequired,
  description: PropTypes.string.isRequired,
  imgUrl: PropTypes.string.isRequired,
  isBusy: PropTypes.bool.isRequired,
});
 ```

 - In goat corral you need to call a method from the 'Prop Types', in the goat you do not need to use this method so no need to import


 ## References

 - Goats Repo