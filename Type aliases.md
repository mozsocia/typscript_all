```js


const logDetails = (uid: string | number, item: string) => {
    console.log(`${item} has a uid of ${uid}`);
}

const greet = (user: {name: string , uid: string | number}) => {
    console.log(`${user.name} says hello`);
}

//***************************************************************** */
type stringOrNum = string | number;

const logDetails2 = (uid:stringOrNum, item: string) => {
    console.log(`${item} has a uid of ${uid}`);
}


const greet2 = (user: {name: string , uid: stringOrNum}) => {
    console.log(`${user.name} says hello`);
}

type objWithName = {name: string, uid: stringOrNum}

const greetAgain = (user: objWithName) => {
    console.log(`${user.name} says hello`);
}