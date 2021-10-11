# Stuffy Granny

Current library is interlayer beetween firebase/firebase-firestore and your own project. Stuffy Granny is helper to request data from firestore. Own project is pet-project `Stranger Places App`.
The idea of it, Improve you skills to create light-way mobile app by RN. Supported React native and written on TS.

**Some information about package that you should know before use it**

## Installation

```bash
yarn add stuffy-granny-lib

npm install stuffy-granny-lib
```

###!important
Before install current library to you project, You need to install everything for [firebase-firestore](https://rnfirebase.io/firestore/usage "firebase-firestore").

To get config of firebase app, request it from Stuffy or Granny!=)

## Usage
Create a file in root of your project, reccomened to named `sglib.config.tsx`

 ##### Import firestore
```javascript
import firestore from '@react-native-firebase/firestore';
```
##### Import stuffy-granny-lib
```javascript
import StuffyGrannyLib from 'stuffy-granny-lib';
```
##### Create instance of stuffy-granny-lib class with argument firestore and export it.
```javascript
export const DB = new stuffy-granny-lib(firestore);
```
Done!!
Now if you need to make some requests to firestore, you need to import DB, and use method that you need.
Example:
```javascript
...
	async () => {
		const result = await DB.getAllUsers();
	}
...
```
### Methods
Methods will add soon. Check methods of class StuffyGranny in `index.tsx` of library.
