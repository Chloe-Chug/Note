# Note

提示框

```

  alert('123');
  
```

一開視窗就執行

```

  window.onload = function() 
    {
      // console.log("window loaded")
    };
    
```

console.log 偵錯

```

  function myfunction()
    {
    console.log('123');
    }
    
```

for迴圈

```

  for (i = 0; i < 10; i++) 
    { 
    console.log(i);
    }
    
輸出後會在console裡面出現1~10


```

Global Variable 全域變數與 Local Variable 區域變數


```

  var var1=0;

  function plus()
  {
    var1= var1 + 1;


    alert(var1);

  }
  
  輸出後會在提示框出現1,2,3,4...
  
  在函式（function）內，透過 var 所宣告的變數才能算是 Local Variable 區域變數，
  若沒有使用 var 關鍵字宣告，無論是在哪裡宣告的變數，都會屬於 Global Variable 全域變數的範疇。
  
```

onchange 事件

```

  onChange 事件可以用在像是 input text、textarea(多行的文字輸入欄位)、
  select option 等 HTML Form 元素上，當元素內容改變時就觸發 onChange Event來執行你所準備好的 JavaScript 程式碼

  function ShowStr(x){
     var Str=document.getElementById(x).value;
     alert(Str);
  }

  請隨意輸入幾個文字：<input type="text" id="Str" onchange="ShowStr(this.id)">

  當輸入完文字滑鼠移開文字欄位就會觸發onchange Event

```

if ， else if ， else 條件判斷式

```

  var Str = "B";
  
  if(Str == "A")
  {
    document.write("這是A");
  }
  else if(Str == "B")
  {
    document.write("這是B");
  }
  else
  {
     document.write("這是C");
  }

  輸出為 這是B。

```

99乘法

```

  利用for迴圈使變數產生數字

  輸出後會產生1~9

  再使兩個變數相乘

  for(i = 1 ; i < 10 ; i++)
  {
    console.log(i*j);
  }

```

js 獲取input value


```

   var name = document.getElementById("name").value;
              alert(name);
              
```

js 改變input的值

```

  <input type="text" id="txt" value="初始文字內容" size="30"/>
  <input type="button" value="更改文字內容" name="btn" onclick="c1();" />

　<script>
  
    var t=document.getElementById("txt");
    t.value="修改的文字內容"
    
　</script>
  
```

js 判斷 input 空值

```

if (document.getElementById('txt_1').value == '') 
{
　alert('數值請勿為空');
}
    
```

js 判斷 1~100 為(2)的倍數

```

for (i=1;i<=100;i++)
　{  
　　if (i%2 == 0)
　　{
　　　console.log(i);
　　}
　}
 
```

onkeyup 事件

```

  <input type="text" onkeyup="myFunction()">
  onkeyup 事件會在鍵盤被鬆開時發生。

```

js 判斷輸入是否為數字

```

　isNaN(numValue)
 
  EXP: if (isNaN(i) == false && isNaN(j) == false && i != ""  && j != "") //判斷是否為數字//判斷是否為空值*/

 
```

parseInt() 函数


```

  parseInt() 函数可解析一个字符串，并返回一个整数。


```

css 實現禁止選取頁面上的內容

```

  .class {
   -webkit-user-select: none;   /* for Chrome */
  }

```

js 修改和獲取p標籤裡面的內容

```

  function textModify()
    {
        var obj = document.getElementById("p");
        alert(obj.innerHTML);
        obj.innerHTML= "google coding"; 
    }
  function textModify2()
    {
        var obj = document.getElementById("p2");
        alert(obj.innerText);
        obj.innerText= "knowledge"; 
    }
    
  JavaScript 的 innerHTML 與 innerText 看似類似，但其實有很大的差異，
  對大多數設計師來說 innerHTML 應該比較熟悉，
  他是用來取得 HTML 元素或寫入字串到 HTML 網頁的語法，且 innerHTML 是 W3C 規定的標準寫法，
  而 innerText 則是除了可以用來取得 HTML 元素之外，還會把元素的 HTML 標籤去除掉，
  但 innerText 並非 W3C 所規定的標準寫法，
  而且僅適用於 IE 瀏覽器，這點非常重要。

```
 
