# React Native Gradient Button

A lightweight Gradient Button library for React Native.

![Examples](./Examples.png =250x)

## Installation

```
yarn add react-native-gradient-button
# or
npm install --save react-native-gradient-button
```

## Props
  - `text`: `String`
    - No default
  - `gradientBegin`: `String` 
    - default: `'#00d2ff'`
    - options: Any hex, rgb, or color    
  - `gradientEnd`: `String`
    - default: `'#3a47d5'`
    - options: Any hex, rgb, or color
  - `gradientDirection`: `String`
    - default: `'horizontal'`
    - options: `horizontal`, `vertical`, `diagonal`
  - `height`: `Number` or `String` (for %)
    - default: `75`
  - `width`: `Number` or `String` (for %)
    - No default
  - `radius`: `Number`
    - default: `50`
  - `impact`: `Boolean`
    - default: `false`
  - `impactStyle`: `String`
    - default: `'Heavy'`
    - options: `Heavy`, `Medium`, `Light`

  **Design+Code Specifc Gradient Props**
  - purpleViolet
  - violetPink
  - pinkDarkGreen
  - blueViolet
  - blueMarine
  - deepBlue

## Examples

```
  <View style={{flex: 1, justifyContent: 'space-evenly', alignItems: 'center', marginVertical: 24}}>
    <GradientButton
      text="Gradient Button"
      gradientBegin="#874f00"
      gradientEnd="#f5ba57"
      gradientDirection="diagonal"
      height={60}
      width={300}
      radius={15}
      impact
      impactStyle='Light'
    />

    <GradientButton text="Purple Violet" width='90%' purpleViolet impact />
    <GradientButton text="Violet Pink" width='90%' violetPink impact />
    <GradientButton text="Pink Dark Green" width='90%' pinkDarkGreen impact />
    <GradientButton text="Blue Violet" width='90%' blueViolet impact />
    <GradientButton text="Blue Marine" width='90%' blueMarine impact />
    <GradientButton text="Deep Blue" width='90%' deepBlue impact />
  </View>
```