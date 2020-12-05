# JavaScript使用マニュアル
## 高階関数
#### forEach
```javascript
var array = ["Tanaka","Suzuki","Yamada"];
//0:Tanaka 1:Suzuki 2:Yamada
arrat.forEach((v,idx) => {
  console.log(idx + ": " + v)
})
```
#### filter
```javascript
var array = [1,2,3,4,5];
//array = [1,2,3,4,5]
//a = [2,4]
var a = arrat.filter(v => {
  return v%2 === 0;
})
```
#### map
```javascript
var array = [1,2,3,4,5];
//array = [1,2,3,4,5]
//a = [6,7,8,9,10]
var a = arrat.map(v => {
  return v+5;
})
```
#### find
```javascript
var array = [1,2,3,4,5];
//array = [1,2,3,4,5]
//a = 2
var a = arrat.find(v => {
  return v%2 === 0;
})
//b = undefined
var b = arrat.find(v => {
  return v%6 === 0;
})
```
#### findIndex
```javascript
var array = [1,2,3,4,5];
//array = [1,2,3,4,5]
//a = 1
var a = arrat.findIndex(v => {
  return v%2 === 0;
})
//b = -1
var b = arrat.findIndex(v => {
  return v%6 === 0;
})
```
#### every
```javascript
var array = [1,2,3,4,5];
var array2 = [2,4];
//a = false 
var a = array.every(v => {
  return v%2 === 0;
})
//b = true 
var b = array2.every(v => {
  return v%2 === 0;
})
```
#### sum
```javascript
var array = [1,2,3,4,5];
var array2 = [1,3,5];
//a = true 
var a = array.sum(v => {
  return v%2 === 0;
})
//b = false
var b = array2.sum(v => {
  return v%2 === 0;
})
```
#### reduce
```javascript
var array = [1,2,3,4,5];
/*初期値：array[0]
  a = 1+2 =3
  a = 3+3 =6
  a = 6+4 =10
  a = 10+5 =15
*/ 
var a = array.reduce((a,b) => {
  return a+b;
})
```
#### reduce(初期値あり)
```javascript
var array = ["Taro", "Hanako", "Ichiro", "Keiko", "Jiro"];
/*初期値：array[0]
  a = 0+4 = 4
  a = 4+6 = 10
  a = 10+6 = 16
  a = 16+5 = 21
  a = 21+4 = 25
*/
var a = array.reduce((a, b) => {
  return a + b.length;
//初期値：0  
}, 0);
console.log(a); 
```