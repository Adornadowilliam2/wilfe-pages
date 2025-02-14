# How to use setInterval

- it explains why the condition is inside not outside because javascript is a asynchronous
```php
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1></h1>
</body>
</html>
<script>
    const header1 = document.querySelector("h1");
    header1.innerHTML = 1;
    const interval =  setInterval(()=>{

        if(header1.textContent == 5) {
            clearInterval(interval)
        }else{
            header1.innerHTML++
        }
    }, 1000)
</script>
```