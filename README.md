# FibonacciSequence
echo "# FibonacciSequence" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/rtrood22/FibonacciSequence.git
git push -u origin master


<!DOCTYPE html>
<html>
    <head>
        <title>Fibonacci Sequence (Rachel Winsor)</title>
    </head>
    <body>
    <div id = "userInterface" class="container">
            <button onclick="main()">Give me my Fibonacci Sequence</button>
            <div id = "inputPanel">
                <label for="n">Length of Fibonacci Sequence: </label>
                <input type="number" id="n" value="5"><br>
            </div>
        </div>
        <!-- Javascript -->
        <script type = "text/javascript">
        
        function main(){
        var fiblength = document.getElementById("n").value;
        var solution = new Array(fiblength);
        for (var i=0;i<fiblength;++i){
            solution[i]=fibSeq(i);
        }
        window.alert(solution);
        }
        function fibSeq(x){
          if(x==0){return 0;}
          if(x==1){return 1;}
          return fibSeq(x-1)+fibSeq(x-2);
        }
        
        
        </script>
    </body>
</html>
