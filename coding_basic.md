# JavaScript使用マニュアル

## JS呼び出し方
```javascript
<script>
  // ここにJavaScriptのコードを書きます
</script>
```

## コンソールへの出力
```javascript
//strictモードに設定
'use strict'

console.log('Hello');
```

## 型
#### 配列
```javascript
//配列の宣言
var array = [];
//要素の追加
array.push('Hello');
```
#### オブジェクト
```javascript
//オブジェクトの宣言
var obj = {};
//nameプロパティの追加
obj.name = 'Hello';
//ageプロパティの追加
obj['age'] = 22;
```
## 型変換
#### 文字列変換（toString）
```javascript
var val = 10;
//str = '10'
var str = val.toString(); 
```
#### 数値変換（parseInt）
```javascript
var str = '10';
//val = 10
//parseInt：第二引数は変化したい進数
var val = parseInt(str,10); 
```
#### 真偽値変換（Boolean）
```javascript
//false：0,undefined,null,NaN,''(空文字列)
var boolF = Boolean(0);
//true：0以外の数値,オブジェクト,配列,文字列
var boolT = Boolean(10); 
```

## 関数定義
```javascript
function 関数名(){

}
```

## 配列

#### 末尾に値追加（push）
```javascript
var array = [1,2,3];
//array = [1,2,3,4]
array.push(4);
```
#### 先頭に値追加（unshift）
```javascript
var array = [1,2,3];
//array = [0,1,2,3]
array.unshift(0);
```
#### 配列の連結（concat）
```javascript
var array1 = [1,2,3];
var array2 = [4,5,6];
//array3 = [1,2,3,4,5,6]
var array3 = array1.concat(array2);
```
#### 先頭の要素削除（shift）
```javascript
var array = [1,2,3];
//array = [2,3] 
//a = 1 
var a = array.shift();
```
#### 末尾の要素削除（pop）
```javascript
var array = [1,2,3];
//array = [1,2] 
//a = 3 
var a = array.pop();
```
#### 要素の削除と挿入（splice）
```javascript
//index：変更開始位置
//howmany：削除する数
array.splice(index,howmany,挿入1,挿入2,...,挿入n)
```
```javascript
ex)
var array = [1,2,3];
//array = [1,10,20,30,3] 
//a = 2 
var a = array.splice(1,1,10,20,30);
```
#### 先頭から検索（indexOf）
見つけた場合：最初に見つけた要素番号を返す
見つからなかった場合：「-1」を返す
```javascript
ex)
var array = [1,2,3];
//array = [1,2,3] 
//index = 1 
var index = array.indexOf(2);
//index = -1 
var index = array.indexOf(4);
```
#### 末尾から検索（lastIndexOf）
見つけた場合：最初に見つけた要素番号を返す
見つからなかった場合：「-1」を返す
```javascript
ex)
var array = [1,2,1,3];
//array = [1,2,1,3] 
//index = 2 
var index = array.LastIndexOf(1);
//index = -1 
var index = array.LastIndexOf(4);
```
#### 要素を連結し文字列化（join）
```javascript
var array = [1,2,3];
//array = '123'
array.join("");
//array = '1,2,3'
array.join(",");
```
#### 一部を切り出す（slice）
元の配列は変更しない
```javascript
//begin：開始位置
/*end：終了位置（endは含まれない）
      指定しない場合は末尾まで
      負数の場合は末尾から数えた位置
*/
array.slice(begin,end);
```
```javascript
var array = [1,2,3];
//array = [1,2,3]
// a = [1,2]
var a = array.slice(0,2)
```
#### 文字列をソート（sort）
#### 数値をソート（sort(comparefunctin)）
比較関数を与える
```javascript
function compareFunction(a, b) {
  if (a < b) { // aがbよりも小さいときは-1を返す
    return -1;
  }
  if (a > b) { // aがbよりも大きいときは1を返す
    return 1;
  }
  // aとbが等しいときは0を返す
  return 0;
}

var arrays = [1,2,5,3,10];
//文字列ソートのため
//array = [1,10,2,3,5]
arrays.sort()

var arrayn = [1,2,5,3,10];
//array = [1,2,3,5,10]
arrayn.sort(compareFunction)
```



