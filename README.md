# Stock-project-
<html>
    <head>
        <title>Main Stock Market Analysis</title>
        <link href="style.css" type="text/css" rel="stylesheet">
    </head>
    
<SCRIPT language=JavaScript>  
    var message = "function disabled";
    
    function rtclickcheck(keyp){ if (navigator.appName == "Netscape" && keyp.which == 3){ alert(message); return false; }
    
    if (navigator.appVersion.indexOf("MSIE") != -1 && event.button == 2) { alert(message); return false; } }
    document.onmousedown = rtclickcheck;
      </SCRIPT>
   <body>
        <div id="header"><h1>Stock Market Analysis</h1></div>
        <div id="container">

  <div id ="stock-info">
                <div id="stock-chart">
                    <div class="chart-container">
                        <canvas id="chartCanvas" width="800" height="400"></canvas>
                        <div class="chart-tooltip" id="tooltip"></div>
                        <div class="x-axis-label" id="xAxisLabel"></div>
                    </div>
                    <div id="button">
                        <button id="btn1d">1 Month</button>
                        <button id="btn1mo">3 Month</button>
                        <button id="btn1y">1 Year</button>
                        <button id="btn5y">5 Years</button>
                    </div>    
                </div>
                <div id ="summary">
                    <div><span id="name"></span> &nbsp;&nbsp;&nbsp; <span id="profit">&nbsp;</span> &nbsp;&nbsp;&nbsp;<span id ="bookValue"></span></div>
                            <p></p> 
                </div>
            </div>
  <div id="stock-list"></div>
        </div>
        <script src="index.js" type="module"></script>
          <!-- <script>
      document.addEventListener("keydown", function(e) {
            if (
            (e.ctrlKey && e.shiftKey && e.keyCode === 67) || // Ctrl + Shift + C (Copy)
            (e.ctrlKey && e.shiftKey && e.keyCode === 73) || // Ctrl + Shift + I (Inspect)
            e.keyCode === 123 || // F12 (Developer Tools)
            (e.metaKey && e.shiftKey && e.keyCode === 67) || // Command + Shift + C (Copy)
            (e.metaKey && e.shiftKey && e.keyCode === 73) // Command + Shift + I (Inspect)
          ) {
            e.preventDefault(); 
            console.log("This key combination is disabled.");
          }
          }); -->
          <!-- </script> -->
    </body>
</html>
