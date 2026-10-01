# Golden-Smile-
Golden Smile is a travel company that offers one-day island tours in Nha Trang. Its purpose is to promote island tourism and attract more tourists. 
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Golden Smile — Khám phá đảo hoang Nha Trang</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:wght@400;600;800&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --sea-deep:#0E4749; --turquoise:#2C8C99; --sand:#F2E8D5; --gold:#E8A33D; --coral:#E85B45; --ink:#12302E;
  box-sizing:border-box; padding-top:env(safe-area-inset-top,0px); padding-bottom:env(safe-area-inset-bottom,0px);
}
*{box-sizing:inherit; margin:0; padding:0;}
html{scroll-padding-top:env(safe-area-inset-top,0px); scroll-behavior:smooth;}
html,body{background:var(--sand); color:var(--ink); font-family:'Inter',sans-serif; overflow-x:hidden;}
h1,h2,h3,.disp{font-family:'Bricolage Grotesque',sans-serif;}
.wrap{max-width:1080px; margin:0 auto; padding:0 28px;}
img{max-width:100%;}
a{color:inherit;}

/* NAV */
nav{position:sticky; top:0; z-index:20; background:rgba(242,232,213,.92); backdrop-filter:blur(6px); border-bottom:1px solid rgba(18,48,46,.1);}
nav .wrap{display:flex; align-items:center; justify-content:space-between; height:64px;}
.brand{font-family:'Bricolage Grotesque',sans-serif; font-weight:800; font-size:1.15rem; letter-spacing:-.02em;}
.brand span{color:var(--coral);}
nav .links{display:flex; gap:26px; font-size:.92rem; font-weight:500;}
nav .links a{text-decoration:none; opacity:.85;}
nav .links a:hover{opacity:1;}
.btn{display:inline-block; background:var(--coral); color:#fff; padding:10px 20px; border-radius:100px; font-weight:600; font-size:.9rem; text-decoration:none; border:none; cursor:pointer;}
.btn:hover{background:#d24b3a;}
.btn-ghost{background:transparent; border:1.5px solid var(--ink); color:var(--ink);}

/* HERO */
.hero{position:relative; padding:64px 0 0; overflow:hidden;}
.hero .wrap{display:grid; grid-template-columns:1.1fr .9fr; gap:40px; align-items:center; padding-bottom:60px;}
.eyebrow{font-size:.95rem; color:var(--turquoise); font-weight:600; margin-bottom:14px;}
.hero h1{font-size:clamp(2.4rem,5vw,3.6rem); line-height:1.04; font-weight:800; letter-spacing:-.02em; max-width:11ch;}
.hero p.lede{margin-top:20px; font-size:1.1rem; line-height:1.6; max-width:42ch; color:#2a4b47;}
.hero .cta-row{margin-top:30px; display:flex; gap:14px; flex-wrap:wrap;}
.slogan{margin-top:38px; font-family:'Bricolage Grotesque'; font-style:italic; font-weight:600; color:var(--sea-deep); font-size:1rem;}

.horizon{position:relative; height:340px;}
.horizon svg{width:100%; height:100%;}

.wave-divider{width:100%; display:block; line-height:0;}
.wave-divider svg{width:100%; height:60px; display:block;}

/* SEA-DEEP SECTION */
.deep{background:var(--sea-deep); color:var(--sand); padding:70px 0;}
.deep h2{color:#fff;}

/* SECTION HEADER */
.section-head{max-width:52ch; margin-bottom:44px;}
.section-head h2{font-size:clamp(1.7rem,3vw,2.3rem); font-weight:800; letter-spacing:-.01em; line-height:1.15;}
.section-head p{margin-top:14px; font-size:1.02rem; line-height:1.6; opacity:.85;}

section{padding:76px 0;}

/* THREE LEVELS — nested rings, echoing the source model */
.rings-block{display:grid; grid-template-columns:.9fr 1.1fr; gap:50px; align-items:center;}
.rings{position:relative; width:100%; aspect-ratio:1/1; max-width:420px; margin:0 auto;}
.ring{position:absolute; border-radius:50%; display:flex; align-items:center; justify-content:center; text-align:center;}
.ring.r1{inset:0; background:radial-gradient(circle at 30% 30%, #f6d38b, var(--gold)); }
.ring.r2{inset:16%; background:radial-gradient(circle at 30% 30%, #57b0ba, var(--turquoise));}
.ring.r3{inset:35%; background:radial-gradient(circle at 30% 30%, #175c5e, var(--sea-deep)); color:#fff; font-weight:700; font-size:.95rem; padding:10px;}
.ring-label{position:absolute; font-size:.72rem; font-weight:600; color:var(--ink); background:var(--sand); padding:4px 10px; border-radius:100px; border:1px solid rgba(18,48,46,.15);}
.lbl1{top:-6px; left:50%; transform:translateX(-50%);}
.lbl2{bottom:8%; left:2%;}
.lbl3{bottom:8%; right:2%;}

.level-list{display:flex; flex-direction:column; gap:22px;}
.level{border-left:3px solid var(--turquoise); padding-left:20px;}
.level.core{border-color:var(--sea-deep);}
.level.aug{border-color:var(--gold);}
.level h3{font-size:1.15rem; font-weight:700; margin-bottom:6px;}
.level p{font-size:.96rem; line-height:1.55; opacity:.85; max-width:46ch;}

/* TOUR CARD */
.tour-panel{background:#fff; border:1px solid rgba(18,48,46,.12); border-radius:20px; padding:0; overflow:hidden; display:grid; grid-template-columns:1.1fr 1fr;}
.tour-info{padding:38px;}
.tour-info h3{font-size:1.5rem; font-weight:800; margin-bottom:8px;}
.tour-info .price{font-size:2rem; font-weight:800; color:var(--coral); margin:14px 0 4px;}
.tour-info .price small{font-size:.9rem; font-weight:500; color:var(--ink); opacity:.7;}
.feature-list{list-style:none; margin-top:22px; display:flex; flex-direction:column; gap:10px;}
.feature-list li{display:flex; gap:10px; font-size:.95rem; align-items:flex-start;}
.check{flex:none; width:18px; height:18px; border-radius:50%; background:var(--turquoise); color:#fff; font-size:.65rem; display:flex; align-items:center; justify-content:center; margin-top:2px;}
.tour-visual{background:linear-gradient(160deg, var(--turquoise), var(--sea-deep)); position:relative;}
.tour-visual svg{width:100%; height:100%;}

/* GUIDES / CARE */
.grid3{display:grid; grid-template-columns:repeat(3,1fr); gap:26px;}
.pillar{padding:26px 0;}
.pillar .num{font-family:'Bricolage Grotesque'; font-weight:800; font-size:1rem; color:var(--coral);}
.pillar h3{font-size:1.15rem; font-weight:700; margin:10px 0 8px;}
.pillar p{font-size:.94rem; line-height:1.55; opacity:.8;}

/* SOUVENIR */
.souvenir{background:var(--ink); color:var(--sand); border-radius:24px; padding:50px; display:grid; grid-template-columns:1fr 1fr; gap:40px; align-items:center;}
.souvenir h2{color:#fff; font-size:1.9rem;}
.souvenir p{margin-top:16px; line-height:1.6; opacity:.85; max-width:44ch;}
.magsafe{position:relative; aspect-ratio:1/1; display:flex; align-items:center; justify-content:center;}
.magsafe svg{width:80%; height:80%;}

/* TESTIMONIAL STRIP */
.strip{background:var(--gold); color:var(--ink); padding:44px 0;}
.strip .wrap{display:flex; gap:40px; flex-wrap:wrap; align-items:center; justify-content:space-between;}
.stat{text-align:left;}
.stat b{font-family:'Bricolage Grotesque'; font-size:2.1rem; font-weight:800; display:block;}
.stat span{font-size:.85rem; opacity:.8;}

/* CTA */
.cta-block{text-align:center; padding:90px 0;}
.cta-block h2{font-size:clamp(1.8rem,4vw,2.6rem); max-width:16ch; margin:0 auto 18px;}
.cta-block p{max-width:44ch; margin:0 auto 30px; opacity:.8; line-height:1.6;}

footer{background:var(--sea-deep); color:var(--sand); padding:44px 0 30px;}
footer .wrap{display:flex; justify-content:space-between; flex-wrap:wrap; gap:20px; font-size:.88rem;}
footer .foot-brand{font-family:'Bricolage Grotesque'; font-weight:800; font-size:1.1rem; color:#fff; margin-bottom:8px;}
footer .cols{display:flex; gap:60px; flex-wrap:wrap;}
footer a{opacity:.8; text-decoration:none;}
.fine{margin-top:30px; opacity:.55; font-size:.78rem; border-top:1px solid rgba(255,255,255,.12); padding-top:18px;}

@media(max-width:820px){
  .hero .wrap{grid-template-columns:1fr;}
  .horizon{height:220px; order:-1;}
  .rings-block{grid-template-columns:1fr;}
  .tour-panel{grid-template-columns:1fr;}
  .tour-visual{height:200px;}
  .grid3{grid-template-columns:1fr;}
  .souvenir{grid-template-columns:1fr; padding:34px;}
  nav .links{display:none;}
}
@media (prefers-color-scheme: dark){
  :root:not([data-theme="light"]){ }
}
</style>
</head>
<body>

<nav>
  <div class="wrap">
    <div class="brand">Golden<span>Smile</span></div>
    <div class="links">
      <a href="#story">Câu chuyện</a>
      <a href="#tour">Tour</a>
      <a href="#guides">Đội ngũ</a>
      <a href="#souvenir">Quà lưu niệm</a>
    </div>
    <a href="#book" class="btn">Đặt tour</a>
  </div>
</nav>

<header class="hero">
  <div class="wrap">
    <div>
      <div class="eyebrow">Khám phá đảo hoang · Nha Trang</div>
      <h1>Những hòn đảo mà bản đồ du lịch chưa từng ghi tên.</h1>
      <p class="lede">Golden Smile đưa bạn đến 3 hòn đảo ít người biết ngoài khơi Nha Trang trong một ngày — không tàu đông, không lịch trình dàn dựng, chỉ có biển thật và những câu chuyện thật.</p>
      <div class="cta-row">
        <a href="#book" class="btn">Đặt chỗ ngay — 750K₫</a>
        <a href="#story" class="btn btn-ghost">Xem hành trình</a>
      </div>
      <div class="slogan">"One day. One trip. One story."</div>
    </div>
    <div class="horizon">
      <svg viewBox="0 0 400 340" xmlns="http://www.w3.org/2000/svg">
        <circle cx="300" cy="70" r="46" fill="#E8A33D"/>
        <path d="M0 210 Q 60 190 120 210 T 240 210 T 400 210 V340 H0 Z" fill="#2C8C99"/>
        <path d="M0 250 Q 70 230 140 250 T 280 250 T 400 250 V340 H0 Z" fill="#175c5e" opacity="0.7"/>
        <path d="M40 205 L60 180 L85 205 Z" fill="#0E4749"/>
        <path d="M250 208 L280 170 L315 208 Z" fill="#12302E"/>
        <path d="M180 105 L188 130 L178 130 L182 150 L160 122 L170 122 Z" fill="#0E4749" opacity=".85"/>
      </svg>
    </div>
  </div>
  <div class="wave-divider">
    <svg viewBox="0 0 1440 60" preserveAspectRatio="none"><path d="M0 30 Q 360 60 720 30 T 1440 30 V60 H0 Z" fill="#0E4749"/></svg>
  </div>
</header>

<section class="deep" id="story">
  <div class="wrap">
    <div class="section-head">
      <h2>Sản phẩm cốt lõi không phải là chuyến tàu — mà là cảm giác khám phá.</h2>
      <p style="color:#cfe6df;">Khách hàng không mua vé tàu ra đảo. Họ mua lại cảm giác đặt chân lên một bãi cát chưa ai chụp ảnh, được kể một câu chuyện làng chài chưa lên Google. Đó là điều mọi hành trình của Golden Smile phải giữ vững.</p>
    </div>

    <div class="rings-block">
      <div class="rings">
        <div class="ring r1"></div>
        <div class="ring r2"></div>
        <div class="ring r3">Khám phá &<br>trải nghiệm</div>
        <div class="ring-label lbl1">Augmented</div>
        <div class="ring-label lbl2">Tangible</div>
        <div class="ring-label lbl3">Core</div>
      </div>
      <div class="level-list">
        <div class="level core">
          <h3>Lõi sản phẩm</h3>
          <p>Cảm giác khám phá — trải nghiệm chân thực tại những hòn đảo ít người biết ở Nha Trang.</p>
        </div>
        <div class="level">
          <h3>Sản phẩm hữu hình</h3>
          <p>Tour 1 ngày khởi hành sớm đến 3 đảo ẩn, giá 700K–800K₫/người, hướng dẫn viên song ngữ EN/VN, tàu đúng giờ và an toàn.</p>
        </div>
        <div class="level aug">
          <h3>Sản phẩm tăng cường</h3>
          <p>Đặt tour qua Klook/Traveloka/website, thanh toán MoMo/VNPay, hủy linh hoạt, chăm sóc sau tour qua Zalo OA, ưu đãi loyalty 10% cho lần sau.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="tour">
  <div class="wrap">
    <div class="section-head">
      <h2>Một hành trình, giá rõ ràng, không phụ phí ẩn.</h2>
      <p>Golden Smile giữ giá thân thiện với người trẻ và khách quốc tế đi lẻ, nhưng không cắt giảm trải nghiệm.</p>
    </div>
    <div class="tour-panel">
      <div class="tour-info">
        <div style="font-size:.85rem; color:var(--turquoise); font-weight:600;">TOUR 3 ĐẢO ẨN</div>
        <h3>Khám phá đảo hoang một ngày</h3>
        <div class="price">750.000₫ <small>/ người</small></div>
        <ul class="feature-list">
          <li><span class="check">✓</span> Khởi hành sớm, tránh đoàn đông</li>
          <li><span class="check">✓</span> Hướng dẫn viên song ngữ, giàu kinh nghiệm địa phương</li>
          <li><span class="check">✓</span> Nhóm nhỏ, tàu đúng giờ, an toàn</li>
          <li><span class="check">✓</span> Chăm sóc tour trước – trong – sau chuyến đi</li>
          <li><span class="check">✓</span> Quà lưu niệm MagSafe kỷ niệm hành trình</li>
        </ul>
        <div class="cta-row" style="margin-top:24px;">
          <a href="#book" class="btn">Đặt tour này</a>
        </div>
      </div>
      <div class="tour-visual">
        <svg viewBox="0 0 300 300" xmlns="http://www.w3.org/2000/svg">
          <circle cx="150" cy="150" r="150" fill="#123e40"/>
          <path d="M0 190 Q 75 170 150 190 T 300 190 V300 H0 Z" fill="#175c5e"/>
          <path d="M60 175 L90 130 L120 175 Z" fill="#F2E8D5" opacity=".9"/>
          <path d="M170 180 L200 145 L235 180 Z" fill="#F2E8D5" opacity=".7"/>
          <circle cx="230" cy="70" r="26" fill="#E8A33D"/>
        </svg>
      </div>
    </div>
  </div>
</section>

<section id="guides" style="background:#eadfc4;">
  <div class="wrap">
    <div class="section-head">
      <h2>Đối thủ cạnh tranh ở giá và tàu. Golden Smile thắng ở con người.</h2>
      <p>Ba trụ cột giữ khách quay lại — không phải giảm giá thêm.</p>
    </div>
    <div class="grid3">
      <div class="pillar">
        <div class="num">Hướng dẫn viên</div>
        <h3>Am hiểu, song ngữ, kể chuyện thật</h3>
        <p>Không đọc kịch bản — hướng dẫn viên là người địa phương, kể chuyện làng chài và lịch sử đảo bằng trải nghiệm của chính họ.</p>
      </div>
      <div class="pillar">
        <div class="num">Chăm sóc tour</div>
        <h3>Đồng hành trước và sau chuyến đi</h3>
        <p>Nhắc lịch qua Zalo OA, hỗ trợ thời tiết/đổi lịch linh hoạt, và một tin nhắn cảm ơn kèm mã ưu đãi sau khi khách về đất liền.</p>
      </div>
      <div class="pillar">
        <div class="num">Cộng đồng</div>
        <h3>UGC thật, không dàn dựng</h3>
        <p>Khuyến khích khách đăng khoảnh khắc thật lên TikTok/Threads, tag để được repost — quảng cáo tốt nhất đến từ chính khách hàng.</p>
      </div>
    </div>
  </div>
</section>

<section id="souvenir">
  <div class="wrap">
    <div class="souvenir">
      <div>
        <div class="eyebrow" style="color:#E8A33D;">QUÀ LƯU NIỆM</div>
        <h2>Một tấm MagSafe, một ký ức cầm được.</h2>
        <p>Mỗi khách kết thúc hành trình với một chiếc ốp MagSafe khắc ảnh hoặc tọa độ hòn đảo đã ghé — vật kỷ niệm nhỏ nhắc lại một ngày không giống bất kỳ tour nào khác.</p>
        <a href="#book" class="btn" style="margin-top:22px; display:inline-block;">Tìm hiểu về bộ quà tặng</a>
      </div>
      <div class="magsafe">
        <svg viewBox="0 0 200 300" xmlns="http://www.w3.org/2000/svg">
          <rect x="10" y="10" width="180" height="280" rx="28" fill="#1c4a48" stroke="#F2E8D5" stroke-width="2"/>
          <circle cx="100" cy="150" r="46" fill="none" stroke="#E8A33D" stroke-width="3" stroke-dasharray="6 6"/>
          <path d="M75 150 Q 100 120 125 150 Q 100 180 75 150 Z" fill="#E8A33D"/>
          <circle cx="100" cy="150" r="6" fill="#0E4749"/>
        </svg>
      </div>
    </div>
  </div>
</section>

<div class="strip">
  <div class="wrap">
    <div class="stat"><b>3</b><span>hòn đảo ẩn khám phá mỗi hành trình</span></div>
    <div class="stat"><b>4.3★</b><span>đánh giá trung bình mục tiêu</span></div>
    <div class="stat"><b>&lt;24h</b><span>thời gian phản hồi mọi đánh giá</span></div>
    <div class="stat"><b>10%</b><span>ưu đãi loyalty cho lần đặt tiếp theo</span></div>
  </div>
</div>

<section class="cta-block" id="book">
  <div class="wrap">
    <h2>Sẵn sàng cho một ngày không nằm trong bản đồ du lịch?</h2>
    <p>Đặt chỗ qua Klook, Traveloka hoặc trực tiếp tại đây để nhận ưu đãi 10% cho lần đặt đầu tiên.</p>
    <div class="cta-row" style="justify-content:center;">
      <a href="#" class="btn">Đặt tour trên Klook</a>
      <a href="#" class="btn btn-ghost">Nhắn Zalo OA</a>
    </div>
  </div>
</section>

<footer>
  <div class="wrap">
    <div>
      <div class="foot-brand">Golden Smile</div>
      <div style="opacity:.8; max-width:32ch;">Tour khám phá đảo hoang tại Nha Trang. "One day. One trip. One story."</div>
    </div>
    <div class="cols">
      <div>
        <div style="font-weight:600; margin-bottom:8px; color:#fff;">Liên hệ</div>
        <div><a href="#">Zalo OA</a></div>
        <div><a href="#">Instagram</a></div>
        <div><a href="#">TikTok</a></div>
      </div>
      <div>
        <div style="font-weight:600; margin-bottom:8px; color:#fff;">Đặt tour</div>
        <div><a href="#">Klook</a></div>
        <div><a href="#">Traveloka</a></div>
        <div><a href="#book">Website</a></div>
      </div>
    </div>
  </div>
  <div class="wrap fine">© 2026 Golden Smile Tours, Nha Trang. Trang minh họa cho mục đích thuyết trình.</div>
</footer>

</body>
</html>
