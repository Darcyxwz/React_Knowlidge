# React_Knowlidge
## 分类
进行分类处理时，可以将要分类的物品塑造成一个object，并添加唯一区分属性value进行区分，这样可以避免混杂处理情况！
## Object
```js
const [checkedItems, setCheckedItems] = useState({}); //被勾选的tasks的对象
const checkedItemsNumber = Object.keys(checkedItems).length; //被勾选的数量
```
checkedItems这里被塑造为了一个object，它有key，value

Object.keys(objectName)：可以将object的keys转化为一个array，并用length求长度，从而得知有多少个keys

{ ...prevState }可以进行浅复制
```js
if (updatedCheckedItems[task]) {
  delete updatedCheckedItems[task];
} else {
  updatedCheckedItems[task] = true;
}
```
(updatedCheckedItems[task])，如果含有这个task（一个key），则为true，否则为undefined，注意，不是false!!!
```js
const isChecked = checkedItems[task] || false;
```
此时这种写法就可以使得答案一定为false！
## 
