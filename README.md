
<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>지난 모임 참가자 | 블랙라벨 더논현</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Serif+KR:wght@200;300;400;500;600;700&family=Pretendard:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --white:#FFFFFF;
    --cream:#FBF7F6;
    --rose:#C97B86;
    --rose-deep:#8B4A56;
    --rose-soft:#F3E4E6;
    --ink:#2B2526;
    --ink-soft:#6B5F60;
    --line:#E8DCDD;
  }

  *{margin:0;padding:0;box-sizing:border-box;}

  html{scroll-behavior:smooth;}

  body{
    font-family:'Pretendard','Noto Serif KR',serif;
    color:var(--ink);
    background:var(--ink);
    line-height:1.7;
    overflow-x:hidden;
  }

  .serif{font-family:'Noto Serif KR',serif;}

  a{text-decoration:none;color:inherit;}

  /* ---------- Nav ---------- */
  header{
    position:fixed;
    top:0;left:0;right:0;
    z-index:100;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:22px 6%;
    background:rgba(43,37,38,0.88);
    backdrop-filter:blur(10px);
    border-bottom:1px solid transparent;
    transition:border-color .3s;
  }
  header.scrolled{border-color:rgba(255,255,255,0.12);}

  .logo{
    font-family:'Noto Serif KR',serif;
    font-weight:600;
    font-size:19px;
    letter-spacing:0.5px;
    color:var(--white);
  }
  .logo span{color:var(--rose);}

  nav ul{
    display:flex;
    align-items:center;
    gap:36px;
    list-style:none;
  }
  nav a{
    font-size:13.5px;
    letter-spacing:0.5px;
    color:#C9BFC0;
    transition:color .25s;
  }
  nav a:hover{color:var(--rose);}
  nav a.current{color:var(--rose);}

  .nav-cta{
    border:1px solid var(--rose);
    color:var(--white) !important;
    padding:9px 22px;
    border-radius:2px;
    font-size:13px;
    letter-spacing:1px;
  }
  .nav-cta:hover{background:var(--rose);}

  @media (max-width:820px){
    nav ul{gap:20px;}
    nav ul li:not(.nav-back){display:none;}
  }
  @media (max-width:600px){
    .nav-cta{display:none;}
  }

  /* ---------- Page header ---------- */
  .page-hero{
    padding:170px 6% 60px;
    text-align:center;
    max-width:640px;
    margin:0 auto;
  }
  .eyebrow{
    display:inline-flex;
    align-items:center;
    gap:10px;
    font-size:12.5px;
    letter-spacing:2.5px;
    color:var(--rose);
    margin-bottom:20px;
    justify-content:center;
  }
  .page-hero h1{
    font-family:'Noto Serif KR',serif;
    font-weight:400;
    font-size:clamp(28px,4vw,42px);
    line-height:1.4;
    color:var(--white);
    margin-bottom:18px;
  }
  .page-hero h1 strong{color:var(--rose);font-weight:700;}
  .page-hero p{
    color:#C9BFC0;
    font-size:15px;
  }

  /* ---------- Past Participants ---------- */
  .past-section{padding:20px 6% 130px;}
  .section-inner{max-width:1180px;margin:0 auto;}
  .past-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:0;
    border:1px solid rgba(255,255,255,0.15);
  }
  .past-col{
    padding:56px 50px;
    position:relative;
  }
  .past-col:first-child{border-right:1px solid rgba(255,255,255,0.15);}
  .past-col .tag{
    font-size:12px;
    letter-spacing:2px;
    color:var(--rose);
    margin-bottom:14px;
    display:block;
  }
  .past-col h3{
    font-family:'Noto Serif KR',serif;
    font-size:25px;
    font-weight:400;
    color:var(--white);
    margin-bottom:26px;
  }
  .past-col ul{list-style:none;}
  .past-col li{
    font-size:13.5px;
    color:#D8D0D1;
    padding:12px 0;
    border-top:1px solid rgba(255,255,255,0.1);
    display:flex;
    align-items:baseline;
    gap:10px;
    line-height:1.6;
  }
  .past-col li:first-of-type{border-top:none;}
  .past-col li::before{
    content:'';
    width:5px;height:5px;
    border-radius:50%;
    background:var(--rose);
    flex-shrink:0;
    transform:translateY(-2px);
  }
  @media (max-width:980px){
    .past-grid{grid-template-columns:1fr;}
    .past-col:first-child{border-right:none;border-bottom:1px solid rgba(255,255,255,0.15);}
  }
  @media (max-width:600px){
    .past-col{padding:40px 26px;}
  }

  /* ---------- Back link ---------- */
  .back-link-wrap{
    text-align:center;
    margin-top:56px;
  }
  .back-link{
    display:inline-flex;
    align-items:center;
    gap:8px;
    border:1px solid rgba(255,255,255,0.25);
    color:var(--white);
    padding:14px 34px;
    border-radius:2px;
    font-size:13.5px;
    letter-spacing:1px;
    transition:border-color .25s, color .25s;
  }
  .back-link:hover{border-color:var(--rose);color:var(--rose);}

  /* ---------- Footer ---------- */
  footer{
    background:#1E1A1B;
    color:#9C9293;
    padding:44px 6% 26px;
    text-align:center;
    font-size:12.5px;
  }
</style>
</head>
<body>

<!-- ================= HEADER ================= -->
<header id="header">
  <div class="logo">블랙라벨 <span>더논현</span></div>
  <nav>
    <ul>
      <li><a href="index.html#message">소개</a></li>
      <li><a href="index.html#why">차이점</a></li>
      <li><a href="index.html#gallery">모임 사진</a></li>
      <li><a href="index.html#process">진행 절차</a></li>
      <li><a href="past.html" class="current">지난 모임</a></li>
      <li class="nav-back"><a href="index.html" class="nav-cta">메인으로</a></li>
    </ul>
  </nav>
