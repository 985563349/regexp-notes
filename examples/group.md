**trim方法模拟**

```javascript
const trim = (str) => str.replace(/^\s+|\s+$/g, '')
```



**单词首字母大写**

```javascript
const titleize = (str) => str.toLowerCase().replace(/(?:^|\s)\w/g, (c) => c.toUpperCase())
```



**驼峰化**

```javascript
const camelize = (str) => str.replace(/[-_\s]+(.)?/g, (match, c) => c ? c.toUpperCase() : c)
```



**中划线化**

```javascript
const dasherize = (str) => str.replace(/([A-Z])/g, '-$1').replace(/[-_\s]+/g, '-').toLowerCase()
```



**匹配成对标签**

```javascript
const regex = /<([^>]+)>[\d\D]*<\/\1>/
```

