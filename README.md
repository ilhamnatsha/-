<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>مملكة الهام الجميلة 🎀</title>
<style>
  body {
    font-family: 'Arial', sans-serif;
    background: #fff0f9;
    color: #444;
    margin: 0; padding: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 100vh;
  }
  header {
    background: #ffb6c1;
    width: 100%;
    padding: 25px 0;
    color: white;
    font-size: 32px;
    font-weight: bold;
    text-align: center;
    box-shadow: 0 4px 10px #ff9ac1;
  }
  main {
    flex: 1;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 25px;
    padding: 40px 20px;
    max-width: 700px;
    width: 100%;
  }
  .card {
    background: white;
    border-radius: 20px;
    box-shadow: 0 0 15px #ffbfdc;
    width: 200px;
    height: 150px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    transition: transform 0.3s ease;
    font-weight: bold;
    color: #c2185b;
    font-size: 22px;
    text-align: center;
  }
  .card:hover {
    transform: scale(1.08);
    box-shadow: 0 0 25px #ff69b4;
  }
  footer {
    background: #ffb6c1;
    width: 100%;
    padding: 12px 0;
    color: white;
    font-size: 16px;
    text-align: center;
    box-shadow: 0 -4px 10px #ff9ac1;
  }
</style>
</head>
<body>

<header>مملكة الهام الجميلة 🎀</header>

<main>
  <div class="card" onclick="goTo('banat-game.html')">أسئلة بناتية كيوت 💖</div>
  <div class="card" onclick="goTo('puzzle-game.html')">لعبة ترتيب الصور 🧩</div>
  <div class="card" onclick="goTo('tasks.html')">قائمة المهام اليومية 📝</div>
  <div class="card" onclick="goTo('diary.html')">دفتر الذكريات 📔</div>
  <div class="card" onclick="goTo('calendar.html')">التقويم 📅</div>
  <div class="card" onclick="goTo('motivations.html')">كلمات محفزة ✨</div>
  <div class="card" onclick="goTo('drawing.html')">صفحة الرسم 🎨</div>
</main>

<footer>© 2025 مملكة الهام | كل الحقوق محفوظة 🎀</footer>

<script>
  function goTo(page) {
    window.location.href = page;
  }
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>🎀 لعبة الأسئلة البناتية اللطيفة</title>
<style>
  body {
    font-family: 'Arial', sans-serif;
    background: #fff0f9;
    color: #444;
    padding: 20px;
  }
  header {
    background: #ffb6c1;
    color: white;
    text-align: center;
    padding: 15px;
    font-size: 26px;
    font-weight: bold;
    border-radius: 12px;
  }
  .question-box {
    background: white;
    border-radius: 15px;
    padding: 20px;
    margin: 20px auto;
    max-width: 500px;
    box-shadow: 0 0 12px #ffbfdc;
  }
  .question-text {
    font-size: 22px;
    color: #c2185b;
    margin-bottom: 15px;
  }
  input[type="text"] {
    width: 100%;
    padding: 12px;
    font-size: 18px;
    border: 2px solid #ffc0cb;
    border-radius: 10px;
    margin-bottom: 15px;
    box-sizing: border-box;
  }
  button {
    background-color: #ff69b4;
    color: white;
    border: none;
    font-weight: bold;
    font-size: 18px;
    padding: 12px;
    border-radius: 15px;
    cursor: pointer;
    width: 100%;
  }
  .response {
    margin-top: 15px;
    font-size: 20px;
    color: #c2185b;
    font-weight: bold;
    min-height: 40px;
    min-width: 100%;
    text-align: center;
  }
</style>
</head>
<body>

<header>🎀 لعبة الأسئلة البناتية اللطيفة</header>

<div class="question-box">
  <div class="question-text" id="question">مرحبا يا أميرتي! اضغطي "السؤال التالي" لبدء اللعبة 💖</div>
  <input type="text" id="answer" placeholder="اكتبي جوابك هنا..." />
  <button onclick="submitAnswer()">جاوبيني يا أميرتي</button>
  <button onclick="nextQuestion()" style="margin-top:10px; background:#ffc0cb; color:#c2185b;">السؤال التالي</button>
  <div class="response" id="response"></div>
</div>

