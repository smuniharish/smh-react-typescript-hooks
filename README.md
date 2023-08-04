# smh-react-typescript-hooks

smh-react-typescript-hooks

## Installation
NPM
```sh
npm install smh-react-typescript-hooks
```
React or React Native
```sh
npm install --save smh-react-typescript-hooks
```
Expo
```sh
npx expo install smh-react-typescript-hooks
```
### Available Hooks
* useDefaultReducer

## Usage
This package is customized react hooks for making development easier, faster and more performant

#### useDefaultReducer
##### props

* options

| Parameter | Type     | Description | Default| **Required* |
| :-------- | :------- | :-------| :------- | :----- |
| `initialState` | `object` | the object of key value pairs | None | True |

* Structured Parameters

| Parameter | Definition | type |
| :-------- | :------- | :----- |
| `state` | This state always returns the latest state | object |
| `multipleAction` | fuction which accepts object type to update the state values | function |

State :
State is a set of values based on the initial state
multipleAction: Its a function accepts the updatable object values
### example
```js
import {useDefaultReducer} from 'smh-react-typescript-hooks'

// I would like to recommand to create initialState before the component declaration
const initialState = {
  email:null,
  password:null,
  ...
}
const component =>{
  //Declaration only inside the component
  const {state,multipleAction} = useDefaultReducer(initialState)

  useEffect(()=>{
    ...
    multipleAction({email:"samamuniharish@gmail.com",password:"123456"})
  },[])
}
```
And we're done 🎉
## Contributing

Contribution are always welcome, no matter how large or small !

We want this community to be friendly and respectful to each other.Please follow it in all your interactions with the project.

Please feel free to drop me a mail [S MUNI HARISH](samamuniharish@gmail.com)

## Acknowledgements

Thanks to the authors of these libraries for inspiration

## Sponsor & Support

To keep this library maintained and up-to-date please consider [sponsoring it on GitHub](https://github.com/sponsors/smuniharish). Or if you are looking for a private support or help in customizing the experience, then reach out to me on Linkedin [@smuniharish](https://www.linkedin.com/in/smuniharish).

## License

[MIT](./LICENSE)

---

Made with ❤️
