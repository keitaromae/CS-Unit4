```
<!DOCTYPE html>
<html>
<head>
<title>About me</title>
</head>
<body>

<style>
h1 {
	font-family: sans-serif ;
    font-color: rgb(255,255,255);
}

ul {
	font-family: sans-serif;
    line-height: 2em;

}

body { 
	background-color: coral;
    color: white;
}
.spinner {
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
          transform: translate(-50%, -50%);
  -webkit-transform-origin: center;
          transform-origin: center;
  width: 120px;
  height: 120px;
}
 
/* Loading テキスト */
.spinner span {
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
          transform: translate(-50%, -50%);
  font-size: 12px;
}

.spinner.type8 {
  border-radius: 50%;
  border-width: 8px;
  border-style: solid;
  border-color: #fff rgba(255, 255, 255, 0.12) rgba(255, 255, 255, 0.12);
  /* ローディング要素のアニメーションを指定 */
  -webkit-animation: spinner1_1 1.5s infinite linear forwards;
          animation: spinner1_1 1.5s infinite linear forwards;
}
.spinner.type8 span {
  /* Loading テキストのアニメーションを指定 */
  animation: spinner_loading_text 1.5s infinite linear forwards reverse;
}
 
/* ローディング要素のアニメーション内容 */
@-webkit-keyframes spinner1_1 {
  0% {
    -webkit-transform: translate(-50%, -50%) rotate(0);
            transform: translate(-50%, -50%) rotate(0);
  }
  100% {
    -webkit-transform: translate(-50%, -50%) rotate(360deg);
            transform: translate(-50%, -50%) rotate(360deg);
  }
}
 
@keyframes spinner1_1 {
  0% {
    -webkit-transform: translate(-50%, -50%) rotate(0);
            transform: translate(-50%, -50%) rotate(0);
  }
  100% {
    -webkit-transform: translate(-50%, -50%) rotate(360deg);
            transform: translate(-50%, -50%) rotate(360deg);
  }
}
 
/* Loading テキストのアニメーション内容 */
@-webkit-keyframes spinner_loading_text {
  0% {
    opacity: 1;
    -webkit-transform: translate(-50%, -50%) rotate(0deg);
            transform: translate(-50%, -50%) rotate(0deg);
  }
  50% {
    opacity: 0;
    -webkit-transform: translate(-50%, -50%) rotate(180deg);
            transform: translate(-50%, -50%) rotate(180deg);
  }
  100% {
    opacity: 1;
    -webkit-transform: translate(-50%, -50%) rotate(360deg);
            transform: translate(-50%, -50%) rotate(360deg);
  }
}
@keyframes spinner_loading_text {
  0% {
    opacity: 1;
    -webkit-transform: translate(-50%, -50%) rotate(0deg);
            transform: translate(-50%, -50%) rotate(0deg);
  }
  50% {
    opacity: 0;
    -webkit-transform: translate(-50%, -50%) rotate(180deg);
            transform: translate(-50%, -50%) rotate(180deg);
  }
  100% {
    opacity: 1;
    -webkit-transform: translate(-50%, -50%) rotate(360deg);
            transform: translate(-50%, -50%) rotate(360deg);
  }
}

</style>

<h1>Who is "Keitaro"?</h1>
<p><em>quick facts about me.</em></p>
<ul>
	<li><strong>'03:</strong> spawn in Okinawa <strong>Jan 26th</strong></li>
    <li><strong>'13:</strong> spawn in virtual minecraft world as "shukatus"</li>
    <li><strong>'17:</strong> Started playing Counter-Strike with my friends</li>
    <li><strong>'17:</strong> Graduated JHS start preparing for my huge journey.</li>
    <li><strong>'18:</strong> Joined <a href="https://uwcisak.jp">UWC ISAK Japan</a> and started my amazing life here!</li>
    <li><strong>'19:</strong> My first <a href="https://www.ibo.org">IB year</a> started.</li>
    <li><strong>'20~:</strong> Corona time</li>
</ul>


<div class="box">
  
  <div class="spinner type8">
    <span>Loading...</span>
  </div>
</div>



</body>
</html>
```