<script>
  const questions = [
    "كم عمرك يا جميلتي؟ 🐥",
    "شو لونك المفضل؟ 🎀",
    "شو أكتر شيء بتحبيه تعمليه بالوقت الفراغ؟ 🌷",
    "مين أعز صديقة عندك؟ 💕",
    "شو أكتر أكلة بتحبيها؟ 🍰",
    "كيف بتوصفين شخصيتك؟ ✨",
    "لو صار عندك قوة خارقة، شو بتكون؟ 🦸‍♀️",
    "شو حلمك الكبير؟ 🌟",
    "شو أغلى شيء عندك؟ 💖",
    "لو تقدري تروحي أي مكان، وين؟ ✈️"
  ];

  const responses = [
    {
      "10": "عمر العسل والرقة يا عسل 🍯",
      "11": "أنتِ في أجمل مرحلة شباب 💖",
      "12": "عمر التفتح والفرح 🌸",
      "13": "يا سلام! عمرك روعة كل سنة تزيدي تألقي! ✨",
      "14": "العمر جميل وياك، وقلبي معاك 💗",
      "15": "15 سنة جمال ونعومة وطيبة الدنيا كلها 💕",
      "default": "كل سنة وأنتِ أحلى وأجمل 🌷"
    },
    {
      "زهري": "يا روحي، اللون اللي بيعكس رقتك وجمالك 💕",
      "أزرق": "لون السماء الهادية، زي قلبك الطيب 💙",
      "أخضر": "لون الطبيعة والحياة، مثلك تمامًا 🌿",
      "أصفر": "لون الشمس اللي بينير أيامك ☀️",
      "أحمر": "لون القلب والعاطفة، يا قلبي المحب ❤️",
      "أبيض": "لون النقاء والصفاء، زي روحك الطاهرة 🤍",
      "أسود": "لون الغموض والأناقة، ملكة بكل معنى الكلمة 🖤",
      "default": "لونك مميز وجميل مثلك! 🌈"
    },
    {
      "القراءة": "القراءة غذاء العقل والروح، يا فطنة القمر 🌙",
      "الرسم": "موهبة فنية نادرة، يا ملكة الألوان 🎨",
      "الرياضة": "قوية ونشيطة، هذا اللي بحب أشوفه! 💪",
      "السفر": "روحك مغامرة ومحبة لاكتشاف الجديد ✈️",
      "الطبخ": "طباخة ماهرة، رائحة الأكل تسحر القلوب 🍲",
      "default": "كل نشاط بتعمليه يضيف لجمالك سحر 💫"
    },
    {
      "مريم": "مريم صديقتك الوفية واللطيفة، يا محظوظة 💕",
      "سارة": "سارة قلبها كبير ويحبك بجنون 💖",
      "نور": "نور تنير حياتك وتملأها حبًا 🌟",
      "ليلى": "ليلى ملاك برقة وحنية يا غالية 🌷",
      "default": "الصداقة الحلوة هدية العمر 💝"
    },
    {
      "البيتزا": "بيتزا لذيذة زي قلبك الحنون 🍕",
      "الكنافة": "حلاوة الكنافة على طيبتك يا روحي 🍯",
      "الشاورما": "شاورما بطعم الذكريات الحلوة 🥙",
      "المندي": "مندي شهي مثل طيبة قلبك 🍗",
      "default": "كل الأكلات حلوة لما تأكليها أنتِ 💖"
    },
    {
      "لطيفة": "يا رقة المشاعر وجمال القلب 💖",
      "جريئة": "شجاعة وقوية، أميرة بكل معنى الكلمة! 👑",
      "خجولة": "رقيقة وهادئة، مثل نسمة نسيم 🌸",
      "مرحة": "ضحكتك أجمل صوت في الدنيا 🎉",
      "default": "شخصيتك مميزة وفريدة 💫"
    },
    {
      "الطيران": "طيري عالي فوق الغيوم، يا حرّة روحي! 🕊️",
      "الاختفاء": "غموض وسحر، ملكة الظل 👑",
      "السرعة": "رشيقة وخفيفة، مثل النسمة 💨",
      "التخاطر": "قوة عقلية وعاطفية عظيمة 💭",
      "default": "أي قوة تختاريها رح تكون رائعة مثلك! 🌟"
    },
    {
      "السفر": "السفر يوسع الأفق ويحقق الأحلام 🌍",
      "النجاح": "النجاح تاج على رأسك يا ملكة 💎",
      "الزواج": "حب وعائلة جميلة، أجمل أمنيات الحياة 💕",
      "التعليم": "العلم نور، وأنتِ نور متلألئ! 📚",
      "default": "أحلامك كبيرة وجميلة يا فاتنة 💖"
    },
    {
      "العائلة": "العائلة هي كنز الحياة الحقيقي 💝",
      "الصداقة": "الصداقة أغلى من الذهب 💛",
      "الصحة": "الصحة تاج على الرأس، دمتِ بخير! 🌸",
      "النجاح": "نجاحك هو فرح قلبي وسعادتي 💕",
      "default": "أغلى شيء هو أنتِ بكل ما فيكِ 💖"
    },
    {
      "باريس": "باريس مدينة الحب والرومانسية، مثلك تمامًا ❤️",
      "دبي": "دبي مدينة السحر والحداثة 🌆",
      "مصر": "مصر بلد الحضارة والتاريخ العظيم 🏺",
      "طوكيو": "طوكيو تجمع بين الحداثة والتقاليد 🏯",
      "default": "أي مكان تختاريه رح يكون مميز معكِ 💫"
    }
  ];

  let currentQuestion = -1;

  function nextQuestion() {
    currentQuestion++;
    if (currentQuestion >= questions.length) {
      currentQuestion = 0;
    }
    document.getElementById("question").textContent = questions[currentQuestion];
    document.getElementById("answer").value = "";
    document.getElementById("response").textContent = "";
  }

  function submitAnswer() {
    const answer = document.getElementById("answer").value.trim();
    if (!answer) {
      document.getElementById("response").textContent = "رجاءً اكتبي جوابك يا أميرتي 💖";
      return;
    }

    let reply = "";
    const responseSet = responses[currentQuestion];

    for (const key in responseSet) {
      if (key.toLowerCase() === answer.toLowerCase()) {
        reply = responseSet[key];
        break;
      }
    }
    if (!reply) {
      reply = responseSet["default"];
    }
    document.getElementById("response").textContent = reply;
  }
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>🎀 لعبة ترتيب الصور البناتية 🧩</title>
<style>
  body {
    font-family: 'Arial', sans-serif;
    background: #fff0f9;
    color: #444;
    padding: 20px;
    text-align: center;
  }
  header {
    background: #ffb6c1;
    color: white;
    padding: 15px;
    font-size: 26px;
    font-weight: bold;
    border-radius: 12px;
    margin-bottom: 20px;
  }
  #group-select {
    margin-bottom: 20px;
    font-size: 18px;
    padding: 10px;
    border-radius: 10px;
    border: 2px solid #ffc0cb;
    background: #fff0f9;
    color: #c2185b;
    cursor: pointer;
  }
  #puzzle-container {
    max-width: 360px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 5px;
  }
  .piece {
    width: 110px;
    height: 110px;
    border-radius: 12px;
    box-shadow: 0 0 8px #ffbfdc;
    background-size: cover;
    background-position: center;
    cursor: pointer;
    border: 3px solid transparent;
    transition: border-color 0.3s;
  }
  .piece.selected {
    border-color: #ff69b4;
  }
  #message {
    margin-top: 20px;
    font-size: 20px;
    color: #c2185b;
    font-weight: bold;
  }
  button {
    margin-top: 15px;
    padding: 12px 20px;
    font-size: 18px;
    border: none;
    border-radius: 15px;
    background-color: #ff69b4;
    color: white;
    cursor: pointer;
    font-weight: bold;
  }
</style>
</head>
<body>

<header>🎀 لعبة ترتيب الصور البناتية 🧩</header>

<select id="group-select" onchange="loadGroup()">
  <option value="-1">اختر مجموعة الصور 🌸</option>
  <option value="0">مجموعة الفراشات 🦋</option>
  <option value="1">مجموعة الكيكات 🍰</option>
  <option value="2">مجموعة الدباديب 🐻</option>
</select>

