<!DOCTYPE html>
<html>
<head>
  <title>JEONGMIN KEUM</title>
  <style>
    /* 간단한 스타일링 */
    /* ... (기존 CSS 내용 그대로 유지) ... */

    /* 3단 레이아웃 스타일 */
    body {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-gap: 20px;
      background-color: #dbdbdb;
      font-family: 'Pretendard', Regular;
      margin: 0;
      padding: 0;
    }

    .sidebar {
      background-color: #dbdbdb;
      padding: 25px;
      box-sizing: border-box;
      grid-column: 1;
      text-align: left;
      font-size: 14px;
      font-weight: normal; /* sidebar 폰트 굵기 설정 */
    }

    .main-content {
  background-color: #dbdbdb;
  padding: 0 25px; /* 좌우 여백 추가 */
  box-sizing: border-box;
  grid-column: 2;
  max-width: 100%; /* 최대 너비 설정 */
  margin: 0 auto; /* 가운데 정렬 */
    }

    .description {
      background-color: #dbdbdb;
      padding: 25px;
      box-sizing: border-box;
      grid-column: 3;
      font-size: 14px;
      font-weight: normal; /* description 폰트 굵기 설정 */
    }

    /* 목차에서 리스트 점 제거 */
    .sidebar ul {
      list-style-type: none;
      padding: 0;
      margin: 0;
      display: flex;
      flex-direction: column;
    }

    /* h2에 대한 스타일 수정 */
    .sidebar h2 {
      font-family: 'Pretendard', Regular, sans-serif;
      cursor: pointer;
      margin: 0;
      padding: 0;
      font-weight: 400; /* h2 폰트 굵기 설정 */
      margin-bottom: 10px; /* JEONGMIN KEUM과 다른 항목 사이 간격 설정 */
    }

    /* sidebar 내 리스트 아이템들의 스타일 */
    .sidebar li {
      font-family: 'Pretendard', Regular, sans-serif;
      cursor: pointer;
      margin: 0;
      padding: 0;
      font-weight: 400; /* 리스트 아이템 폰트 굵기 설정 */
      margin-bottom: 3px; /* JEONGMIN KEUM과 다른 항목 사이 간격 설정 */
    }
     /* 미디어 쿼리 */
    @media (min-width: 768px) {
      body {
        flex-direction: row; /* 768px 이상 화면에서 가로 방향으로 배치 */
      }
        /* 반응형 디자인 */
    @media screen and (max-width: 768px) {
      /* 화면이 768px보다 작을 때 적용될 스타일 */
      body {
        display: block;
      }
      .sidebar,
      .main-content,
      .description {
        width: 100%;
      }
    }


    @media screen and (min-width: 768px) {
      /* 화면이 768px 이상일 때 적용될 스타일 */
      body {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-gap: 20px;
      }
      .sidebar,
      .main-content,
      .description {
        width: auto;
        height: 790px;
      }
    }

    /* 미디어 쿼리 */
@media (max-width: 768px) {
  body {
    flex-direction: column; /* 화면이 768px 미만일 때 세로 방향으로 배치 */
  }
  .sidebar, .main-content, .description {
    max-width: none; /* 모든 요소의 최대 너비 초기화 */
    flex: 1; /* 모든 요소가 동일한 공간을 차지하도록 설정 */
  }
}
/* CSS */
.mouse-emoji {
  display: none;
  position: absolute;
  pointer-events: none;
  z-index: 9999;
  font-size: 25px;
  /* 추가한 이모지 스타일링 */
  color: black; /* 이모지 색상 변경 */
  font-weight: lighter; /* 또는 bold, lighter, 등의 값을 사용하여 두께 조절 가능 */

    }
.emoji1 {
      display: none;
    }

    .emoji2 {
      display: none;
    }

    .emoji3 {
      display: none;
    }

   .bottom-text {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  padding: -20px 0; /* 패딩 수정 */
  padding-left: -40px; /* 왼쪽 여백 조정 */
  text-align: left;
  font-size: 8.5px;
  font-weight: normal;
    }
    


  </style>
</head>
<body>

  <div class="mouse-emoji emoji1">🍽️+˚…~</div>
  <div class="mouse-emoji emoji2">🍦…˚+˚</div>
  <div class="mouse-emoji emoji3">🥚+˚…~</div>
  <div class="sidebar">
    <!-- 목차 -->
    <h2 onclick="showDescription()">Jeongmin Keum</h2>
    <ul>
      <li onclick="changeContent('egg')">Everyone has an egg to hatch</li>
      <li onclick="changeContent('goblet')">a curved goblet glass</li>
      <li onclick="changeContent('mug')">Dasom mug</li>
      <li onclick="changeContent('apple')">Red apple bowling</li>

      <!-- 목차 항목 추가 -->
      <!-- 이메일 추가 -->
      <li><a href="mailto:jeongminkeum@gmail.com">jeongminkeum@gmail.com</a></li>
      <!-- 전화번호 추가 -->
      <li><a href="tel:+821089659390">+82 10 8965 9390</a></li>
      <!-- 인스타그램 링크 추가 -->
      <li><a href="https://www.instagram.com/oominkeum/">oominkeum</a></li>
    </ul>

  </div>
  <div class="main-content" id="main-content">
    <!-- 이미지 -->
    <img src="pizza.png" width="500" height="790">
  </div>
  <div class="description" id="description" style="display: none;width: 100%;">
    <!-- 설명 -->
    <p>안녕하세요 경험을 더하는 디자이너 금정민입니다.</p>

    <p>디자인에는 단순한 외관 뿐만 아니라 사용자의 경험을 개선하고 새로운 가치를 전달하는 역할이 있다고 믿습니다. 이러한 철학이 제 디자인 작업에 반영되어 있습니다.</p>

    <p>프로젝트를 통해 다양성을 추구하며, 새로운 도전에 열린 마음으로 접근하는 것을 즐깁니다. 내적 도전을 통해 긍정적인 태도를 유지하고, 새로운 아이디어와 디자인으로 더 나은 경험을 창조하는 것을 목표로 삼고 있습니다</p>
    <!-- ... (기존 설명 내용 그대로 유지) ... -->
  </div>

  <div class="bottom-text">
    <pre>
      ===========================================
      ==========================================
      * +……+˚……˚+……+˚……˚+……+˚……˚+……+˚……˚+……+
      *
      *          ･ ｡　　★彡
      *    ☆彡｡∴｡｡　☆彡　･
      *    　･ﾟ*｡★彡･ ｡*･ﾟ　★彡
      *    　　･ ｡･*･ﾟ｡　　 ･
      *    　･ ｡･*･ﾟ｡
      *
      * 
      * ̛ ̛ ´´ ´´ ´´ ̛ ̛ ´´ ´´ ´´ ̛ ̛ ´´ ´´ ´´
      *
      * +……+˚……˚+……+˚……˚+……+˚……˚+……+˚……˚+……+
      ==========================================
      ==========================================
      @2023 Jeongmin Keum
      ==========================================
    </pre>
  </div>

  <script>

 // 마우스 이벤트 리스너 추가
 document.addEventListener('mousemove', function(e) {
    var emoji1 = document.querySelector('.emoji1');
    var emoji2 = document.querySelector('.emoji2');
    var emoji3 = document.querySelector('.emoji3');
    
    var emojiSize = 20; // 이모지 크기
    var spacing = 55; // 이모지 간격

    // 첫 번째 이모지
    emoji1.style.left = e.pageX + 'px';
    emoji1.style.top = e.pageY + 'px';
    emoji1.style.display = 'block'; // 이모지 1 표시

    // 두 번째 이모지
    emoji2.style.left = e.pageX + emojiSize + spacing + 'px';
    emoji2.style.top = e.pageY + 'px';
    emoji2.style.display = 'block'; // 이모지 2 표시

    // 세 번째 이모지
    emoji3.style.left = e.pageX + (emojiSize + spacing) * 2 + 'px';
    emoji3.style.top = e.pageY + 'px';
    emoji3.style.display = 'block'; // 이모지 3 표시
  });
  function changeContent(item) {
    var mainContent = document.getElementById('main-content');
    var description = document.getElementById('description');
    var imgSrc = '';
    var contentText = '';

    // 각 항목에 따라 이미지와 내용 변경
    if (item === 'egg') {
      imgSrc = 'egg_image.png'; // 클릭한 항목에 따라 이미지 경로 변경
      contentText = `<p> 데미안에서 나온 '새는 알에서 나오기 위해 투쟁한다. 알은 세계이다. 태어나려고 하는 자는 누구든 하나의 세계를 파괴하지 않으면 안된다.’를 바탕으로 제작한 계란 형태의 초로, 모두가 알을 부화시키기 위해 투쟁하는 과정을 상징합니다.</p>
      
     <p> 이 계란은 누구나 가지고 있는 가능성과 목표에 도전하고 헌신하는 모습을 담고 있습니다. 높은 위에서부터 녹는 초는 무언가를 정면으로 돌파하고 파고드는 잔상을 담아내어, 각자의 가능성을 적극적으로 표현하는 모습을 상징합니다.</p>
      
      <p>이 작품은 모두가 자신의 목표와 가능성을 향해 나아가며, 자신을 표현하고자 하는 메시지를 전달합니다. </p> <p>또한, '정체성과 본성'을 표현하기 위해서는 내면의 깊은 곳으로 진심으로 파고들어야 한다는 메시지를 함께 담고 있습니다.</p>`; // 클릭한 항목에 따라 내용 변경
    } else if (item === 'goblet') {
         imgSrc = 'goblet_image.png'; // 클릭한 항목에 따라 이미지 경로 변경
      contentText = `<p>사람은 가끔 예상치 못한 일들로 인해 굽거나 휘어지기도 합니다. 하지만 그 휘어진 모습 또한 삶의 일부입니다.</p> <p>이런 상황은 새로운 경험과 성장의 기회로 이어집니다. 마치 휘어진 고블렛잔처럼, 저는 삶의 변화를 수용하고 적응하는 능력을 가지고 있습니다.</p> <p>이 휘어진 잔은 저에게 끊임없는 새로운 가능성과 유연성을 상기시켜줍니다.</p>`; // 클릭한 항목에 따라 내용 변경
    } else if (item === 'mug') {
      imgSrc = 'dasom_mug_image.png'; // 클릭한 항목에 따라 이미지 경로 변경
      contentText = `<p> 2022년 여름, 뉴욕 여행은 저에게 큰 영감을 주었습니다.그곳에서 새로운 인연을 만나고, 시야가 확대되며 새로운 생각을 많이 하게 되었습니다.</p> <p>한국으로 돌아와서 작업 중에 컵에 커피를 마실 때, 때로는 생각에 빠져 손잡이를 놓칠 때가 있었습니다.</p> <p>그럴 때마다, 내가 가장 좋아하는 컵이 그냥 손잡이가 많이 달려서 이 생각에서 벗어나지 않고 안전하게 잡을순 없을까라는 생각에서 부터 제작되었습니다.</p>
      
      <p>이 손잡이가 많은 I ♥ NY 컵의 손잡이를 잡을 때마다 뉴욕에서의 인연과 경험이 떠오르며, 안정된 시간을 보낼 수 있었습니다.<p>`; // 클릭한 항목에 따라 내용 변경
    } else if (item === 'apple') {
      imgSrc = 'red_apple_bowling_image.png'; // 클릭한 항목에 따라 이미지 경로 변경
      contentText = `<p>저에게 있어 사과는 항상 특별한 의미를 갖고 있습니다. 할머니와 할아버지가 사과 농장을 하셔서 식탁에는 항상 사과가 있었고, 부모님이 항상 깍아서 주셨습니다.</p> <p>이런 사과는 풍요와 사랑을 상징하는데요, 그래서 조부모님과 부모님의 사랑과 지지를 사과 모양의 볼링공으로 표현해보게 되었습니다.</p>

      <p>이 작품은 삶에서 목표를 이루고 성취하는 모습을 나타내고 있습니다.</p>
      <p>지지와 사랑의 의미를 담은 사과 볼링공으로, 인생의 볼링핀을 넘어 뜨리고, 스트라이킹 아웃으로 마무리 짓는 것과 같은 느낌을 담고 있습니다.</p>`; // 클릭한 항목에 따라 내용 변경
    }

    // main-content와 description 내용 변경
    mainContent.innerHTML = '<img src="' + imgSrc + '" width="540" height="790">';
    description.innerHTML = '<p>' + contentText + '</p>';
    description.style.display = 'block'; // description 표시
  }

  function showDescription() {
    var description = document.getElementById('description');
    description.style.display = 'block'; // description 표시
  }

  // JEONGMIN KEUM을 클릭하여 페이지가 로드될 때 설명을 보이도록 설정
  showDescription();
</script>

</body>
</html>
