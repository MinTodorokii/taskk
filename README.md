<!DOCTYPE html>
<html>
    <head>
        <script>
            function goBack() {
              window.history.back()
            }
        </script>

        <meta charset="utf-8">
        <title>Project: Scene change</title>
        <style>
        #leafers {
            position: absolute;
            top: 210px;
            left: 378px;
        }
            
        </style>
       
    </head>
    <body>

        <button onclick="myFunction()">Try it</button>
            <p id="demo"></p>
  

       
    <img src="https://www.kasandbox.org/programming-images/landscapes/beach-with-palm-trees.png" value="PLAY"  onclick="play()">
    <audio id="audio" src="F:\sound.mp3" ></audio>


    <img src="https://www.kasandbox.org/programming-images/avatars/leafers-seedling.png" id="leafers" onmouseover="this.src='MIŠKO/yoongi.png'" onmouseout="this.src='https://www.kasandbox.org/programming-images/avatars/leafers-seedling.png'">
   
     
  
   
    
   
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
    <script>
        $("#leafers").on("click", function(event) {
            document.getElementById("leafers").width = "300";
  });
         </script>
        <script>
            function myFunction() {
              var txt;
              var person = prompt("Please enter your name:", "Harry Potter");
              if (person == null || person == "") {
                txt = "User cancelled the prompt.";
              } else {
                txt = "Hello " + person + "! How are you today?";
              }
              document.getElementById("demo").innerHTML = txt;
            }
            </script>
    
</html>