<div id="puzzle-container"></div>

<button onclick="checkSolution()">تحقق من الترتيب</button>

<div id="message"></div>

<script>
  const groups = [
    {
      name: "مجموعة الفراشات 🦋",
      images: [
        "https://i.imgur.com/nUdxPz9.jpg",
        "https://i.imgur.com/2uLGG6J.jpg",
        "https://i.imgur.com/sOYDtv0.jpg",
        "https://i.imgur.com/MogK0kp.jpg",
        "https://i.imgur.com/G3Ykk3Z.jpg",
        "https://i.imgur.com/aF4bErJ.jpg"
      ]
    },
    {
      name: "مجموعة الكيكات 🍰",
      images: [
        "https://i.imgur.com/Ih2b6XG.jpg",
        "https://i.imgur.com/TTdfJ5c.jpg",
        "https://i.imgur.com/kykR3zC.jpg",
        "https://i.imgur.com/6GSn4Qz.jpg",
        "https://i.imgur.com/QPBnMxo.jpg",
        "https://i.imgur.com/n35pqHK.jpg"
      ]
    },
    {
      name: "مجموعة الدباديب 🐻",
      images: [
        "https://i.imgur.com/2jP4mwF.jpg",
        "https://i.imgur.com/6d8B9tD.jpg",
        "https://i.imgur.com/pWVEGdl.jpg",
        "https://i.imgur.com/8Wyw9r9.jpg",
        "https://i.imgur.com/GsC0d3Z.jpg",
        "https://i.imgur.com/HWqeZr6.jpg"
      ]
    }
  ];

  let selectedGroupIndex = -1;
  let pieces = [];
  let selectedPieceIndex = null;

  function shuffle(array) {
    for (let i = array.length -1; i > 0; i--) {
      const j = Math.floor(Math.random() * (i +1));
      [array[i], array[j]] = [array[j], array[i]];
    }
  }

  function loadGroup() {
    const select = document.getElementById('group-select');
    selectedGroupIndex = parseInt(select.value);
    if (isNaN(selectedGroupIndex) || selectedGroupIndex < 0) {
      document.getElementById('puzzle-container').innerHTML = '';
      document.getElementById('message').textContent = '';
      return;
    }
    pieces = groups[selectedGroupIndex].images.map((src, index) => ({src, index}));
    shuffle(pieces);
    selectedPieceIndex = null;
    renderPieces();
    document.getElementById('message').textContent = 'اختاري قطعتين لتبديلهما لترتيب الصور 🎀';
  }

  function renderPieces() {
    const container = document.getElementById('puzzle-container');
    container.innerHTML = '';
    pieces.forEach((piece, idx) => {
      const div = document.createElement('div');
      div.className = 'piece';
      div.style.backgroundImage = `url(${piece.src})`;
      div.dataset.index = idx;
      div.onclick = () => selectPiece(idx);
      if (idx === selectedPieceIndex) {
        div.classList.add('selected');
      }
      container.appendChild(div);
    });
  }

  function selectPiece(idx) {
    if (selectedPieceIndex === null) {
      selectedPieceIndex = idx;
    } else if (selectedPieceIndex === idx) {
      selectedPieceIndex = null;
    } else {
      [pieces[selectedPieceIndex], pieces[idx]] = [pieces[idx], pieces[selectedPieceIndex]];
      selectedPieceIndex = null;
      renderPieces();
    }
  }

  function checkSolution() {
    for (let i = 0; i < pieces.length; i++) {
      if (pieces[i].index !== i) {
        document.getElementById('message').textContent = 'للأسف الترتيب غير صحيح بعد، جربي مرة تانية يا أميرة 🌸';
        return;
      }
    }
    document.getElementById('message').textContent = 'واااو، مبروك يا أميرتي! رتبتي الصور صح 🎉💕';
  }
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>🎀 لعبة الاختيار العشوائي</title>
<style>
  body {
    font-family: 'Arial', sans-serif;
    background: #fff0f9;
    color: #c2185b;
    text-align: center;
    padding: 30px 20px;
  }
  header {
    background: #ffb6c1;
    padding: 15px;
    border-radius: 12px;
    font-size: 26px;
    font-weight: bold;
    color: white;
    margin-bottom: 30px;
  }
  input, button {
    font-size: 18px;
    padding: 12px;
    border-radius: 12px;
    border: 2px solid #ffc0cb;
    width: 80%;
    max-width: 400px;
    margin-bottom: 20px;
  }
  button {
    background: #ff69b4;
    color: white;
    border: none;
    cursor: pointer;
    font-weight: bold;
    transition: background 0.3s;
  }
  button:hover {
    background: #ff4d94;
  }
  #result {
    font-size: 24px;
    font-weight: bold;
    margin-top: 25px;
    min-height: 40px;
  }
</style>
</head>
<body>

<header>🎀 لعبة الاختيار العشوائي</header>

<p>اكتبي خياراتك مفصولة بفاصلة <code>,</code> وخلّي اللعبة تختار لك شي حلو 💖</p>
<input type="text" id="choicesInput" placeholder="مثلاً: بيتزا, آيس كريم, شكولاتة, بسكويت" />
<br/>
<button onclick="chooseRandom()">اختاري لي يا أميرتي!</button>

<div id="result"></div>

