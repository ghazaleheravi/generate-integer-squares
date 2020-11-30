# generate-integer-squares
<!doctype html>
    <html lang="en-us dir="ltr">
        <head>

           <meta charset="uft-8">
           <title>squares</title>
        
        </head>
        <body>

            <label for="int">Enter number:</label>
            <input id="int" type="text">
            <button>generate integer squares</button>
            <p>output:</p>
            
            <script>

                let input = document.querySelector('#int');
                let button = document.querySelector('button');
                let output = document.querySelector('p');

                button.addEventListener('click',square);

                function square(){
                    let num = input.value;
                    let result;
                    input.value = '';
                    input.focus();
                   
                   let sqrtNum = Math.floor(Math.sqrt(num));
                   for(let i=1;i<=sqrtNum;i++){
                       if(i<=sqrtNum){
                          result = i*i; 
                          output.textContent += result + ' ';
                         
                       }
                    }
                 }

            </script>
        </body>
    </html>    