</header>

<!-- ================= PAGE HERO ================= -->
<div class="page-hero">
  <span class="eyebrow">PAST MEETING</span>
  <h1 class="serif">지난 모임 <strong>참가자 보기</strong></h1>
  <p>블랙라벨 더논현에 실제로 참여했던 회원분들의 프로필을 소개합니다.</p>
</div>

<!-- ================= PAST PARTICIPANTS ================= -->
<section class="past-section">
  <div class="section-inner">
    <div class="past-grid">
      <div class="past-col">
        <span class="tag">FOR MEN</span>
        <h3 class="serif">인성과 능력을<br>보장합니다</h3>
        <ul>
          <li>남자1호. 92년생 / 공무원 / 키175 / 순박단정한선비몸매 스타일</li>
          <li>남자2호. 92년생 / 공무원 / 키184 / 순둥하고 지적인 스타일</li>
          <li>남자3호. 85년생 / 투자자 / 키183 / 엄친아 자상예남 스타일</li>
          <li>남자4호. 90년생 / IT엔지니어 / 키176 / 청순하고 섬세한능력남 스타일</li>
          <li>남자5호. 87년생 / 개발자 / 키177 / 깔끔한 상남자 스타일</li>
          <li>남자6호. 91년생 / 의사 / 키175 / 단정하고 순둥한의사 스타일</li>
          <li>남자7호. 83년생 / 공기업 / 키184 / 남자다운 며느리상 스타일</li>
          <li>남자8호. 86년생 / 금융보험관리직 / 키177 / 부드러운 존잘 스타일</li>
          <li>남자9호. 88년생 / 금융보험관리직 / 키181 / 주진모닮은 테토미남 스타일</li>
          <li>남자10호. 84년생 / 건축업이사 / 키180 / 멀끔한 미존잘 스타일</li>
          <li>남자11호. 83년생 / AI개발회사경영 / 키174 / 훈훈상냥한 에겐 스타일</li>
          <li>남자12호. 89년생 / 의류회사팀장 / 키177 / 귀엽고 듬직한곰 스타일</li>
          <li>남자13호. 96년생 / 대기업영업직 / 키178 / 훈내진동 강아지 스타일</li>
          <li>남자14호. 81년생 / 계조도매업체대표 / 키177 / 차분한 신사 스타일</li>
          <li>남자15호. 83년생 / 4급공무원 / 키179 / 지니어스 귀공자 스타일</li>
          <li>남자16호. 83년생 / SK하이닉스 / 키183 / 훈훈한 영국신사 스타일</li>
          <li>남자17호. 95년생 / 의사 / 키180 / 훈훈잘생긴 의사 스타일</li>
          <li>남자18호. 87년생 / 화학대기업 / 키180 / 젠틀깔끔한 스타일</li>
        </ul>
      </div>
      <div class="past-col">
        <span class="tag">FOR WOMEN</span>
        <h3 class="serif">인성과 미모를<br>보장합니다</h3>
        <ul>
          <li>여자1호. 93년생 / 간호사 / 청순여성스러운 스타일</li>
          <li>여자2호. 95년생 / 서비스직 / 귀엽고 친한 이목구비 스타일</li>
          <li>여자3호. 90년생 / 패션회사디렉터 / 여리여리한 도시미녀 스타일</li>
          <li>여자4호. 89년생 / 뷰티샵운영 / 건강미넘치는 섹시녀 스타일</li>
          <li>여자5호. 93년생 / 대기업 / 김태리닮은 은은한 청순 스타일</li>
          <li>여자6호. 94년생 / 취업준비생 / 꾸밈없이 편안한 스타일</li>
          <li>여자7호. 95년생 / 사무직 / 꾸밈없는 긴생머리 스타일</li>
          <li>여자8호. 83년생 / 경영기획 / 도도한듯 청순한 스타일</li>
          <li>여자9호. 95년생 / 공무원 / 청순단아한 결정체 스타일</li>
          <li>여자10호. 94년생 / 유통회사원 / 다정상냥 청순귀염 스타일</li>
          <li>여자11호. 87년생 / 언론인 / 발랄상큼 지적인 스타일</li>
          <li>여자12호. 90년생 / IT회사원 / 청순한 미녀 스타일</li>
          <li>여자13호. 99년생 / 간호사 / 존예 청순발랄 MZ 스타일</li>
          <li>여자14호. 03년생 / 대학생 / 카리나닮은 존예 스타일</li>
          <li>여자15호. 88년생 / 승무원 / 단아&amp;우아한 존예 스타일</li>
          <li>여자16호. 82년생 / 데이터분석가 / 분위기미인 스타일</li>
          <li>여자17호. 90년생 / 은행원 / 첫사랑재질 존예걸 스타일</li>
          <li>여자18호. 99년생 / 행정사무직 / 귀엽고발랄한 스타일</li>
          <li>여자19호. 89년생 / 미디어 / 매력있는 댕댕미 스타일</li>
        </ul>
      </div>
    </div>

    <div class="back-link-wrap">
      <a href="index.html" class="back-link">← 메인 페이지로 돌아가기</a>
    </div>
  </div>
</section>

<!-- ================= FOOTER ================= -->
<footer>
  © 2026 BLACK LABEL THE NON-HYUN. All rights reserved.
</footer>

<script>
  const header = document.getElementById('header');
  window.addEventListener('scroll', () => {
    header.classList.toggle('scrolled', window.scrollY > 20);
  });
</script>

</body>
</html>