<script>
  function chooseRandom() {
    const input = document.getElementById('choicesInput').value.trim();
    if (!input) {
      document.getElementById('result').textContent = "رجاءً اكتبي خيارات يا أميرتي 💖";
      return;
    }
    const choices = input.split(',').map(c => c.trim()).filter(c => c !== "");
    if (choices.length === 0) {
      document.getElementById('result').textContent = "الخيارات غير صالحة، جرّبي مرة ثانية 💫";
      return;
    }
    const randomIndex = Math.floor(Math.random() * choices.length);
    const chosen = choices[randomIndex];
    document.getElementById('result').textContent = `أنا اخترت لكِ: 🌸 ${chosen} 🌸`;
  }
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>🎀 لعبة سودوكو بناتية</title>
<style>
  body {
    font-family: 'Arial', sans-serif;
    background: #fff0f9;
    color: #c2185b;
    text-align: center;
    padding: 20px;
  }
  header {
    background: #ffb6c1;
    color: white;
    padding: 15px;
    font-size: 26px;
    font-weight: bold;
    border-radius: 12px;
    margin-bottom: 20px;
  }
  #sudoku-grid {
    margin: 0 auto;
    border: 4px solid #ff69b4;
    border-radius: 15px;
    width: 360px;
    height: 360px;
    display: grid;
    grid-template-columns: repeat(9, 1fr);
    grid-template-rows: repeat(9, 1fr);
    gap: 2px;
  }
  input[type="number"] {
    width: 100%;
    height: 100%;
    font-size: 20px;
    text-align: center;
    border: 1px solid #ffc0cb;
    border-radius: 8px;
    outline: none;
    background: #fff0f9;
    color: #c2185b;
  }
  input[type="number"]:focus {
    border-color: #ff69b4;
    background: #ffe4ec;
  }
  /* تمييز المربعات 3x3 */
  .block-border {
    border: 2px solid #ff69b4;
  }
  #controls {
    margin-top: 15px;
  }
  button {
    background: #ff69b4;
    color: white;
    font-weight: bold;
    padding: 12px 20px;
    margin: 5px;
    border: none;
    border-radius: 15px;
    cursor: pointer;
    font-size: 18px;
    transition: background 0.3s;
  }
  button:hover {
    background: #ff4d94;
  }
  #message {
    margin-top: 15px;
    font-weight: bold;
    color: #c2185b;
    min-height: 24px;
  }
</style>
</head>
<body>

<header>🎀 لعبة سودوكو بناتية</header>

<div id="sudoku-grid"></div>

<div id="controls">
  <button onclick="startGame()">ابدأي اللعبة</button>
  <button onclick="checkSolution()">تحققي من الحل</button>
  <button onclick="showSolution()">أريني الحل</button>
</div>

<div id="message"></div>

<script>
  // لغز سودوكو بسيط (0 يعني خانات فارغة)
  const puzzle = [
    5, 3, 0, 0, 7, 0, 0, 0, 0,
    6, 0, 0, 1, 9, 5, 0, 0, 0,
    0, 9, 8, 0, 0, 0, 0, 6, 0,
    8, 0, 0, 0, 6, 0, 0, 0, 3,
    4, 0, 0, 8, 0, 3, 0, 0, 1,
    7, 0, 0, 0, 2, 0, 0, 0, 6,
    0, 6, 0, 0, 0, 0, 2, 8, 0,
    0, 0, 0, 4, 1, 9, 0, 0, 5,
    0, 0, 0, 0, 8, 0, 0, 7, 9
  ];

  // الحل الكامل للسودوكو
  const solution = [
    5,3,4,6,7,8,9,1,2,
    6,7,2,1,9,5,3,4,8,
    1,9,8,3,4,2,5,6,7,
    8,5,9,7,6,1,4,2,3,
    4,2,6,8,5,3,7,9,1,
    7,1,3,9,2,4,8,5,6,
    9,6,1,5,3,7,2,8,4,
    2,8,7,4,1,9,6,3,5,
    3,4,5,2,8,6,1,7,9
  ];

  const grid = document.getElementById('sudoku-grid');
  const message = document.getElementById('message');

  function createGrid() {
    grid.innerHTML = '';
    for (let i = 0; i < 81; i++) {
      const input = document.createElement('input');
      input.type = 'number';
      input.min = 1;
      input.max = 9;
      input.maxLength = 1;
      input.dataset.index = i;
      input.oninput = () => {
        if (input.value.length > 1) input.value = input.value.slice(0,1);
        if (input.value < 1 || input.value > 9) input.value = '';
      };
      // تمييز الحدود للكتل 3x3
      const row = Math.floor(i / 9);
      const col = i % 9;
      if (col === 2 || col === 5) input.style.borderRight = '3px solid #ff69b4';
      if (col === 3 || col === 6) input.style.borderLeft = '3px solid #ff69b4';
      if (row === 2 || row === 5) input.style.borderBottom = '3px solid #ff69b4';
      if (row === 3 || row === 6) input.style.borderTop = '3px solid #ff69b4';
      grid.appendChild(input);
    }
  }

  function startGame() {
    createGrid();
    for(let i=0; i<81; i++) {
      const input = grid.children[i];
      if (puzzle[i] !== 0) {
        input.value = puzzle[i];
        input.disabled = true;
        input.style.backgroundColor = '#ffd6e7';
        input.style.color = '#c2185b';
        input.style.fontWeight = 'bold';
      } else {
        input.value = '';
        input.disabled = false;
        input.style.backgroundColor = '#fff0f9';
        input.style.color = '#c2185b';
        input.style.fontWeight = 'normal';
      }
    }
    message.textContent = 'ابدأي بحل اللغز، يا أميرة القلب! 💖';
  }

  function checkSolution() {
    let correct = true;
    for(let i=0; i<81; i++) {
      const val = parseInt(grid.children[i].value);
      if (val !== solution[i]) {
        correct = false;
        break;
      }
    }
    if (correct) {
      message.textContent = 'واااو، حلّتي اللغز صح! مبروك يا أميرتي 🎉💕';
    } else {
      message.textContent = 'في أخطاء، جرّبي مرة ثانية وبكل حب! 🌸';
    }
  }

  function showSolution() {
    for(let i=0; i<81; i++) {
      const input = grid.children[i];
      input.value = solution[i];
      input.disabled = true;
      input.style.backgroundColor = '#ffd6e7';
      input.style.color = '#c2185b';
      input.style.fontWeight = 'bold';
    }
    message.textContent = 'هذا هو الحل الكامل، يا ملكة! 🌟';
  }

  window.onload = () => {
    createGrid();
  };
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>🎀 لعبة مطابقة كيوت</title>
<style>
  body {
    font-family: 'Arial', sans-serif;
    background: #fff0f9;
    color: #c2185b;
    text-align: center;
    padding: 20px;
  }
  header {
    background: #ffb6c1;
    color: white;
    padding: 15px;
    font-size: 26px;
    font-weight: bold;
    border-radius: 12px;
    margin-bottom: 20px;
  }
  #game-board {
    max-width: 400px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 12px;
  }
  .card {
    width: 80px;
    height: 80px;
    background: #ffe4ec;
    border-radius: 15px;
    box-shadow: 0 0 8px #ffbfdc;
    cursor: pointer;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 40px;
    user-select: none;
    transition: background 0.3s;
  }
  .card.flipped, .card.matched {
    background: #ff69b4;
    color: white;
    cursor: default;
  }
  #message {
    margin-top: 20px;
    font-weight: bold;
    font-size: 20px;
  }
  button {
    margin-top: 15px;
    padding: 12px 20px;
    font-size: 18px;
    border: none;
    border-radius: 15px;
    background-color: #ff69b4;
    color: white;
    cursor: pointer;
    font-weight: bold;
  }
