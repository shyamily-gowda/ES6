# ES6
ES6 features with examples
### Rest:

Would you like to bind the first few function parameters to variables, and others to single variables as an array?

```
function printColors(first, second, third, ...others) {
  console.log('Top three colors are ' + first + ', ' + second + ' and ' + third + '. Others are: ' + others)
}
printColors('yellow', 'blue', 'orange', 'white', 'black')
```
Result:
Top three colors are yellow


### for-of

Iterates over the array

```
const arr = [1,3,4];
for(const el of arr){
	console.log(el); 
}
```
Result:
1
2
3

### entries()

Array method to get index and element together.

```
const num = [1,3,4];
for(const [index,el] of num.entries()){
	console.log(index,el); 
}
```
Result:
0 1
1 3
2 4

### Of object
Enables extraction of requested properties from the object and assigning them to variables of the same name as properties.

```
function printName({fname,lname}){
    console.log('hi',fname,lname)    
}
const person = {
    fname : 'sam',
    lname: 'kumar',
    city: 'blore'
}
printName(person);
```
Result:
*hi sam kumar*
