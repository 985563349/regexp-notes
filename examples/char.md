**匹配16进制颜色**

```javascript
'#ffbbad #Fc01DF #FFF #ffE'.match(/#([a-zA-Z0-9]{6}|[a-z-A-Z0-9]{3})/g) // ['#ffbbad', '#Fc01DF', '#FFF', '#ffE']
```



**匹配时间**

```javascript
// 以24小时为例
const regex = /^([01][0-9]|[2][0-3]):[0-5][0-9]$/
regex.test('23:59') // true
regex.test('02:07') // true
```



**匹配日期**

```javascript
// 以 yyyy-mm-dd为例
/^[0-9]{4}-(0[1-9]|1[0-2])-(0[1-9]|[12][0-9]|3[01])$/.test('2022-07-14') // true
```



**windows操作系统文件路径**

```javascript
// 文件名不能出现特殊字符 \ : * | " ? \r \n /
/[a-zA-Z]:\\([^\\:*|"?\r\n/]+\\)*([^\\:*"?\r\n/]+)?$/.test('F:\\study\\javascript') // true
```



**匹配id**

```javascript
// 要求从 <div id="container" class="main"></div> 中提取出 id="container"
'<div id="container" class="main"></div>'.match(/id="[^"]*"/);
```

