# Stuffy Granny

Current library is interlayer beetween firebase/firebase-firestore and your own project. Stuffy Granny is helper to request data from firestore. Supported React native and React and written on TS.


**Some information about package that you should know before use it**

## Installation

```bash
yarn add stuffy-granny-lib

npm install stuffy-granny-lib
```

###!important
Before install current library to you project, You need to install everything for [firebase-firestore](https://rnfirebase.io/firestore/usage "firebase-firestore").

## Usage
Create a file in root of your project, reccomened to named `sglib.config.tsx`
```javascript
# Import firestore
import firestore from '@react-native-firebase/firestore'; (Example for Ract native)
# Import stuffy-granny-lib
import SGL from 'stuffy-granny-lib' (Example works for RN and R)

#create instance of StuffyGrannyLib class with argument firestore and export it.
export const DB = new SGL(firestore);

Done!!
Now if you need make some requests to firestore, you need to import DB, and use method that you need.
Example: 

...
	const result = await DB.getAllUsers();
...

```

