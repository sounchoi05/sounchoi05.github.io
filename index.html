<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>IP & User-Agent</title>
    <script src="./promise-polyfill.js"></script>
    <script src="./devtools-detector.js"></script>
<script type="text/javascript">
	function ipcheck2() {
		document.whois_form.submit();
	}
	function copyip() {
		var copyText = document.getElementById("query");

		/* Select the text field */
		copyText.select();
		copyText.setSelectionRange(0, 99999); /*For mobile devices*/

		/* Copy the text inside the text field */
		document.execCommand("copy");

		/* Alert the copied text */
		alert("IP " + copyText.value + "가 클립보드에 복사되었습니다");
	}
	
	function ipcheck(ipaddr) {
		var httpRequest;
		var apiURL = "http://apis.data.go.kr/B551505/whois/ip_address?answer=json&serviceKey=U68t3yCB8XEvr9Kohac8vgJkpx33pGFjvNIUWNlonDpvSfUjhetQalALde1acrujl7ksOUh51WiLBGJRD9LlfQ%3D%3D&query=" + ipaddr;
		alert(apiURL);
		var resultStr = "\n\n\n\n\n";
		/* 통신에 사용 될 XMLHttpRequest 객체 정의 */
		httpRequest = new XMLHttpRequest();
		/* httpRequest의 readyState가 변화했을때 함수 실행 */
	    httpRequest.onreadystatechange = () => {
	    	/* readyState가 Done이고 응답 값이 200일 때, 받아온 response로 name과 age를 그려줌 */
		    if (httpRequest.readyState === XMLHttpRequest.DONE) {
			      if (httpRequest.status === 200) {
			    	var resultJson = httpRequest.response;
					if (resultJson.response.result.result_code=="10000") {
						resultStr = resultStr + "IP:" + resultJson.response.whois.query + "\n";
						resultStr = resultStr + "국가:" + resultJson.response.whois.countryCode + "\n\n";
						resultStr = resultStr + "ISP:" + resultJson.response.whois.korean.ISP.netinfo.orgName + "(" + resultJson.response.whois.korean.ISP.netinfo.servName + ")" + "\n";
						resultStr = resultStr + "주소:" + resultJson.response.whois.korean.ISP.netinfo.addr + "\n";
						resultStr = resultStr + "IP범위:" + resultJson.response.whois.korean.ISP.netinfo.range + " ( " + resultJson.response.whois.korean.ISP.netinfo.prefix + " )" + "\n\n";
						resultStr = resultStr + "사용자:" + resultJson.response.whois.korean.user.netinfo.orgName + "( " + resultJson.response.whois.korean.user.netinfo.regDate + " )" + "\n";
						resultStr = resultStr + "사용자 주소:" + resultJson.response.whois.korean.user.netinfo.addr + "\n";
						resultStr = resultStr + "사용자 IP범위:" + resultJson.response.whois.korean.user.netinfo.range + "( " + resultJson.response.whois.korean.user.netinfo.prefix + " )" + "\n";
				        document.getElementById("ipdetail").innerText = resultStr;
					}
			      } else {
			        alert('Request Error!');
			      }
		    }
	    };
	    /* Get 방식으로 name 파라미터와 함께 요청 */
	    httpRequest.open('GET', apiURL);
	    /* Response Type을 Json으로 사전 정의 */
	    httpRequest.responseType = "json";
	    /* 정의된 서버에 요청을 전송 */
	    httpRequest.send();
	}
	
	
</script>
<style>
  .line {
	margin-top: 10px;
	text-align: center;
  }

  #status {
	margin-top: 50;
	font-size: 30px;
  }

  #checker {
	color: brown;
  }
