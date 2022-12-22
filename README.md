# show.js

一个html的js库，能够在元素出现在视口的时候添加class，执行动画，也能够监视一个元素，当元素出现在视口的时候执行回调函数
## useage

```html
<!-- html -->
<div class="show">
<div>
```

```js
// JavaScript
import {Show} from 'showjs'
//添加元素动画
new Show()
/**
 * selector: string = 'show'  默认的元素元素选择器
 * enterClass: string = 'animate__animated animate__flash' 默认的出现动画
 * leaveClass: string = 'animate__animated animate__swing' 默认的离开动画
 * options?: IntersectionObserverInit IntersectionObserver的配置，不传则使用默认配置
 * 
 */
//监听元素出现
new Show().listen(options:object)
/**
 * options: IntersectionObserverInit & { selector: string | Element[]; callback?: Function }
 * IntersectionObserverInit 同上，不传则使用默认
 * selector 监视元素class或Element[] 必传
 * callback 当监视的元素出现在页面时的回调函数
 */

//
```

### Install
```shell
npm i @sakurasz/show.js
```
or if you'd like to use yarn
```shell
yarn add @sakurasz/show.js
```