# Disclaimer
This is simply a rework of original repo from at https://github.com/WrathChaos/react-native-counter-input 
which I refactor into pure JS from TypeScripts and removed all other tools and dependecies. Credit goes to FreakyCoder, kurayogun@gmail.com. 

<img alt="React Native Counter Input" src="assets/logo.png" width="1050"/>

<p align="center">
  <img alt="React Native Counter Input"
        src="assets/Screenshots/RN-Counter-Input.png" width="49%" />
  <img alt="React Native Counter Input"
        src="assets/Screenshots/RN-Counter-Input.gif" width="49%" />
</p>

<p align="center">
  <img alt="React Native Counter Input"
        src="assets/Screenshots/RN-Counter-Input-Horizontal.png"  />
</p>

# Installation

Add the dependency:

```bash
npm i react-native-counter-input
```

## Peer Dependencies

<h5><i>IMPORTANT! You need install them</i></h5>

```js
"@freakycoder/react-native-bounceable": ">= 0.1.1",
```

# Usage

## Import

```jsx
import CounterInput from "react-native-counter-input";
```

## Fundamental Usage

```jsx
<CounterInput
  onChange={(counter) => {
    console.log("onChange Counter:", counter);
  }}
/>
```

# Configuration - Props

| Property                      |   Type    |  Default  | Description                                                                               |
|-------------------------------|:---------:|:---------:|-------------------------------------------------------------------------------------------|
| style                         |   style   |  default  | change/override the main container style                                                  |
| horizontal                    |  boolean  |   false   | make the button horizontal design                                                         |
| initial                       |  number   |     0     | set the initial value for the counter input                                               |
| onChange                      | function  | undefined | set your own logic for onChange method, it triggers on any change                         |
| onChangeText                  | function  | undefined | it triggers when the TextInput changes                                                    |
| onIncreasePress               | function  | undefined | it triggers when the increase button is pressed                                           |
| onDecreasePress               | function  | undefined | it triggers when the decrease button is pressed                                           |
| backgroundColor               |  string   |   #fff    | change the CounterInput's background color                                                |
| min                           |  number   | undefined | set a minimum input value                                                                 |
| max                           |  number   | undefined | set a maximum input value                                                                 |
| step                          |  number   | undefined | set an amount of step to increment or decrement                                           |
| reverseCounterButtons         |  boolean  |   false   | reverse the counter buttons                                                               |
| increaseButtonBackgroundColor |  string   |  #0b349a  | change the CounterInput's active increase button background color                         |
| decreaseButtonBackgroundColor |  string   |  #0b349a  | change the CounterInput's active decrease button background color                         |
| ImageComponent                | component |   Image   | set your own Image component instead of default `RN Image` component such as; `FastImage` |

## Author

Iain Heng, iainheng@gmail.com

## License

React Native Counter Input is available under the MIT license. See the LICENSE file for more info.
