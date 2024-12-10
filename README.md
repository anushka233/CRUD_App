<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Switch_Bulb</title>
</head>
<style>
    /* body{
        background-color: black;
    } */
    /* img{
        padding : 30px;
        margin-left : 600px;
        margin-top: 100px;
        
    } */
     .center{
        display: block;
        margin-left: auto;
        margin-right: auto;
        padding: 0%;
     }
     .btn{
        padding: 20px;
        background-color: green;
        text-align: center;
        width: 130px;
        font-family:Georgia, 'Times New Roman', Times, serif;
        font-size: 30px;
        margin-left: 700px;

     }
</style>
<body>
    <img id="bulb" src="off_bulb.jpg" alt="picture of off_bulb is here" class="center"height=500px width=400px>
    <btn id="toggleBtn" class="center btn">Turn On</btn>
</body>

<script>
    let btn = document.getElementById('toggleBtn')
    let bulb = document.getElementById('bulb')
    btn.addEventListener('click', toggleBulb)

    function toggleBulb(e){
        if(btn.textContent.includes('On')){
            bulb.src = "On_bulb.jpg";
            btn.textContent = "Turn Off";
        }
        else{
            bulb.src = "Off_bulb.jpg";
            btn.textContent = "Turn On";
        }
      
    }
    // document.addEventListener

</script>
</html>
