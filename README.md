<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Project: Scene change</title>
        <style>
        #leafers {
            position: absolute;
            top: 210px;
            left: 378px;
        }
        .dot {
                border-radius: 10px;
                background: black;
                position: absolute;
                width: 10px;
                height: 10px;
        }
        </style>
    </head>
    <body>

    <img src="https://www.kasandbox.org/programming-images/landscapes/beach-with-palm-trees.png">

    <img src="https://www.kasandbox.org/programming-images/avatars/leafers-seedling.png" id="leafers" value="PLAY"  onclick="play()" >
    <audio id="audio" src="sound.mp3" ></audio>
    
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
    <script>
        
              $("leafers).on("click", function(event) {
        var $dot = $("<div></div>");
        $dot.addClass("dot");
        $dot.css("position", "absolute");
        $dot.css("top", event.pageY + "px");
        $dot.css("left", event.pageX + "px");
        $dot.appendTo("body");
    });
    function play(){
    var audio = document.getElementById("audio");
    audio.play(); 
    }
    </script>
    </body>
</html>
    
  
