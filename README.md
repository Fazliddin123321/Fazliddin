<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bir kichik o'yin 🙂</title>
<style>
body{
    margin:0;
    font-family:Arial,sans-serif;
    background:linear-gradient(135deg,#ff9a9e,#fad0c4);
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    text-align:center;
}
.box{
    background:#fff;
    padding:30px;
    border-radius:20px;
    width:90%;
    max-width:400px;
    box-shadow:0 10px 30px rgba(0,0,0,.2);
}
button{
    margin-top:20px;
    padding:12px 25px;
    border:none;
    border-radius:30px;
    background:#ff4d6d;
    color:#fff;
    font-size:18px;
    cursor:pointer;
}
h2{color:#ff4d6d;}
</style>
</head>
<body>

<div class="box">
    <h2 id="title">🎁 Siz uchun kichik syurpriz</h2>
    <p id="text">Tayyormisiz?</p>
    <button onclick="next()">Boshlash</button>
</div>

<script>
const steps=[
"1-bosqich ✅<br><br>Tabassumingizni tasavvur qildim 😊",
"2-bosqich ✅<br><br>Yana bitta tugmani bosing.",
"3-bosqich ✅<br><br>Eng qiziq joyiga oz qoldi...",
"4-bosqich ✅<br><br>Oxirgi qadam!",
"🌹 <h2>Chiroyli qizning xonimlari pishtimi? 😊❤️</h2>"
];

let i=0;
function next(){
    document.getElementById("text").innerHTML=steps[i];
    i++;
    if(i>=steps.length){
        document.querySelector("button").style.display="none";
    }
}
</script>

</body>
</html>
