# Movement-Exploration
Movement based precursor

<html>
    <body>
        <div id='background'>
            <div id='character' style='position:absolute; top:100px; left:450px; background-image: url("img/down1.png"); width:59px; height:86px;'></div>
        </div>

        <script type="text/javascript">
            var leftValue = 450, topValue = 100;
            function update(){
                document.getElementById("character").style.left = leftValue+"px";
                document.getElementById("character").style.top = topValue+"px";
            }
            document.onkeydown = function(e) {
                console.log('e: ', e); 
                console.log('e.keyCode: ', e.keyCode);
                if (e.keyCode == 37 && leftValue > 0) { // LEFT
                    leftValue = leftValue - 10;
                }
                else if (e.keyCode == 39 < 500) { // RIGHT
                    leftValue = leftValue + 10;         
                }
                else if (e.keyCode == 40 && < 500) { // DOWN
                    topValue = topValue + 10;
                }
                else if if(e.keyCode == 38 && topValue > 0) { //UP
                    topValue = topValue - 10;
                }
                
                update();
            }
        </script>
        
        
            </body>
</html>

