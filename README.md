<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Мое портфолио(К.К.)
  <br>
  </title>
  <style>
    body {
     font-family: 'Roboto', sans-serif;
     max-width: 800px; 
     margin: 0 auto;   
     padding: 20px;    
     line-height: 1.5; 
     background-color: #f5f5f5; 
    }
    h1 {
      color: #2c3e50;   
      text-align: center; 
    }
    .card {
      background: white;
      padding: 20px;
      margin: 20px 0;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1); 
    }
    .photo-right {
    float: right;       
    margin-left: 10px; 
    margin-bottom: 10px;
    }
    .photo-left {
    float: left;       
    margin-right: 20px; 
    margin-bottom: 5px;
    margin-top: 15px;
    }
    .content {
    flex: 1;
    margin-bottom: 200px; 
    }
  </style>
</head>
<body>
  <h1>Мое портфолио😝</h1>
  <div class="card">
    <img src="assets/My photo.jpg" alt="Моё фото" class="photo-right"  width="130" style="border-radius: 10%;">
    <h2>Обо мне</h2>
    <p>  Привет! Я учусь создавать красивые сайты с помощью кода :) 
    <br> Я начинающий веб-дизайнер и пока мало что умею, но обещаю стараться и учиться новому!))</p>
    <div style="clear: both;"></div>
  </div>
  <div class="card">
    <h2>Мои контакты</h2>
        <br>
        <img src="386659_mailru_mail.ru_icon.png" alt="Mail.ru" class="photo-left" width="25">
        <p><i class="fas fa-envelope"></i> Kovalenkova_k_kurgan@mail.ru</p>
<a href="mailto:Kovalenkova_k_kurgan@mail.ru">Написать письмо</a>
        <br><img src="2613278_chat_chatting_cloud based_messenger_social media_icon.png" alt="Tg" class="photo-left" width="25">
        <p><i class="fab fa-telegram"></i> @Hungry_for_ever</p>
<a href="https://t.me/Hungry_for_ever" target="_blank" rel="noopener noreferrer">
 Перейти в телеграмм
</a>
  </div>
<div class="card">
    <h2>Моя группа поддержки</h2>
    <div class="support-team">
        <div class="person">
            <img src="friend1.jpg" alt="Мой товарищ Тоша" width="250">
            <img src="photo_5210942773967056513_y.jpg" alt="Тряпочка" width="250">
            <img src="friend2.jpg" alt="Ужасный хищник!" width="250">
            <p>Тоша: <i>"Мур-р-р!"</i></p>
        </div>
    </div>
</div>
<div class="card">
<p id="compliment">Нажми на кнопку — получишь комплимент!</p>
<button onclick="generateCompliment()">✨ Получить комплимент</button>
<script>
function generateCompliment() {
    const compliments = [
        "Тот, кто сейчас читает этот текст, получит удачу на весь день!",
        "Когда ты проходишь мимо, цветы поворачиваются посмотреть на тебя ещё раз",
        "У тебя красивая улыбка. Почаще дари ее миру!",
        "Твоя доброта делает людей счастливее",
        "Твои глаза бездонны, как Байкал!",
        "Твой образ сегодня необычайно прекрасен",
        "Вау, тебе очень идет эта прическа!",
    ];
    const randomCompliment = compliments[Math.floor(Math.random() * compliments.length)];
    document.getElementById('compliment').innerText = randomCompliment;
}
</script>
</div>
<div style="text-align: center;">
    <br><button id="no-click" class="btn-danger">🚨 НЕ НАЖИМАТЬ!</button>
    <p id="hack-message" style="display: none; margin: 10px auto 0; max-width: 300px; color: red; font-weight: bold;">
       Вас взломали! 💻
    </p>
    <p id="secret-message" style="display: none; margin: 10px auto 0; max-width: 300px;">
        А я предупреждала! 😈
    </p>
</div>

<script>
document.getElementById('no-click').addEventListener('click', function() {
    document.getElementById('secret-message').style.display = 'block';
    document.getElementById('hack-message').style.display = 'block';
    this.textContent = "☠️ Всё пропало!"; 
    this.style.background = "#000"; 
});
</script>

<style>
.btn-danger {
    background: #e74c3c;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
    display: block;
    margin: 0 auto;
    transition: all 0.3s; 
}
.btn-danger:hover {
    background: #c0392b;
}
</style>
<style>
.support-team {
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
}
.person {
    text-align: center;
}
.person img {
    border-radius: 5%;
}
</style>
</body>
</html>