</style>
</head>
<body>

<header>🎀 لعبة مطابقة كيوت</header>

<div id="game-board"></div>

<div id="message"></div>

<button onclick="startGame()">إعادة اللعب</button>

<script>
  const cardsSymbols = ['🌸', '🐻', '🍰', '🦋', '🎀', '🐥', '🍬', '🐱'];
  let cards = [];
  let flippedCards = [];
  let matchedCount = 0;
  const board = document.getElementById('game-board');
  const message = document.getElementById('message');

  function shuffle(array) {
    for (let i = array.length -1; i > 0; i--) {
      const j = Math.floor(Math.random() * (i +1));
      [array[i], array[j]] = [array[j], array[i]];
    }
  }

  function startGame() {
    matchedCount = 0;
    flippedCards = [];
    message.textContent = '';
    cards = [...cardsSymbols, ...cardsSymbols]; // نسختين لكل رمز
    shuffle(cards);
    board.innerHTML = '';
    cards.forEach((symbol, index) => {
      const card = document.createElement('div');
      card.className = 'card';
      card.dataset.symbol = symbol;
      card.dataset.index = index;
      card.textContent = '';
      card.onclick = () => flipCard(card);
      board.appendChild(card);
    });
  }

  function flipCard(card) {
    if (card.classList.contains('flipped') || card.classList.contains('matched')) return;
    if (flippedCards.length === 2) return;

    card.classList.add('flipped');
    card.textContent = card.dataset.symbol;
    flippedCards.push(card);

    if (flippedCards.length === 2) {
      setTimeout(checkMatch, 700);
    }
  }

  function checkMatch() {
    const [first, second] = flippedCards;
    if (first.dataset.symbol === second.dataset.symbol) {
      first.classList.add('matched');
      second.classList.add('matched');
      matchedCount += 2;
      message.textContent = 'رائع! وجدتي تطابقًا كيوت! 💖';
      if (matchedCount === cards.length) {
        message.textContent = 'واااو! أكملتِ اللعبة! مبروك يا أميرتي! 🎉🎀';
      }
    } else {
      first.classList.remove('flipped');
      second.classList.remove('flipped');
      first.textContent = '';
      second.textContent = '';
      message.textContent = 'حاولي مرة أخرى، أنتِ قوية يا كتكوتة! 💪💖';
    }
    flippedCards = [];
  }

  window.onload = startGame;
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>🎀 لعبة صراحة أو جراءة</title>
<style>
  body {
    font-family: 'Arial', sans-serif;
    background: #fff0f9;
    color: #c2185b;
    text-align: center;
    padding: 20px;
  }
  header {
    background: #ffb6c1;
    color: white;
    padding: 15px;
    font-size: 26px;
    font-weight: bold;
    border-radius: 12px;
    margin-bottom: 20px;
  }
  button {
    background: #ff69b4;
    border: none;
    border-radius: 15px;
    color: white;
    cursor: pointer;
    font-size: 18px;
    padding: 12px 25px;
    margin: 15px 10px;
    font-weight: bold;
    transition: background 0.3s;
  }
  button:hover {
    background: #ff4d94;
  }
  #result {
    margin-top: 20px;
    font-size: 22px;
    font-weight: bold;
    min-height: 80px;
    padding: 10px;
    border-radius: 15px;
    background: #ffe4ec;
    color: #c2185b;
  }
</style>
</head>
<body>

<header>🎀 لعبة صراحة أو جراءة</header>

<button onclick="showTruth()">صراحة</button>
<button onclick="showDare()">جرأة</button>

<div id="result"></div>

<script>
  const truths = [
    "ما أجمل صفة في نفسك؟ 💖",
    "من هو صديقك المفضل ولماذا؟ 🌸",
    "ما أكثر شيء يخوفك؟ 😱",
    "شو آخر مرة ضحكتي فيها من قلب؟ 😂",
    "ما سر صغير لم تخبريه لأحد؟ 🤫"
  ];

  const dares = [
    "ارسلي لأمك رسالة حب! 💌",
    "اعملي حركة رقص كيوت الآن! 💃",
    "قولي كلمة لطيفة لصديقتك القادمة! 🥰",
    "ارسم وردة صغيرة على ورقة ووريني الصورة! 🌹",
    "اصنعي قوس قزح باستخدام ألوانك المفضلة! 🌈"
  ];

  const resultDiv = document.getElementById('result');

  function getRandom(arr) {
    return arr[Math.floor(Math.random() * arr.length)];
  }

  function showTruth() {
    const question = getRandom(truths);
    resultDiv.textContent = `صراحة: ${question}`;
  }

  function showDare() {
    const challenge = getRandom(dares);
    resultDiv.textContent = `جرأة: ${challenge}`;
  }
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>🎀 لعبة الأسئلة البناتية</title>
<style>
  body {
    font-family: 'Arial', sans-serif;
    background: #fff0f9;
    color: #c2185b;
    text-align: center;
    padding: 20px;
  }
  header {
    background: #ffb6c1;
    color: white;
    padding: 15px;
    font-size: 26px;
    font-weight: bold;
    border-radius: 12px;
    margin-bottom: 20px;
  }
  #question {
    font-size: 22px;
    margin-bottom: 15px;
  }
  input[type="text"] {
    padding: 12px;
    font-size: 18px;
    border-radius: 12px;
    border: 2px solid #ffc0cb;
    width: 80%;
    max-width: 400px;
    text-align: center;
    margin-bottom: 15px;
  }
  button {
    background: #ff69b4;
    border: none;
    border-radius: 15px;
    color: white;
    cursor: pointer;
    font-size: 18px;
    padding: 12px 20px;
    font-weight: bold;
  }
  #response {
    margin-top: 20px;
    font-size: 20px;
    font-weight: bold;
    min-height: 40px;
  }