input min屬性

 
```
 
  輸入 1980-01-01 之前的日期:
  <input type="date" name="bday" max="1979-12-31"><br>

  輸入 2000-01-01 之後的日期:
  <input type="date" name="bday" min="2000-01-02"><br>

  數量 (在1和5之間):
  <input type="number" name="quantity" min="1" max="5"><br>

  min 屬性規定 <input> 元素的最小值。

  提示：min 屬性與 max 屬性配合使用，可創建合法值範圍。

  注意：max 和 min 屬性適用於以下 input 類型：number、range、date、datetime、datetime-local、month、time 和 week。
  
```

Js isNAN()

```

  isNAN()函數用於檢查其參數是否 是非數字值
  isNaN(x)
  
  如果x是特殊的非數字值NAN(或者能被轉換為這樣的值),返回的值就是true。如果x是其他值,則返回false。
  
```

Js 實現點擊跳轉到指定位置

```

  1. 通過html錨點實現滾動定位到頁面指定位置(DIV)
  
  <a href="#abc">點擊跳轉</a>
  <div id="abc">將要跳轉到這裡</div>
  
  2.通過點擊button按鈕使用js實現滾動跳轉到頁面指定位置(DIV)
  
  <script>
  
  function onTopClick()
  {
  window.location.hash = "#abc";
  }
  
  </script>
  
  <input type="button" name="Submit" value="提交" onclick="onTopClick()">
  
  3.用animate屬性，當點擊錨點後，頁面滾動到相應的DIV。接著上面的代碼，具體添加如下代碼：
  
 css樣式：

  div {
        height: 800px;
        width: 400px;
        border: 2px solid black;
      }
  #container {
        position: fixed;
        margin:50px 500px;
      }
  .anchor {
       display: block;
       height: 91px;
       margin-top: -91px;
       visibility: hidden;
      }

 html頁面：
  
  <div id="container">
       <p id="p1">div1</p>
        <p id="p2">div2</p>
        <p id="p3">div3</p>
  </div>

    <div id="div1" class="anchor"></div>
    <div>div1</div>
    
    <div id="div2" class="anchor"></div>
    <div>div2</div>
    
    <div id="div3" class="anchor"></div>
    <div>div3</div>

 
  js代碼如下：

  <script type="text/javascript" src="http://code.jquery.com/jquery-1.8.0.min.js"></script>
  $(document).ready(function() {
    $("#p1").click(function() {
      $("html, body").animate({
        scrollTop: $("#div1").offset().top }, {duration: 500,easing: "swing"});
      return false;
    });

    $("#p2").click(function() {
      $("html, body").animate({
        scrollTop: $("#div2").offset().top }, {duration: 500,easing: "swing"});
      return false;
    });

    $("#p3").click(function() {
      $("html, body").animate({
        scrollTop: $("#div3").offset().top }, {duration: 500,easing: "swing"});
      return false;
    });
  });

```

Js substr() 字符串中抽取從 start 下標開始的指定數目的字符。

```

  stringObject.substr(start,length);
  
  例：時間補0
  var h = ('0'+d.getHours()).substr(-2);   
  
```

Js 每隔一秒就執行

```

  setTimeout("test()",1000);
  
```

Js 基本類 使用onClick 及 this取得id

```

  <script>
    function myMsg(myObj)
    {
    alert("id 為: " + myObj.id);
    }
  </script>
  
  <input type="button" id="myButton" name="mybutton" value="送出" onclick="myMsg(this)">

  結果顯示為：　id為myButton
  
```  

Js 獲取ID改變背景顏色

```

   function change_line(line) {

    console.log(line);

    var obj1 = document.getElementById("hour-h");
    var obj2 = document.getElementById("min-h");
    var obj3 = document.getElementById("second-h");

    if (line == 'line1') {
      obj1.style.backgroundColor = "#4158D0";
      obj2.style.backgroundColor = "#C850C0";
      obj3.style.backgroundColor = "#FFCC70";
    }

```

自定義 滑鼠樣式

```

  #mouse
  {
      border:1px solid black;
      cursor:url(wii.ani);
  }
  
  放在所需範圍之div裡，例如：整體網頁均要顯示此樣式就放在最大的div裡。
  
  
