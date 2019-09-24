# React Native Wheel of Fortune

# Run on your device

Snack: https://snack.expo.io/@catalinmiron/react-native-wheel-of-fortune

### Youtube tutorial

[![React Native Wheel of Fortune Youtube tutorial](react-native-wheel-of-fortune-tutorial.gif)](https://www.youtube.com/watch?v=tc3G-bO1p8Q)

In this lesson we’re going to be building a **Wheel of Fortune** in React Native using react-native-gesture-handler, D3 (d3-shape) and Expo for creating the react-native project.

- Expo: https://expo.io/
- React Native Gesture Handler: https://github.com/kmagiera/react-native-gesture-handler
- Popmotion Popcorn: https://popmotion.io/popcorn
- RandomColor: https://randomcolor.lllllllllllllllll.com
- Pin SVG: http://clipartist.net/social/clipartist.net/G/places_pin_icon.svg


### Example
#### Component usage example:
```
const participants = [1,2,3,4,5]
const rewards = participants.map( e => ({ uri: `https://i.pravatar.cc/300?${e}` }) )

return (
<View style={styles.container}>
    <WheelOfFortune
        onRef={ref => (this.child = ref)} 
        rewards={ rewards }
        knobSize={20}
        borderWidth={0}
        borderColor={'#fff'}
        playButton={() => (<Image style={styles.playButton} source={ circleArrows } />) }
        colors={['#99BAE1', '#73A4D0', '#4C7CBE']}
        winner={3}
        innerRadius={100}
        duration={1000}
        backgroundColor={'#fff'}
        getWinner={ (value, index) => {
            console.log('====================================');
            console.log('FINISH!', value);
            console.log('====================================');
        }}
    />
    <Button title="Press me" onPress={ () => { this.child._onPress() } } />
</View>
);
```


You can find me on:

- Github: http://github.com/catalinmiron
- Twitter: http://twitter.com/mironcatalin

Wanna give me a coffe?

- Paypal: mironcatalin@gmail.com
