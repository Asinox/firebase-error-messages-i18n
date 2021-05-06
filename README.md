# firebase-error-messages-i18n

## Installation

Using npm

```
$ npm i firebase-error-messages-i18n
```

Using yarn

```
$ yarn add firebase-error-messages-i18n
```

## Usage

```js
import firebase from "firebase";
import fbmessage from "firebase-error-messages-i18n/es-do.json";

firebase
  .auth()
  .signInWithEmailAndPassword("email", "password")
  .catch(e => {
    const errorText = fbmessage[e.code] || e.message;
    alert(errorText);
  });
```

## Contribution

Envía un pull request.

## License

[MIT](https://opensource.org/licenses/MIT)