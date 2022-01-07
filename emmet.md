# emmet语法

## 快速生成HTML结构语法

- 生成标签 直接输入标签名 按tab键即可   比如  div   然后tab 键， 就可以生成 <div></div>

- 如果想要生成多个相同标签  加上 * 就可以了 比如   **div*3**  就可以快速生成3个div

- 如果有父子级关系的标签，可以用 >  比如   **ul > li**就可以了

- 如果有兄弟关系的标签，用  +  就可以了 比如 **div+p**  

- 如果生成带有类名或者id名字的，标签名.类名，如  **p.demo**  或者  **span#two**  就可以了

- 如果生成的div 类名是有顺序的， 可以用 **自增符号  $**   (从1开始)

- 如果想要在生成的标签内部写内容可以用  **{ }**  表示

  ```html
      <!-- 基本用法 -->
  ul>li*3
  
  div>span
  
  ul+ol
  
  		<!-- 自动带类名、id -->
  .demo
  >>>>
  		<div class="demo"></div>    默认生成带类的div标签
  
  p.demo
  >>>>
      <p class="demo"></p>
  
  span#first
  >>>>
      <span id="first"></span>
  
      <!-- 自增符号 $ 超级好用 -->
  div#div-id$*5
  >>>>
      <div id="div-id1"></div>
      <div id="div-id2"></div>
      <div id="div-id3"></div>
      <div id="div-id4"></div>
      <div id="div-id5"></div>
  div.demo$*5
  >>>>
      <div class="demo1"></div>
      <div class="demo2"></div>
      <div class="demo3"></div>
      <div class="demo4"></div>
      <div class="demo5"></div>
  
      <!--   {} 的使用   -->
  div{我是周大帅}*5
  >>>>
      <div>我是周大帅</div>
      <div>我是周大帅</div>
      <div>我是周大帅</div>
      <div>我是周大帅</div>
      <div>我是周大帅</div>
  
  div{我是第$个周大帅}*5
  >>>
      <div>我是第1个周大帅</div>
      <div>我是第2个周大帅</div>
      <div>我是第3个周大帅</div>
      <div>我是第4个周大帅</div>
      <div>我是第5个周大帅</div>
  ```

## 快速生成CSS样式语法

CSS 基本采取简写形式即可

​		比如 w200   按tab  可以 生成  width: 200px;

​		比如 lh26px   按tab  可以生成  line-height: 26px;