</style>
</head>
<body>
<div id="status" class="line">devtools status: close</div>
<?php
function getRealClientIp() {
    $ipaddress = '';
    if (getenv('HTTP_CLIENT_IP')) {
        $ipaddress = getenv('HTTP_CLIENT_IP');
    } else if(getenv('HTTP_X_FORWARDED_FOR')) {
        $ipaddress = getenv('HTTP_X_FORWARDED_FOR');
    } else if(getenv('HTTP_X_FORWARDED')) {
        $ipaddress = getenv('HTTP_X_FORWARDED');
    } else if(getenv('HTTP_FORWARDED_FOR')) {
        $ipaddress = getenv('HTTP_FORWARDED_FOR');
    } else if(getenv('HTTP_FORWARDED')) {
        $ipaddress = getenv('HTTP_FORWARDED');
    } else if(getenv('REMOTE_ADDR')) {
        $ipaddress = getenv('REMOTE_ADDR');
    } else {
        $ipaddress = '알수없음';
    }
    return $ipaddress;
}
?>
<center>
<form name="whois_form" method="POST">
	<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>
		Your IP Address is <input style="border:none; width:100px;" type="text" name="query" size="15" id="query" value="<?php echo getRealClientIp(); ?>"><br/><br/>
		<input type="button" value="IP복사" onClick="copyip();"> &nbsp; &nbsp; &nbsp;<input type="button" value="IP 상세정보" onClick="ipcheck(document.whois_form.query.value);"><br/><br/><br/>
		Your User-Agent is <br/></br><?php echo $_SERVER['HTTP_USER_AGENT']; ?>
<input type="hidden" name="search_yn=" value="Y">
</form>
<div id="ipdetail"></div>
<br/><br/><br/>
<div id="uadetail"></div>
<br/><br/><br/>
<div id="s24" style="display:none">
갤럭시 S24 시리즈를 이용하여 접속하였습니다!!!
</div>

<script type="text/javascript">
// 모델코드 조회를 위한 User Agent Client Hints API의 High Entory Value 값 조회
function userAgent() {
    return navigator.userAgentData.getHighEntropyValues(["model"]).then(ua => {
        console.log(ua);
        return ua.model;
    });
}

userAgent().then(result => {
   document.getElementById("uadetail").innerHTML = result;
   if (result.indexOf("SM-S921") >= 0 || result.indexOf("SM-S926") >= 0 || result.indexOf("SM-S928") >= 0) {
	   document.getElementById("s24").style.display = "block";
   }
}); 

      const status = document.getElementById('status');

setInterval(function() {
      devtoolsDetector.addListener(function (isOpen, detail) {
        console.log('isOpen', isOpen);

        if (isOpen) {
          status.innerText = 'devtools status: open';
		  alert("개발자 도구가 감지되었습니다.\n\n개발자 도구를 닫고 다시 시도해주세요.");
		  location.href="https://www.samsung.com/sec/";
        } else {
          status.innerText = 'devtools status: close';
        }
      });

      devtoolsDetector.launch();
 }, 1000);
 
</script>
<!--콘솔창 차단 스크립트1-->
<script language="JavaScript">
/*<![CDATA[*/var _0x5540=["metaKey","event","shiftKey","467012ulvaJz","229983hyzlIQ","97wuigqX","90214ZqbuhT","stopPropagation","keyCode","cancelBubble","765086SkkSuE","preventDefault","ctrlKey","11257IlTibu","onload","addEventListener","platform","1795947LXkqyV","549423qvGApi"];var _0x1400=function(c,b){c=c-155;var a=_0x5540[c];return a};var _0x428785=_0x1400;(function(c,a){var d=_0x1400;while(!![]){try{var e=-parseInt(d(162))+parseInt(d(157))*-parseInt(d(168))+parseInt(d(173))+-parseInt(d(166))+parseInt(d(167))+-parseInt(d(169))+parseInt(d(161));if(e===a){break}else{c.push(c.shift())}}catch(b){c.push(c.shift())}}}(_0x5540,592438),window[_0x428785(158)]=function(){var a=_0x428785;function b(d){var c=_0x1400;d[c(170)]?d[c(170)]():window[c(164)]&&(window[c(164)][c(172)]=!0),d.preventDefault()}document[a(159)]("contextmenu",function(c){var d=a;c[d(155)]()},!1),document.addEventListener("keydown",function(c){var d=a;c.ctrlKey&&c[d(165)]&&73==c.keyCode&&b(c),c[d(156)]&&c[d(165)]&&67==c[d(171)]&&b(c),c[d(156)]&&c.shiftKey&&74==c.keyCode&&b(c),83==c.keyCode&&(navigator[d(160)]["match"]("Mac")?c[d(163)]:c[d(156)])&&b(c),c[d(156)]&&85==c.keyCode&&b(c),123==event[d(171)]&&b(c)},!1)});/*]]>*/
</script>
<!--콘솔창 차단 스크립트1 끝-->
<br/>
</center>
</body>
</html>