</style>
</head>
<body>

<header>🎀 لعبة الأسئلة البناتية</header>

<div id="question"></div>
<input type="text" id="answerInput" placeholder="اكتبي جوابك هنا..." />
<br/>
<button onclick="submitAnswer()">أرسلي جوابي</button>

<div id="response"></div>

<script>
  const questions = [
    "شو لونك المفضل؟ 🌸",
    "كم عمرك؟ 🐥",
    "شو اسم دبدوبك؟ 🐻",
    "شو أكتر شي بتحبيه تعمليه في وقت فراغك؟ 🎀",
    "لو كنتي حلوى، شو بتكوني؟ 🍬"
  ];

  const responses = {
    "لونك المفضل؟ 🌸": {
      "أحمر": "واااو، الأحمر لون الحب والشغف، ذوق راقي يا أميرتي! ❤️",
      "وردي": "الوردي لون الأميرات والأحلام الجميلة، جميل جدا! 🌷",
      "أزرق": "الأزرق هادي وجميل، يناسب روحك الهادية! 💙",
      "أصفر": "الأصفر مشرق وفرح، مثل ابتسامتك يا كتكوتة! 💛",
      "أخضر": "الأخضر لون الحياة والطبيعة، يا زهرة جميلة! 🌿"
    },
    "كم عمرك؟ 🐥": {
      "15": "عمر الزهور والضحكات، كل سنة وأنتِ بخير يا أميرة! 🎉",
      "14": "أجمل سنوات المراهقة، يا رب دايمًا فرحانة! 🌸",
      "16": "عمر الحلم والنجاح، فخورة فيكِ! 💖"
    },
    "شو اسم دبدوبك؟ 🐻": {
      "": "يا له من اسم لطيف! دبدوبك أكيد حبيبك الوفي! 🧸"
    },
    "شو أكتر شي بتحبيه تعمليه في وقت فراغك؟ 🎀": {
      "الرسم": "فنانة جميلة! استمري برسم أحلامك يا أميرتي! 🎨",
      "القراءة": "مذهلة! المعرفة نور يا ملكة! 📚",
      "اللعب": "الضحك والمرح هو سر السعادة، برافو! 😊"
    },
    "لو كنتي حلوى، شو بتكوني؟ 🍬": {
      "شكولاتة": "أنتِ حلوة زي الشكولاتة، الكل يحبك! 🍫",
      "مارشميلو": "ناعمة وطيبة، مثل المارشميلو اللطيف! ☁️",
      "بسكو": "مقرمشة وظريفة، مثل قلبك! 💖"
    }
  };

  let currentQuestionIndex = 0;

  function showQuestion() {
    document.getElementById('question').textContent = questions[currentQuestionIndex];
    document.getElementById('answerInput').value = '';
    document.getElementById('response').textContent = '';
  }

  function submitAnswer() {
    const question = questions[currentQuestionIndex];
    const answer = document.getElementById('answerInput').value.trim();
    if (!answer) {
      document.getElementById('response').textContent = "رجاءً اكتبي جواب يا أميرتي 💖";
      return;
    }
    let reply = responses[question][answer];
    if (!reply) {
      // رد لطيف افتراضي لو الجواب غير موجود
      reply = "جوابك مميز وفريد، يا زهرة قلبي! 🌸";
    }
    document.getElementById('response').textContent = reply;
    currentQuestionIndex = (currentQuestionIndex + 1) % questions.length;
    setTimeout(showQuestion, 2500);
  }

  window.onload = showQuestion;
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>يومياتي الأميرة 💖🎀</title>
<style>
  /* الخطوط والألوان */
  body {
    font-family: 'Arial', sans-serif;
    background: #fff0f9;
    color: #c2185b;
    margin: 0;
    padding: 0;
  }
  header {
    background: #ff69b4;
    color: white;
    padding: 15px;
    text-align: center;
    font-size: 28px;
    font-weight: bold;
  }
  nav {
    background: #ffb6c1;
    display: flex;
    justify-content: space-around;
    padding: 12px 0;
  }
  nav button {
    background: none;
    border: none;
    color: white;
    font-weight: bold;
    font-size: 16px;
    cursor: pointer;
    padding: 8px 15px;
    border-radius: 12px;
    transition: background 0.3s;
  }
  nav button.active, nav button:hover {
    background: #ff4d94;
  }
  main {
    max-width: 600px;
    margin: 20px auto 60px;
    padding: 0 15px;
  }
  section {
    display: none;
  }
  section.active {
    display: block;
  }
  /* التقويم */
  #calendar {
    width: 100%;
    border-collapse: collapse;
    text-align: center;
  }
  #calendar th, #calendar td {
    border: 1px solid #ffbfdc;
    padding: 10px;
    font-size: 14px;
    width: 14.28%;
    height: 60px;
    vertical-align: top;
    cursor: pointer;
    user-select: none;
  }
  #calendar th {
    background: #ff69b4;
    color: white;
  }
  #calendar td:hover {
    background: #ffe4ec;
  }
  #calendar td.selected {
    background: #ff4d94;
    color: white;
    font-weight: bold;
  }
  /* كلمات محفزة */
  #quote {
    font-size: 22px;
    font-weight: bold;
    background: #ffe4ec;
    padding: 20px;
    border-radius: 15px;
    margin-bottom: 10px;
    min-height: 80px;
  }
  /* الرسم */
  #drawCanvas {
    border: 3px solid #ff69b4;
    border-radius: 15px;
    background: #fff0f9;
    display: block;
    margin: 15px auto;
    touch-action: none;
  }
  #drawControls button {
    background: #ff69b4;
    border: none;
    color: white;
    padding: 12px 18px;
    margin: 8px 6px;
    font-weight: bold;
    border-radius: 15px;
    cursor: pointer;
    font-size: 16px;
  }
  /* تسجيل صوتي */
  #recorderControls button {
    background: #ff69b4;
    border: none;
    color: white;
    padding: 12px 18px;
    margin: 8px 6px;
    font-weight: bold;
    border-radius: 15px;
    cursor: pointer;
    font-size: 16px;
  }
  #recordingsList audio {
    margin: 10px 0;
    width: 100%;
    outline: none;
  }
  /* مذكرات - صور وفيديوهات */
  #notesList {
    margin-top: 15px;
  }
  .note {
    background: #ffe4ec;
    border-radius: 15px;
    padding: 15px;
    margin-bottom: 15px;
    position: relative;
  }
  .note textarea {
    width: 100%;
    height: 80px;
    border-radius: 12px;
    border: 1px solid #ffbfdc;
    padding: 8px;
    resize: vertical;
    font-size: 16px;
    color: #c2185b;
  }
  .note button.add-media {
    background: #ff69b4;
    color: white;
    border: none;
    padding: 8px 15px;
    margin: 8px 0;
    border-radius: 15px;
    cursor: pointer;
    font-weight: bold;
  }
  .media-preview {
    margin-top: 10px;
  }
  .media-preview img, .media-preview video {
    max-width: 100%;
    border-radius: 12px;
    margin-top: 8px;
  }
  /* زر إضافة مذكرات */
  #addNoteBtn {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background: #ff69b4;
    color: white;
    font-size: 36px;
    border-radius: 50%;
    width: 60px;
    height: 60px;
    border: none;
    cursor: pointer;
    box-shadow: 0 0 15px #ff4d94;
    line-height: 48px;
    font-weight: bold;
  }
  /* المهام */
  #tasksList {
    margin-top: 10px;
  }
  .task {
    background: #ffe4ec;
    border-radius: 15px;
    padding: 12px;
    margin-bottom: 12px;
    position: relative;
  }
  .task-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .task input[type="checkbox"] {
    transform: scale(1.4);
    margin-left: 8px;
  }
  .subtasks {
    margin-top: 8px;
    margin-right: 20px;
  }
  .subtask {
    background: #ffd6e7;
    border-radius: 12px;
    margin-bottom: 6px;
    padding: 6px 8px;
    display: flex;
    align-items: center;
  }
  .subtask input[type="checkbox"] {
    transform: scale(1.2);
    margin-left: 8px;
  }
  .notes-textarea {
    width: 100%;
    margin-top: 8px;
    border-radius: 12px;
    border: 1px solid #ffc0cb;
    padding: 8px;
    resize: vertical;
    font-size: 16px;
    color: #c2185b;
  }
  .add-subtask-btn {
    background: #ff69b4;
    border: none;
    color: white;
    padding: 8px 12px;
    border-radius: 12px;
    cursor: pointer;
    font-weight: bold;
    margin-top: 6px;
  }
  .add-task-btn {
    background: #ff69b4;
    border: none;
    color: white;
    padding: 12px 18px;
    border-radius: 15px;
    cursor: pointer;
    font-weight: bold;
    margin-top: 12px;
    width: 100%;
  }
