[jsx-without-react](https://dirkarnez.github.io/jsx-without-react/)
===================================================================
From [How to Use JSX Without React. JSX gives us a great way to handle… | by Kartik Nair | Better Programming](https://betterprogramming.pub/how-to-use-jsx-without-react-21d23346e5dc)

### Notes
- newer version of [@babel/standalone - npm](https://www.npmjs.com/package/@babel/standalone) does not work (expecting `window.React`). This project uses the oldest version `7.0.0`
- svg must use `createElementNS` instead
  - [Editor — Convert SVG to valid JSX.](https://svg2jsx.com/)
 
### TODOs
- [ ] [hubs/src/utils/jsx-entity.ts at master · Hubs-Foundation/hubs](https://github.com/Hubs-Foundation/hubs/blob/master/src/utils/jsx-entity.ts)
- [ ] [dhow/src/jsx-runtime.js at master · kartiknair/dhow](https://github.com/kartiknair/dhow/blob/master/src/jsx-runtime.js)
  - ```
    function App() {
      return <h1>Hello World</h1>;
    }
    
    // Inserted by a compiler (don't import it yourself!)
    import {jsx as _jsx} from 'react/jsx-runtime';
    
    function App() {
      return _jsx('h1', { children: 'Hello world' });
    }
    
    https://www.npmjs.com/package/jsx-runtime
    https://github.com/OpenJSX
    https://github.com/OpenJSX/jsx-to-html
    https://github.com/OpenJSX/jsx-to-html
    https://github.com/OpenJSX/jsx-to-idom
    https://github.com/OpenJSX/jsx-to-dom
    https://github.com/OpenJSX/jsx-runtime
    ```

### Reference
- [How to create the app using JSX without React - DEV Community](https://dev.to/devsmitra/how-to-create-the-app-using-jsx-without-react-k08)
- [Using JSX without react - DEV Community](https://dev.to/kartiknair/using-jsx-without-react-28eb)
- [jsx-in-the-browser (forked) - CodeSandbox](https://codesandbox.io/s/jsx-in-the-browser-forked-xxfvio?file=/main.js)
- [How to Use JSX Without React. JSX gives us a great way to handle… | by Kartik Nair | Better Programming](https://betterprogramming.pub/how-to-use-jsx-without-react-21d23346e5dc)
