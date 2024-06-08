# JS-important-concepts
1. Implemented Debouncing concept
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>simple calculation</title>
</head>
<body>
    <input type="text" name="searchbar" placeholder="Search anything.." oninput="searchbar()">
    <script> 
    let val = 0;
    function outer(){
        console.log("Request",++val);
    }
    let timer;
    function searchbar(){
        clearTimeout(timer);
        timer = setTimeout(function(){
            outer();
        },1000);
    }
    </script>
</body>
</html>