</style>
</head>
<body>

<header>يومياتي الأميرة 💖🎀</header>

<nav>
  <button class="active" data-target="calendarSection">التقويم</button>
  <button data-target="quotesSection">كلمات محفزة</button>
  <button data-target="drawingSection">الرسم</button>
  <button data-target="recordingSection">تسجيل صوتي</button>
  <button data-target="notesSection">مذكرات</button>
  <button data-target="tasksSection">المهام</button>
</nav>

<main>
  <!-- التقويم -->
  <section id="calendarSection" class="active">
    <h2>تقويم اليوم</h2>
    <table id="calendar"></table>
  </section>

  <!-- الكلمات المحفزة -->
  <section id="quotesSection">
    <h2>كلمات محفزة ليومك</h2>
    <div id="quote">...</div>
    <button onclick="showNewQuote()">كلمة جديدة</button>
  </section>

  <!-- الرسم -->
  <section id="drawingSection">
    <h2>الرسم الحر</h2>
    <canvas id="drawCanvas" width="500" height="400"></canvas>
    <div id="drawControls">
      <button onclick="clearCanvas()">مسح الرسم</button>
    </div>
  </section>

  <!-- التسجيل الصوتي -->
  <section id="recordingSection">
    <h2>تسجيل صوتي</h2>
    <div id="recorderControls">
      <button id="startRecBtn">ابدأي التسجيل</button>
      <button id="stopRecBtn" disabled>أوقفي التسجيل</button>
    </div>
    <div id="recordingsList"></div>
  </section>

  <!-- المذكرات -->
  <section id="notesSection">
    <h2>مذكراتك</h2>
    <div id="notesList"></div>
    <button id="addNoteBtn" title="إضافة مذكرة جديدة">+</button>
  </section>

  <!-- المهام -->
  <section id="tasksSection">
    <h2>قائمة المهام</h2>
    <div id="tasksList"></div>
    <button id="addTaskBtn" class="add-task-btn">أضيفي مهمة جديدة</button>
  </section>
</main>

