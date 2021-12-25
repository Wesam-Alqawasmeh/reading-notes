# Class 41 Reading

---

## React Native

React Native combines the best parts of native development with React, a best-in-class JavaScript library for building user interfaces.

React Native lets you create truly native apps and doesn't compromise your users' experiences. It provides a core set of platform agnostic native components like View, Text, and Image that map directly to the platform’s native UI building blocks.

React components wrap existing native code and interact with native APIs via React’s declarative UI paradigm and JavaScript. This enables native app development for whole new teams of developers, and can let existing native teams work much faster.

React Native is like React, but it uses native components instead of web components as building blocks. So to understand the basic structure of a React Native app, you need to understand some of the basic React concepts, like JSX, components, state, and props. If you already know React, you still need to learn some React-Native-specific stuff, like the native components.

**ReactJS Counter Example**

        // ReactJS Counter Example using Hooks!

        import React, { useState } from 'react';



        const App = () => {
        const [count, setCount] = useState(0);

        return (
            <div className="container">
            <p>You clicked {count} times</p>
            <button
                onClick={() => setCount(count + 1)}>
                Click me!
            </button>
            </div>
        );
        };


        // CSS
        .container {
        display: flex;
        justify-content: center;
        align-items: center;
        }

**React Native Counter Example**

        // React Native Counter Example using Hooks!

        import React, { useState } from 'react';
        import { View, Text, Button, StyleSheet } from 'react-native';

        const App = () => {
        const [count, setCount] = useState(0);

        return (
            <View style={styles.container}>
            <Text>You clicked {count} times</Text>
            <Button
                onPress={() => setCount(count + 1)}
                title="Click me!"
            />
            </View>
        );
        };

        // React Native Styles
        const styles = StyleSheet.create({
        container: {
            flex: 1,
            justifyContent: 'center',
            alignItems: 'center'
        }
        });

![react native](https://e3arabi.com/wp-content/uploads/2020/12/React-Native-Titre.png)

---

## Expo

Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.

**Expo Snack Player**

It’s a handy tool created by Expo to embed and run React Native projects and share how they render in platforms like Android and iOS. The code is live and editable, so you can play directly with it in your browser.

![expo](https://docs.expo.dev/static/images/og.png)
