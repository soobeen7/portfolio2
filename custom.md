🚀 바이브코딩 프리미엄 포트폴리오 커스터마이징 가이드

이 문서는 학생들이 코드를 완벽히 이해하지 못하더라도, HTML 내의 특정 영역(텍스트, 이미지 주소)만 수정하면 자신만의 완벽한 포트폴리오를 만들 수 있도록 작성된 매뉴얼입니다. 메모장이나 코드 에디터에서 index.html 파일을 열고 아래 안내에 따라 수정하세요.

1️⃣ [인트로 화면] 텍스트 수정하기

사이트 접속 시 가장 먼저 보이는 화면입니다. 코드를 열고 id="introScreen" 부분을 찾아 아래 내용들을 학생의 정보로 바꿔주세요.

<!-- 기존 코드 -->
<div class="intro-anim sub-title" id="introSubTitle">Vibe Coding class</div>
<h1 class="intro-anim super-title" id="introMainTitle">
  <span>CREATIVE</span>
  <span>JOURNEY</span>
</h1>

<!-- 변경 예시 -->
<div class="intro-anim sub-title" id="introSubTitle">My awesome portfolio</div>
<h1 class="intro-anim super-title" id="introMainTitle">
  <span>HELLO</span>
  <span>WORLD</span>
</h1>


2️⃣ [메인 화면] 이름 및 직업 수정하기

인트로에서 버튼을 누르면 나타나는 메인 주인공 영역입니다. id="hero" 부분을 수정하세요.

<!-- 기존 코드 -->
<div class="hero-element sub-title opacity-0 translate-y-10" id="heroSubTitle">Interactive Developer</div>
<h1 class="hero-element super-title opacity-0 translate-y-10" id="heroMainTitle">
  <span>Kim</span>
  <span>Vibe.</span>
</h1>

<!-- 변경 예시 -->
<div class="hero-element sub-title opacity-0 translate-y-10" id="heroSubTitle">AI Prompt Engineer</div>
<h1 class="hero-element super-title opacity-0 translate-y-10" id="heroMainTitle">
  <span>Hong</span>
  <span>Gildong.</span>
</h1>


3️⃣ [캐릭터 이미지] 내 아바타로 교체하기 (가장 중요!)

마우스 움직임에 반응하며 화면을 떠다니는 캐릭터를 본인의 사진이나 AI 아바타로 변경하세요.

팁: 이미지는 가급적 배경이 투명한 PNG(누끼 이미지)를 사용해야 우주 배경과 완벽하게 어우러집니다.

<!-- id="charWrapper" 부분을 찾으세요 -->
<img src="[https://raw.githubusercontent.com/.../25.png](https://raw.githubusercontent.com/.../25.png)" alt="캐릭터" class="character-img" id="studentImg">

<!-- src 안의 인터넷 링크를 자신의 이미지 링크나 파일명(예: my-avatar.png)으로 바꾸세요 -->
<img src="my-avatar.png" alt="내 캐릭터" class="character-img" id="studentImg">


4️⃣ [프로젝트 내용 1~10] 내용 및 링크 수정하기

총 10개의 프로젝트 영역(id="proj1" ~ id="proj10")이 있습니다. 각 영역 내부에서 이미지, 카테고리, 제목, 설명, 링크를 자유롭게 변경하세요.

수정해야 할 5가지 포인트:

이미지 (<img>): src="..." 부분을 썸네일 이미지 주소로 변경

카테고리 (<div>): 01 // AI INTERACTION 부분을 01 // 게임 개발 등으로 변경

제목 (<h2>): Smart Chatbot 부분을 프로젝트 이름으로 변경

설명 (<p>): 프로젝트에 대한 상세 설명 텍스트 작성

이동 링크 (<a>): <a href="#">의 # 자리에 깃허브, 노션, 유튜브 등 결과물을 볼 수 있는 실제 주소 입력

<!-- 프로젝트 수정 예시 -->
<div class="w-full h-[400px] img-parallax-wrap mb-10">
  <img src="내가만든_게임사진.jpg" alt="Project 1" class="...">
</div>
<div class="flex flex-col">
  <div class="...">01 // GAME DEV</div>
  <h2 class="...">나만의 슈팅 게임</h2>
  <p class="...">파이썬을 활용해 개발한 슈팅 게임입니다.</p>
  <div class="...">
    <!-- href 속성에 링크 넣기 -->
    <a href="[https://github.com/my-game](https://github.com/my-game)" class="circle-link">...</a>
  </div>
</div>


🎨 (선택) 배경 오로라 색상 커스텀

우주에 떠다니는 빛 덩어리(오로라)의 색상을 본인이 좋아하는 테마로 바꿀 수 있습니다. 코드 최상단의 CSS <style> 안에 있는 :root 부분을 수정하세요.

:root {
  /* ... 생략 ... */
  --glow-1: #4f46e5; /* 첫 번째 빛 색상 (인디고) */
  --glow-2: #c026d3; /* 두 번째 빛 색상 (핑크) */
  --glow-3: #0ea5e9; /* 세 번째 빛 색상 (스카이블루) */
}


팁: 원하는 색상의 헥스코드(예: #ff0000)를 구글에 검색해서 복사해 넣으면 됩니다.