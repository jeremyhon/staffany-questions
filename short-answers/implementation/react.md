# React/React Native (5 mins)

1. How do you use a component’s internal state in a functional component?
2. Which lifecycle method should I use to listen for changes in a component’s prop(s)?
3. The code below is for a button component. List at least five mistakes (functional or style wise)

```
    import React from 'react'
    import PropTypes from 'prop-types'

    class Button extends Component {
      constructor(props) {
        super(props)
      }

      state = {
        isPressed: false,
      }

      pressButton(evt) {
        this.setState({isPressed: !this.state.isPressed})
      }

      render() {
        this.setState({ isRendered: true })
        return (
          <button onPress={pressButton()}>
            {if (isPressed) "I was pressed!"}
          </button>
        )
      }
    }

    export default Button
```
