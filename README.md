#Front-end Job Interview Questions Answer Practice

這邊是 fork 自 [Front-end Job Interview Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions) 的前端面試問題

**Note:** 利用 Repository 來練習，並整理自己會的觀念，敬請參考，有任何錯誤也請向我提出，感謝。


## <a name='toc'>目錄</a>

  1. [常見問題](#general-questions)
  1. [HTML 問題](#html-questions)
  1. [CSS 問題](#css-questions)
  1. [JS 問題](#js-questions)
  1. [測試問題](#testing-questions)
  1. [效能問題](#performance-questions)
  1. [網路問題](#network-questions)
  1. [程式碼問題](#coding-questions)
  1. [有趣問題](#fun-questions)

#### <a name='general-questions'>常見問題：</a>

* 你昨天或這週學習了什麼？
> 學習如何做一個產品的討論，邏輯思維的「聯盟 雇主與員工的新關係」

* 寫程式的哪部份最讓你感到很興奮或是有興趣？
> 把東西從無到有，依照自己或是團隊的想法，把他做出來的時候是非常有成就感的事情

* 最近有無遇過不容易的技術性問題，又如何解決？
> 報名網站，在報名前不能有送出方法被看到，增加被攻擊的機會

* 當你開發Web應用程式或網站時，針對UI、安全性、效能、SEO、維護性，以及技術，你考量的點是什麼？
* 說說你喜好的開發環境 (作業系統, 編輯器或 IDE, 瀏覽器, 開發工具 … 之類)。
	1. 開發.NET：Windows 10, Visual Studio 2015, Google Chrome,MS SQL Studio, Linq Pad, Post man, Visual Studio Code....
	2. 開發前端：Mac, Visual Studio Code, Sublime Text, Google Chrome, PostMan

* 你最熟悉哪一套版本控制系統？
> TFS, SVN, Github

* 你可以描述你在開發一個網站時的工作流程嗎？
    1. 確認需求
    2. 討論需求，使需求更明確
    3. 先快速做出 prototype 與 user 確認
    4. 訂出週期任務，持續交付與討論
    5. 完成網站


* 如果有 5 種不同的樣式表 (stylesheets)，該如何整併到網站？
* 你可以描述漸進增強 (progressive enhancement) 和優美退化 (graceful degradation) 間的差異嗎？
* 你怎麼優化一個網站的靜態檔案 (assets) 和資源 (resources)？
* 說出三種能加快網頁讀取速度的方法 (感覺上的速度或是真正的讀取時間)。
    1. js 打包
    2. 1. 檔案最小化
    3. 圖片最佳化
    4. css 最小化
    5. IIS 動態壓縮

* 如果你加入了一個專案，但是他們的程式碼用 tabs，但是你習慣用spaces (空白鍵)，你會怎麼做？
> 通常我會使用 IDE code formate 的功能

* 寫一個簡易的投影片頁面。
* 你用什麼工具來測試你的程式碼效能？
> google chrome dev tool

* 如果今年你能精通一項技術，那會是什麼？
> AngularJS 2

* 描述標準和製定標準機構的重要性？
* 什麼是 Flash of Unstyled Content？ 你怎麼避免 FOUC？
* 解釋什麼是 ARIA 與 screenreaders，它們是怎麼樣讓網站使用更無障礙？
> 基於正確的 HTML 結構(為圖片提供敘述性的文字取代方案﹑正確地使用標題標記、使用無障礙表格)，利用 ARIA 屬性，讓 label 與輸入欄位產生關係，這樣的架構，對於 screenreaders 可以更準確的表達網站內容。
> 
> 請參考 [設計大舌頭 - 我們都應該了解的 無障礙網頁 概念](https://designtongue.me/website-accessibility/)
* 解釋 CSS 動畫與 JavaScript 動畫之間的憂與劣。
> 針對簡單的「一次性」轉換，像切換 UI 元素狀態等，請使用 CSS 動畫。
當您想要擁有進階的效果，像彈跳、停止、暫停、倒帶或減速時，請使用 JavaScript 動畫。
如果您選擇使用 JavaScript 進行動畫處理，請採用 TweenMax，或者較輕量級的解決方案 TweenLite。
>
> 請參考 [Google Developer](https://developers.google.com/web/fundamentals/design-and-ui/animations/css-vs-javascript?hl=zh-tw)
* CORS 是什麼，它解決了什麼問題？
>CORS是一個瀏覽器技術的規範，全名是"跨來源資源共享"（Cross-origin resource sharing）。
>提供了 Web 服務從不同網域傳來沙盒腳本的方法，以避開瀏覽器的同源策略。

#### <a name='html-questions'>HTML 問題:</a>

* `doctype` 做什麼用的？
>  声明必须是 HTML 文档的第一行，在 HTML5 中只有一種，而在 HTML 4.01 中有三種 <!DOCTYPE> 聲明。
>  
> 請參考 [W3School](http://www.w3school.com.cn/tags/tag_doctype.asp)

* standards mode 和 quirks mode 有什麼不同？
>未宣告文件型態 (DOCTYPE) 的缺陷基本上就等同於瀏覽器進入 Quirks Mode 時使用 HTML/CSS 語法的限制與缺陷 (Box Model 定義不同)。
>
> 請參考 [文件型態與接縫模式（DOCTYPE & Quirks Mode）](http://mepopedia.com/?page=866)

* 使用 XHTML 有什麼限制？
>XHTML 是更严谨更纯净的 HTML 版本。
    1. 必須要有終止tag (ex: li, p, tr, th)
    2. 屬性和元素必須是小寫
    3. 屬性值必須使用引號括弧起來 (style = "width:10px;")
    4. 屬性值不能省略
    5. id屬性取代name屬性
    6. 跳脫字元不同
    7. 元素包含內容限制
> 請參考 [XHTML和HTML的差異](http://www.chou-it.com/info/dictionary/web/html/xhtml.html)

* 如果網頁使用 `application/xhtml+xml` 會有問題嗎？
* 你怎麼做一個需要支持多國語言的網頁？
    1. i18n library
    2. l10n library
    3. DB Table對應

* 當開發和設計一個多國語言網站時，有什麼需要小心的？
> 翻譯內容不正確...

* `data-` 屬性的好處在哪？
* 考慮 HTML5 作為一個開放式的網站平台，組成 HTML5 的技術有哪些？
* 請描述 `cookies`, `sessionStorage` 和 `localStorage` 的不同？
    1. Cookie 可设置失效时间。如果在浏览器端生成Cookie，默认是关闭浏览器后失效。
    2. localStorage 除非被清除，否则永久保存。
    3. sessionStorage 當前對話有效，關閉頁面或瀏覽器時清除。
> 請參考 [详说 Cookie, LocalStorage 与 SessionStorage](http://jerryzou.com/posts/cookie-and-web-storage/)

* 描述下列之間的不同 `<script>`, `<script async>` & `<script defer>`。
> script 會等 script 下載完，網頁才會繼續 render。
> script async 會讓 script 在背景下載，下載完畢先執行 script 再繼續 render 網頁。
> script defer 會讓 script 在背景下載，等 DomContentLoaded 在執行 script。

* 為什麼把 CSS `<link>` 放在 `<head></head>` 之間，與將 JS `<script>` 放在 `</body>` 之前是個較好的主意？有什麼例外情形嗎？
> 網頁為依序執行的程式，先讀取 css，讓 html 先排版，以免使用者看到未排版的網頁，又突然完成排版的情況。
> Script js 通常跟排版無關，多為綁定事件，所以使用者再看到畫面到點擊畫面還有一段時間，足以完成綁定。

* 什麼是漸進式呈現？
* 有用過 HTML 樣板語言（template languages）嗎？

#### <a name='css-questions'>CSS 問題：</a>

* CSS 的 class 和 ID 兩者有何差異？
* 描述 "resetting" 和 "normalizing" 的差異性？你會選擇哪一種，為什麼選擇它？
* 描述 Floats 並解釋如何運作。
* 描述 z-index 並且描述堆疊內容 (stacking context) 如何形成。
* 解釋 BFC(Block Formatting Context) 是什麼、如何運作的。
* 有哪些不同的 clearing 技術？哪個適用在哪種內容上？
* 描述 CSS sprites, 你如何實作在網頁或網站上？
* 你最喜愛的圖片取代技術是什麼？你什麼時候會用到？
* 針對各瀏覽器制定的樣式表（browser-specific styling），你的做法是？
* 你怎麼讓你的網頁支援有功能限制的瀏覽器？
  * 你會使用什麼樣的技術/流程 ？
* 有什麼方法來隱藏網頁的內容？ (只顯示在 screen readers)？
* 你使用過 grid system 嗎？如果有的話？你較推薦哪個？
* 你曾經實作 media queries 或是 mobile specific (手機規格的) layouts/CSS?
* 你熟悉任何有關 SVG 嗎？
* 你如何優化你的網頁以利於列印？
* 在寫高效的 CSS 時，有什麼要注意的？
* 使用 CSS preprocessors 的優點和缺點是什麼？ (Sass, Compass, Stylus, LESS)
  * 描述你使用過的喜歡和不喜歡的 CSS preprocessors。
* 你如何使用非標準字體來實作網頁設計？
* 解釋瀏覽器如何按照 CSS selector 找到對應的 element。
* 解釋你所認知的 box model，以及你如何在 CSS 告訴瀏覽器使用不同 box model 來呈現圖層？
* 請解釋 `* { box-sizing: border-box; }`？並且說明使用它的好處？
* 請列出您記憶中 display 屬性的全部值。
* 請說明 inline 和 inline-block 的差異性？
* 請說明 relative、fixed、absolute 和 static 元件差異性？
* 'C' 在 CSS 中代表層疊。樣式的優先級（舉出範例）？如何利用這項功能？
* 你目前有使用哪一套 CSS Framework 在開發環境或產品線上？
  * 如果有，請問是哪一套，並且描述如果改善或提昇 CSS Framework？
* 請問你有使用過 CSS Flexbox 或 Grid specs？
* 如何區分 responsive design 與 adaptive design 有何不同？
* 你曾經使用過 retina graphics？如果有，是在什麼時機以及用了什麼技術？
* 為什麼會用 `translate()` 代替 *aboslute positioning*，或者用 *absolute positioning* 代替 `translate`？為什麼要這樣？

#### <a name='js-questions'>JS 規格問題集：</a>

* 描述 event delegation。
>用 seletor 綁定事件的時候，可以直接使用 $("#test [type=button]").on("click",function(){});
>但這樣在動態增減 element 的時候，不會把事件帶進去，需要重新 binding
>故可以使用 event delegation，把事件綁在上層 (甚至document)，讓事件篩選器來分派事件。
>$("#test").on("click","[type=button]",function(){ });
>
> 請參考 [為什麼有時你應該優先考慮 event delegate 而不是 event binding](http://ithelp.ithome.com.tw/articles/10120565)


* 描述 `this` 如何在 JavaScript 中運作。
    1. this指向於調用該函式之物件
    2. 如果調用函式的前方並未有物件，則函式內this就指向全域物件
    3. this指向利用call或apply所指派給this的物件
    4. 若將函式當作建構式(constructor)來用，則內部的this則指向於new所產生之新物件
    5. .callback函式內的this會指向於調用放入該callback的函式之this所指向之物件
> 請參考 [Javascript：this用法整理](https://software.intel.com/zh-cn/blogs/2013/10/09/javascript-this)

* 描述 prototypal inheritance 如何運作？
> 透過 portotype chain 達成，所有物件都繼承自 Object，包含 function，當取用特定屬性的時候，會先從物件的範圍開始找，如果沒有則會尋找 portotype 的定義，若 prototype 沒有定義則指向 undefined。

* 你如何測試你的 JavaScript？
* AMD vs. CommonJS?
* 解釋下列程式碼為什麼不是IIFE: `function foo(){ }();`.  (Immediately Invoked Function Expression,立即函式)
  * 需要修改那裡使它成為IIFE?
> 需要用括號把 function 括起來，或是用變數接起來
`(function foo(){ })();`
`var ppp = function foo(){ }();`

* `null`、`undefined`和 `undeclared`變數之間有什麼差異？
  * 你如何檢查？
> undeclared 是變數未宣告卻使用，而造成的 error
> undefined 是呼叫變數或方法，但這個方法沒有實際被 Create，造成的結果 
`var undefinedVariable; // undefined`
`typeof undefinedVariable; // "undefined"`
> null 變數被定義為 null 的值，所以 
`var nullVariable = null; // null`
`typeof nullVariable // "object"`
* undeclared variables don’t even exist
* undefined variables exist, but don’t have anything assigned to them
* null variables exist and have null assigned to them

* 什麼是 closure, 如何/為什麼使用?
> 閉包，將變數關入自己的作用範圍

* anonymous functions 典型的使用時機？
`var func = function () { //dosomthihing }`
經常性呼叫，可以重複使用，當 function 名稱修改，程式不需跟著動


* 你如何架構你的程式碼？ (module pattern, classical inheritance?)
* host objects 和 native objects 有何不同？
* `function Person(){}`、`var person = Person()`和`var person = new Person()`之間有何不同？
* `.call` 和 `.apply`有何不同？
> 都是執行 function ，並給定 執行者 (this)，差別在於接參數方式
`function.apply(object, [arg1,arg2 ...]);`
`function.call(object, arg1, arg2 ...);`

* 描述 `Function.prototype.bind`?
> 告訴 function 中，function 中的這個 this 是誰。
`function (){}.bind(object);`

* 你什麼時候優化你的程式？
* 你什麼情況會使用 `document.write()`？
  * 多數的廣告產生仍然使用 `document.write()` 雖然這樣用會令人皺眉
* feature detection, feature inference, 和使用 UA string 有什麼不同？
* 盡可能的詳述描述 AJAX。
* 描述 JSONP 如何運作 (且為何它不是真正的 AJAX)。
* 你是用過 JavaScript templating (樣板) ？
  * 如果有的話，你有用過哪些 libraries？ (Mustache.js, Handlebars … 等)
* 描述 "hoisting"
* 描述 event bubbling.
* "attribute" 和 "property" 的不同？
* 為什麼擴展 JavaScript 內建的 objects 不是個好方法？
* document load event 和 document ready event 有什麼不同？
* `==` 和 `===` 有什麼不同？
> `==` 只會比較兩邊的 value
> `===` 會比較 value 跟 type

* 描述 JavaScript 的 same-origin policy (同源策略)
* 實作如下程式:

```javascript
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
```

* Ternary expression 怎麼來的, "Ternary" 的意思是什麼？
* 什麼是 `"use strict";`? 使用他的優點和缺點是什麼？
* 建個數到 `100` 的迴圈，當數字是 `3` 的倍數時輸出 **"fizz"**，當數字是 `5` 的倍數時輸出 `"buzz"`，當數字同時是 `3` 與 `5` 的倍數時輸出 **"fizzbuzz"**。
* 為什麼保持網站的全域(global scope)原樣是一個好做法？
* 為什麼要用 `load` 事件？有什麼缺點嗎？有其他選擇嗎？又為何選擇它？
* 解釋什麼是 single page app，並怎麼讓它對 SEO 更友善。
* 你對 Promises 的經驗？有用過相關的補強（ployfills）嗎？
* Promises 之於 callbacks 的優劣？
* JavaScript 轉譯器（transpiler）的優缺點？
* 你用什麼工具或技巧來做 JavaScript debug?
* 你都用什麼對 object properties 與 array 進行迭代？
* 解釋 mutable 與 immutable objects 之間的不同。
  * 舉個 immutable 在 JavaScript 中例子？
  * immutability 的憂劣？
  * 如何達成 immutability？
* 解釋同步（synchronous）與非同步（asynchronous）函式之間的差異。
* Event loop 是什麼？
  * call stack 與 task queue 之間的不同？

#### <a name='testing-questions'>測試問題集:</a>

* 寫測試有什麼好壞？
* 都用什麼工具測試代碼是否能運作？
* Unit test 與 functional/integration 間的不同？
* 監控代碼風格 linting 工具的用途是？

#### <a name='performance-questions'>效能問題集:</a>

* 你都用什麼工具尋找效能上的臭蟲？
* 有哪些方法可改善網站在 scrolling 效能？
* 解釋 layout, painting 與 compositing 的不同。（瀏覽器在 render 上的效能問題）

#### <a name='network-questions'>網路問題集:</a>

* 傳統上為什麼用多個域名來放置網站資源會比較好？
* 請詳細描述當您在網址列打入網址開始到最後網頁呈現在螢幕前的整個流程。
* Long-Polling, Websockets, SSE (Server-Sent Event) 之間有什麼差異？
* 請描述下列 request 和 response headers：
  * Diff. between Expires, Date, Age and If-Modified-...
  * DNT
  * Cache-Control
  * Transfer-Encoding
  * ETag
  * X-Frame-Options
* 列出所有你知道的 HTTP 操作，並詳加解釋。

#### <a name='coding-questions'>程式碼問題集:</a>

問題： `foo` 的值是什麼？

```javascript
var foo = 10 + '20';
```

> '1020' //類似強制同型

問題：實作符合下面的函式

```javascript
add(2, 5); // 7
add(2)(5); // 7
```

```javascript
function add (x, y){
	return x+y;
}

function add (x){
	return function (y){
    	return x+y;
    }
}
```

問題: 下面的 statement(陳述式) 會回傳什麼？

```javascript
"i'm a lasagna hog".split("").reverse().join("");
```

> "goh angasal a m'i" , 拆成陣列 > 陣列反轉 > 組合陣列

問題:  `window.foo` 的值是什麼？

```javascript
( window.foo || ( window.foo = "bar" ) );
```

> "bar" , window.foo 是 undefined 所以會是 false, 故會跑右邊的 window.foo = "bar"

問題: 下面的兩個 alerts 的結果會是什麼？

```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

> 第一個 alert 會是 Hello World，因為 IIFE
> 第二個 alert 會出錯，因為 bar undeclared

問題: 下面 `foo.length` 的值是什麼？

```javascript
var foo = [];
foo.push(1);
foo.push(2);
```

> 2

問題：下面這段會印出什麼？

```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

> one, three, two 
> 因為 settimeout的關係，會把 two 放進 queue，執行完 three 才會回來執行 queue 的方法。

#### <a name='fun-questions'>有趣問題：</a>

* 你最近寫過最酷的專案是？
* 你使用的開發工具中，你最喜歡的部分是什麼？
* 你有任何的 pet projects (個人開發的小專案)？ 什麼樣的？
* 你最喜歡 IE 瀏覽器的什麼特點？
* 喜歡咖啡嗎?

#### <a name='contributors'>貢獻作者群:</a>

此文件是由 [@paul_irish](http://twitter.com/paul_irish) [@bentruyman](http://twitter.com/bentruyman) [@cowboy](http://twitter.com/cowboy) [@ajpiano](http://twitter.com/ajpiano)  [@SlexAxton](http://twitter.com/slexaxton) [@boazsender](http://twitter.com/boazsender) [@miketaylr](http://twitter.com/miketaylr) [@vladikoff](http://twitter.com/vladikoff) [@gf3](http://twitter.com/gf3) [@jon_neal](http://twitter.com/jon_neal) [@sambreed](http://twitter.com/sambreed) and [@iansym](http://twitter.com/iansym) 於 2009 年共同發起。

目前已經超過 [100 開發者](https://github.com/h5bp/Front-end-Developer-Interview-Questions/graphs/contributors) 參與此專案.
