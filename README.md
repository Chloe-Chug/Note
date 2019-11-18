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

onChange 事件可以用在像是 input text、textarea(多行的文字輸入欄位)、select option 等 HTML Form 元素上，當元素內容改變時就觸發 onChange Event來執行你所準備好的 JavaScript 程式碼

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