<script>
  // --- تنقل بين الصفحات ---
  const navButtons = document.querySelectorAll('nav button');
  const sections = document.querySelectorAll('main section');
  navButtons.forEach(btn => {
    btn.addEventListener('click', () => {
      navButtons.forEach(b => b.classList.remove('active'));
      btn.classList.add('active');
      const target = btn.getAttribute('data-target');
      sections.forEach(sec => {
        sec.id === target ? sec.classList.add('active') : sec.classList.remove('active');
      });
    });
  });

  // --- التقويم ---
  const calendar = document.getElementById('calendar');
  const today = new Date();
  let selectedDate = null;

  function generateCalendar(year, month) {
    calendar.innerHTML = '';
    const firstDay = new Date(year, month, 1);
    const lastDay = new Date(year, month +1, 0);
    const startDay = firstDay.getDay(); // 0=الأحد ... 6=السبت
    const daysInMonth = lastDay.getDate();

    // ترويسة أيام الأسبوع بالعربي (بدءاً من الأحد لسهولة التوافق)
    const daysNames = ['الأحد', 'الاثنين', 'الثلاثاء', 'الأربعاء', 'الخميس', 'الجمعة', 'السبت'];

    // رأس الجدول
    let thead = document.createElement('thead');
    let headerRow = document.createElement('tr');
    daysNames.forEach(dayName => {
      let th = document.createElement('th');
      th.textContent = dayName;
      headerRow.appendChild(th);
    });
    thead.appendChild(headerRow);
    calendar.appendChild(thead);

    // جسم الجدول
    let tbody = document.createElement('tbody');
    let row = document.createElement('tr');
    // ملء الفراغات قبل بداية الشهر
    for(let i=0; i<startDay; i++) {
      let emptyCell = document.createElement('td');
      row.appendChild(emptyCell);
    }
    // ملء أيام الشهر
    for(let day=1; day<=daysInMonth; day++) {
      if (row.children.length === 7) {
        tbody.appendChild(row);
        row = document.createElement('tr');
      }
      let cell = document.createElement('td');
      cell.textContent = day;
      cell.onclick = () => {
        if (selectedDate) selectedDate.classList.remove('selected');
        cell.classList.add('selected');
        selectedDate = cell;
      };
      // تمييز اليوم الحالي
      if (year === today.getFullYear() && month === today.getMonth() && day === today.getDate()) {
        cell.style.fontWeight = 'bold';
        cell.style.color = '#ff4d94';
      }
      row.appendChild(cell);
    }
    // إكمال صف الأسبوع الأخير بفراغات إذا احتاج
    while(row.children.length < 7) {
      row.appendChild(document.createElement('td'));
    }
    tbody.appendChild(row);
    calendar.appendChild(tbody);
  }

  generateCalendar(today.getFullYear(), today.getMonth());

  // --- الكلمات المحفزة ---
  const quotes = [
    "كل يوم هو فرصة جديدة لتكوني أفضل! 🌸",
    "ابتسامتكِ تضيء العالم، لا تنسيها أبداً! 😊",
    "ثقي بنفسكِ، فأنتِ أجمل أميرة! 👑",
    "الأمل هو سر النجاح، لا تفقديه! 🌟",
    "كل خطوة صغيرة تقربك من حلمك الكبير! 💖"
  ];
  const quoteDiv = document.getElementById('quote');
  function showNewQuote() {
    const idx = Math.floor(Math.random() * quotes.length);
    quoteDiv.textContent = quotes[idx];
  }
  showNewQuote();

  // --- الرسم ---
  const canvas = document.getElementById('drawCanvas');
  const ctx = canvas.getContext('2d');
  let drawing = false;
  let lastX = 0, lastY = 0;

  function startDrawing(e) {
    drawing = true;
    const pos = getPos(e);
    lastX = pos.x;
    lastY = pos.y;
  }
  function stopDrawing() {
    drawing = false;
  }
  function draw(e) {
    if (!drawing) return;
    e.preventDefault();
    const pos = getPos(e);
    ctx.strokeStyle = '#c2185b';
    ctx.lineWidth = 3;
    ctx.lineCap = 'round';
    ctx.beginPath();
    ctx.moveTo(lastX, lastY);
    ctx.lineTo(pos.x, pos.y);
    ctx.stroke();
    lastX = pos.x;
    lastY = pos.y;
  }
  function getPos(e) {
    let rect = canvas.getBoundingClientRect();
    let x, y;
    if (e.touches) {
      x = e.touches[0].clientX - rect.left;
      y = e.touches[0].clientY - rect.top;
    } else {
      x = e.clientX - rect.left;
      y = e.clientY - rect.top;
    }
    return {x, y};
  }
  canvas.addEventListener('mousedown', startDrawing);
  canvas.addEventListener('touchstart', startDrawing);
  canvas.addEventListener('mouseup', stopDrawing);
  canvas.addEventListener('mouseout', stopDrawing);
  canvas.addEventListener('touchend', stopDrawing);
  canvas.addEventListener('touchcancel', stopDrawing);
  canvas.addEventListener('mousemove', draw);
  canvas.addEventListener('touchmove', draw);

  function clearCanvas() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
  }

  // --- تسجيل صوتي ---
  const startRecBtn = document.getElementById('startRecBtn');
  const stopRecBtn = document.getElementById('stopRecBtn');
  const recordingsList = document.getElementById('recordingsList');
  let mediaRecorder;
  let audioChunks = [];

  startRecBtn.onclick = async () => {
    if (!navigator.mediaDevices || !navigator.mediaDevices.getUserMedia) {
      alert('التسجيل غير مدعوم في متصفحك.');
      return;
    }
    try {
      const stream = await navigator.mediaDevices.getUserMedia({ audio: true });
      mediaRecorder = new MediaRecorder(stream);
      mediaRecorder.start();
      audioChunks = [];
      mediaRecorder.ondataavailable = e => audioChunks.push(e.data);
      mediaRecorder.onstop = e => {
        const audioBlob = new Blob(audioChunks, { type: 'audio/mp3' });
        const audioUrl = URL.createObjectURL(audioBlob);
        const audio = document.createElement('audio');
        audio.controls = true;
        audio.src = audioUrl;
        recordingsList.appendChild(audio);
      };
      startRecBtn.disabled = true;
      stopRecBtn.disabled = false;
    } catch {
      alert('لم نستطع الوصول إلى الميكروفون.');
    }
  };

  stopRecBtn.onclick = () => {
    if (mediaRecorder) {
      mediaRecorder.stop();
      startRecBtn.disabled = false;
      stopRecBtn.disabled = true;
    }
  };

  // --- مذكرات مع إضافة صور وفيديوهات ---
  const notesList = document.getElementById('notesList');
  const addNoteBtn = document.getElementById('addNoteBtn');

  function createNote() {
    const noteDiv = document.createElement('div');
    noteDiv.className = 'note';

    const textarea = document.createElement('textarea');
    textarea.placeholder = 'اكتبي مذكرتك هنا...';
    noteDiv.appendChild(textarea);

    // زر إضافة صورة أو فيديو
    const addMediaBtn = document.createElement('button');
    addMediaBtn.textContent = 'أضيفي صورة أو فيديو';
    addMediaBtn.className = 'add-media';
    addMediaBtn.onclick = () => {
      const inputFile = document.createElement('input');
      inputFile.type = 'file';
      inputFile.accept = 'image/*,video/*';
      inputFile.onchange = e => {
        const file = e.target.files[0];
        if (!file) return;
        const reader = new FileReader();
        reader.onload = ev => {
          let media;
          if (file.type.startsWith('image/')) {
            media = document.createElement('img');
            media.src = ev.target.result;
          } else if (file.type.startsWith('video/')) {
            media = document.createElement('video');
            media.src = ev.target.result;
