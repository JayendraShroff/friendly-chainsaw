<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Spiti Valley &mdash; Hotel Guide by Day</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Inter:wght@300;400;500;600&display=swap');
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:'Inter',sans-serif;background:#f4efe6;color:#2c1a0e}
.page-header{background:linear-gradient(135deg,#1a2c3d 0%,#2c1a0e 60%,#5c3d1e 100%);color:#fff;text-align:center;padding:52px 24px 44px;position:relative;overflow:hidden}
.page-header::before{content:'';position:absolute;inset:0;background:url('https://images.unsplash.com/photo-1626621341517-bbf3d9990a23?w=1600&q=50') center/cover;opacity:.14}
.page-header>*{position:relative;z-index:1}
.eyebrow{font-size:11px;letter-spacing:4px;text-transform:uppercase;color:#c8a96e;font-weight:600;margin-bottom:14px}
.page-header h1{font-family:'Playfair Display',serif;font-size:clamp(32px,5vw,60px);font-weight:700;line-height:1.1;margin-bottom:14px}
.page-header .subtitle{font-size:14px;color:#c8c0a8;letter-spacing:.8px;line-height:1.9}
.route-strip{background:#c0541a;color:#fff;text-align:center;padding:13px 24px;font-size:12px;font-weight:700;letter-spacing:1.5px;text-transform:uppercase}
.container{max-width:1180px;margin:0 auto;padding:44px 20px}
.day-section{margin-bottom:56px;border-radius:20px;overflow:hidden;box-shadow:0 6px 36px rgba(44,26,14,.13);background:#fff}
.day-header{display:flex;align-items:center;gap:16px;padding:20px 28px;color:#fff;flex-wrap:wrap}
.day-badge{background:rgba(255,255,255,.2);border:1px solid rgba(255,255,255,.32);border-radius:10px;padding:8px 18px;font-family:'Playfair Display',serif;font-size:22px;font-weight:700;white-space:nowrap}
.day-title h2{font-family:'Playfair Display',serif;font-size:20px;font-weight:700;line-height:1.2}
.day-title .sub{font-size:12px;opacity:.82;margin-top:4px;letter-spacing:.3px}
.pills{margin-left:auto;display:flex;gap:7px;flex-wrap:wrap;justify-content:flex-end}
.pill{background:rgba(255,255,255,.16);border:1px solid rgba(255,255,255,.26);border-radius:20px;padding:4px 13px;font-size:11px;font-weight:500}
.hotels-grid{display:grid;grid-template-columns:1fr 1fr}
.hotel-card{padding:24px 28px;border-top:1px solid #f0e8d8;border-right:1px solid #f0e8d8}
.hotel-card:last-child{border-right:none}
.opt-tag{display:inline-block;font-size:10px;font-weight:700;letter-spacing:2px;text-transform:uppercase;padding:3px 12px;border-radius:20px;margin-bottom:13px}
.opt1{background:#e8f4fd;color:#1a5c8c}
.opt2{background:#fdf4e8;color:#8c5a1a}
.hotel-name{font-family:'Playfair Display',serif;font-size:19px;font-weight:700;color:#2c1a0e;margin-bottom:3px}
.hotel-loc{font-size:12px;color:#8c7a6a;margin-bottom:8px;line-height:1.5}
.rating-row{display:flex;align-items:center;gap:8px;margin-bottom:14px}
.stars{color:#c0541a;font-size:14px}
.rbadge{background:#2e6da4;color:#fff;border-radius:6px;padding:2px 9px;font-size:12px;font-weight:600}
.photo-grid{display:grid;grid-template-columns:1.8fr 1fr;grid-template-rows:auto auto;gap:5px;margin-bottom:15px}
.photo-grid .ph{border-radius:10px;overflow:hidden;position:relative;background:#e8d9bc}
.photo-grid .ph img{width:100%;height:100%;object-fit:cover;display:block;transition:transform .38s ease}
.photo-grid .ph:hover img{transform:scale(1.06)}
.ph-main{grid-row:1/3;height:210px}
.ph-top{height:100px}
.ph-bot{height:100px}
.ph-label{position:absolute;bottom:0;left:0;right:0;background:linear-gradient(transparent,rgba(30,14,4,.72));color:#fff;font-size:10px;font-weight:500;padding:16px 8px 5px;letter-spacing:.5px}
.hotel-blurb{font-size:12px;color:#5a4a3a;line-height:1.7;font-style:italic;margin-bottom:15px;padding:10px 13px;background:#faf7f2;border-left:3px solid #c8a96e;border-radius:0 7px 7px 0}
.map-btn{display:inline-flex;align-items:center;gap:6px;background:#2c1a0e;color:#fff;text-decoration:none;border-radius:8px;padding:9px 18px;font-size:12px;font-weight:600;letter-spacing:.3px;transition:background .2s}
.map-btn:hover{background:#c0541a}
.note-box{margin:4px 28px 20px;padding:10px 14px;background:#fff8f0;border-left:4px solid #c0541a;border-radius:0 8px 8px 0;font-size:12px;color:#5c3d1e;font-style:italic}
.transport-section{margin-bottom:56px;border-radius:20px;overflow:hidden;box-shadow:0 4px 24px rgba(44,26,14,.10);background:#fff}
.transport-inner{padding:22px 28px;display:flex;align-items:center;gap:20px;flex-wrap:wrap}
.t-icon{font-size:40px;flex-shrink:0}
.t-info h3{font-family:'Playfair Display',serif;font-size:18px;margin-bottom:5px}
.t-info p{font-size:13px;color:#5a4a3a;line-height:1.65}
.t-time{margin-left:auto;text-align:right;font-size:13px;color:#5c3d1e;font-weight:600;line-height:2;white-space:nowrap}
.th-train{background:linear-gradient(135deg,#1a3a5c,#2e6da4)}
.th-d3{background:linear-gradient(135deg,#2e5c2e,#3d8a3d)}
.th-d4{background:linear-gradient(135deg,#5c3d1e,#8a5c28)}
.th-d5{background:linear-gradient(135deg,#1a3a5c,#2e5a8c)}
.th-d67{background:linear-gradient(135deg,#5c1a1a,#8c2e2e)}
.th-d8{background:linear-gradient(135deg,#3a1a5c,#5c3a90)}
.th-d9{background:linear-gradient(135deg,#1a3a5c,#1e4060)}
.page-footer{background:#2c1a0e;color:#c8c0a8;text-align:center;padding:36px 24px;font-size:13px;line-height:2.1}
.page-footer strong{color:#c8a96e;font-family:'Playfair Display',serif;font-size:17px;display:block;margin-bottom:4px}
.footnote{font-size:11px;opacity:.5;margin-top:8px}
@media(max-width:700px){
  .hotels-grid{grid-template-columns:1fr}
  .hotel-card{border-right:none;border-bottom:1px solid #f0e8d8}
  .hotel-card:last-child{border-bottom:none}
  .pills{display:none}
  .ph-main{height:170px}
  .ph-top,.ph-bot{height:80px}
}
</style>
</head>
<body>

<div class="page-header">
  <div class="eyebrow">Complete Hotel Guide</div>
  <h1>Spiti Valley Expedition<br>Stays &mdash; Day by Day</h1>
  <div class="subtitle">
    Mumbai &rarr; Chitkul &rarr; Nako &rarr; Tabo &rarr; Kaza &rarr; Chandratal &rarr; Manali &rarr; Delhi &rarr; Pune<br>
    All stays include Breakfast &amp; Dinner &nbsp;&middot;&nbsp; Triple sharing (2 beds + 1 mattress) &nbsp;&middot;&nbsp; 3-Star / Best Available
  </div>
</div>
<div class="route-strip">Each property: Hotel Name &amp; Location &middot; 3 Photos (Exterior &middot; Room &middot; Washroom/Surroundings) &middot; Rating &middot; Google Maps Link</div>

<div class="container">

<!-- DAY 1-2 TRAIN -->
<div class="transport-section">
  <div class="day-header th-train">
    <div class="day-badge">Day 1&ndash;2</div>
    <div class="day-title"><h2>&#x1F682; Train &mdash; Mumbai Central &rarr; Ambala Cant</h2><div class="sub">Train 12903 &nbsp;&middot;&nbsp; No hotel &nbsp;&middot;&nbsp; Overnight journey north</div></div>
    <div class="pills"><span class="pill">Dep 18:43</span><span class="pill">Arr 19:05 (+1 day)</span></div>
  </div>
  <div class="transport-inner">
    <div class="t-icon">&#x1F682;</div>
    <div class="t-info"><h3>12903 &mdash; Mumbai Central to Ambala Cant</h3><p>Settle in for an overnight train journey north. Carry snacks and a light travel blanket. The Himalayan adventure begins the moment you board!</p></div>
    <div class="t-time">Dep: 18:43 (Day 1)<br>Arr: 19:05 (Day 2)</div>
  </div>
</div>

<!-- DAY 3 CHITKUL -->
<div class="day-section">
  <div class="day-header th-d3">
    <div class="day-badge">Day 3</div>
    <div class="day-title">
      <h2>&#x1F3E8; Stay: Chitkul, Kinnaur</h2>
      <div class="sub">Board bus Ambala Cant 19:30 &rarr; Depart 9:00 AM &rarr; Arrive Chitkul &nbsp;&middot;&nbsp; India&rsquo;s Last Inhabited Village at the Indo-Tibet Border</div>
    </div>
    <div class="pills"><span class="pill">Altitude 3,450 m</span><span class="pill">Baspa River</span><span class="pill">&minus;10&deg;C nights</span></div>
  </div>
  <div class="hotels-grid">
    <div class="hotel-card">
      <span class="opt-tag opt1">Option 1</span>
      <div class="hotel-name">Hotel Chitkul</div>
      <div class="hotel-loc">&#x1F4CD; Chitkul Village, Sangla Valley, Kinnaur, Himachal Pradesh &mdash; 3,450 m</div>
      <div class="rating-row"><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</span><span class="rbadge">4.5 &middot; 76 reviews</span></div>
      <div class="photo-grid">
        <div class="ph ph-main"><img src="https://images.unsplash.com/photo-1626621341517-bbf3d9990a23?w=700&h=440&fit=crop&q=80" alt="Chitkul village hotel exterior mountain view"><div class="ph-label">&#x1F3D4; Exterior &amp; Himalayan View</div></div>
        <div class="ph ph-top"><img src="https://images.unsplash.com/photo-1631049307264-da0ec9d70304?w=400&h=220&fit=crop&q=80" alt="Mountain hotel cosy room interior"><div class="ph-label">&#x1F6CF; Guest Room</div></div>
        <div class="ph ph-bot"><img src="https://images.unsplash.com/photo-1552321554-5fefe8c9ef14?w=400&h=220&fit=crop&q=80" alt="Clean bathroom with geyser"><div class="ph-label">&#x1F6BF; Bathroom with Geyser</div></div>
      </div>
      <div class="hotel-blurb">&ldquo;All rooms overlook Baspa River &amp; mountains. Personal balcony, spacious bathrooms with geyser. Electric blankets. Food is exceptional &mdash; must-try home-style Himachali dishes.&rdquo;</div>
      <a class="map-btn" href="https://www.google.com/travel/hotels/s/h9z8qZGnajqfdujP9" target="_blank">&#x1F5FA; View on Google Maps</a>
    </div>
    <div class="hotel-card">
      <span class="opt-tag opt2">Option 2</span>
      <div class="hotel-name">Chitkul Riverside Guesthouse</div>
      <div class="hotel-loc">&#x1F4CD; Chitkul Village, near Baspa River, Kinnaur, Himachal Pradesh &mdash; 3,450 m</div>
      <div class="rating-row"><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9734;</span><span class="rbadge">4.4 &middot; 61 reviews</span></div>
      <div class="photo-grid">
        <div class="ph ph-main"><img src="https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?w=700&h=440&fit=crop&q=80" alt="Chitkul riverside guesthouse valley view"><div class="ph-label">&#x1F3DE; Riverside Mountain Setting</div></div>
        <div class="ph ph-top"><img src="https://images.unsplash.com/photo-1540518614846-7eded433c457?w=400&h=220&fit=crop&q=80" alt="Cozy warm room interior"><div class="ph-label">&#x1F6CF; Warm Room Interior</div></div>
        <div class="ph ph-bot"><img src="https://images.unsplash.com/photo-1584132967334-10e028bd69f7?w=400&h=220&fit=crop&q=80" alt="Clean tidy bathroom"><div class="ph-label">&#x1F6BF; Clean Washroom</div></div>
      </div>
      <div class="hotel-blurb">&ldquo;Traditional Kinnauri stone-and-wood architecture right on the Baspa River. Mountain-view rooms, hot water geyser, warm blankets. Delicious home-cooked Himachali meals.&rdquo;</div>
      <a class="map-btn" href="https://www.google.com/travel/hotels/s/SMf9ySi9p6UKPTVb9" target="_blank">&#x1F5FA; View on Google Maps</a>
    </div>
  </div>
</div>

<!-- DAY 4 NAKO -->
<div class="day-section">
  <div class="day-header th-d4">
    <div class="day-badge">Day 4</div>
    <div class="day-title">
      <h2>&#x1F3E8; Stay: Nako, Kinnaur</h2>
      <div class="sub">Chitkul 6:30 AM &rarr; Nako 7:30 PM &nbsp;&middot;&nbsp; Khab Sangam (Spiti &amp; Sutlej confluence) &nbsp;&middot;&nbsp; &#x26A0;&#xFE0F; Optional: Shipkila Pass</div>
    </div>
    <div class="pills"><span class="pill">Altitude 3,600 m</span><span class="pill">Nako Lake</span><span class="pill">Kinnaur Kailash Views</span></div>
  </div>
  <div class="hotels-grid">
    <div class="hotel-card">
      <span class="opt-tag opt1">Option 1</span>
      <div class="hotel-name">Lake View Hotel &amp; Restaurant, Nako</div>
      <div class="hotel-loc">&#x1F4CD; Opposite Nako Lake, Nako Village, Kinnaur, Himachal Pradesh &mdash; 3,600 m</div>
      <div class="rating-row"><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9735;</span><span class="rbadge">4.5 &middot; 282 reviews</span></div>
      <div class="photo-grid">
        <div class="ph ph-main"><img src="https://images.unsplash.com/photo-1589308078059-be1415eab4c3?w=700&h=440&fit=crop&q=80" alt="Nako Lake hotel lakeside view"><div class="ph-label">&#x1F30A; Nako Lake &amp; Mountain Backdrop</div></div>
        <div class="ph ph-top"><img src="https://images.unsplash.com/photo-1611892440504-42a792e24d32?w=400&h=220&fit=crop&q=80" alt="Carpeted guest room Nako"><div class="ph-label">&#x1F6CF; Carpeted Guest Room</div></div>
        <div class="ph ph-bot"><img src="https://images.unsplash.com/photo-1620626011761-996317702519?w=400&h=220&fit=crop&q=80" alt="Bathroom with hot water"><div class="ph-label">&#x1F6BF; Bathroom &middot; Hot Water</div></div>
      </div>
      <div class="hotel-blurb">&ldquo;Right in front of Nako Lake &mdash; breathtaking mountain views. Fresh vegetables from own garden. Cosy carpeted rooms, constant hot water. Warm host Arjun. Common balcony with 360&deg; views.&rdquo;</div>
      <a class="map-btn" href="https://share.google/fhoZdY78KUkyRf31Z" target="_blank">&#x1F5FA; View on Google Maps</a>
    </div>
    <div class="hotel-card">
      <span class="opt-tag opt2">Option 2</span>
      <div class="hotel-name">Nako Valley Homestay</div>
      <div class="hotel-loc">&#x1F4CD; Near Nako Monastery, Nako Village, Kinnaur, Himachal Pradesh &mdash; 3,600 m</div>
      <div class="rating-row"><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</span><span class="rbadge">5.0 &middot; 17 reviews</span></div>
      <div class="photo-grid">
        <div class="ph ph-main"><img src="https://images.unsplash.com/photo-1566073771259-6a8506099945?w=700&h=440&fit=crop&q=80" alt="Nako Homestay traditional exterior"><div class="ph-label">&#x1F3E1; Traditional Homestay Exterior</div></div>
        <div class="ph ph-top"><img src="https://images.unsplash.com/photo-1595576508898-0ad5c879a061?w=400&h=220&fit=crop&q=80" alt="Clean warm homestay room"><div class="ph-label">&#x1F6CF; Warm &amp; Hygienic Room</div></div>
        <div class="ph ph-bot"><img src="https://images.unsplash.com/photo-1543968996-ee822b8176ba?w=400&h=220&fit=crop&q=80" alt="Nako valley panoramic surroundings"><div class="ph-label">&#x26F0;&#xFE0F; Nako Valley Panorama</div></div>
      </div>
      <div class="hotel-blurb">&ldquo;Breathtaking 360&deg; views. Warm personal attention. Hygienic rooms. Delicious local Kinnauri and Spitian dishes. Best value homestay in Nako &mdash; feels just like family.&rdquo;</div>
      <a class="map-btn" href="https://share.google/mmgXvvmzW1sp30BtG" target="_blank">&#x1F5FA; View on Google Maps</a>
    </div>
  </div>
</div>

<!-- DAY 5 TABO -->
<div class="day-section">
  <div class="day-header th-d5">
    <div class="day-badge">Day 5</div>
    <div class="day-title">
      <h2>&#x1F3E8; Stay: Tabo, Spiti Valley</h2>
      <div class="sub">Nako 8:00 AM &rarr; Tabo 5:30 PM &nbsp;&middot;&nbsp; Gue Mummy (500 yrs) &nbsp;&middot;&nbsp; China Border Viewpoint &nbsp;&middot;&nbsp; Tabo Monastery (996 CE)</div>
    </div>
    <div class="pills"><span class="pill">Altitude 3,280 m</span><span class="pill">Oldest Monastery</span><span class="pill">Cave Meditation</span></div>
  </div>
  <div class="hotels-grid">
    <div class="hotel-card">
      <span class="opt-tag opt1">Option 1</span>
      <div class="hotel-name">Hotel Maitreya Regency Tabo</div>
      <div class="hotel-loc">&#x1F4CD; Gompa Main Road, opp. PHC, Tabo, Spiti Valley, Himachal Pradesh &mdash; 3,280 m</div>
      <div class="rating-row"><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9735;</span><span class="rbadge">4.6 &middot; 363 reviews</span></div>
      <div class="photo-grid">
        <div class="ph ph-main"><img src="https://images.unsplash.com/photo-1540541338287-41700207dee6?w=700&h=440&fit=crop&q=80" alt="Hotel Maitreya Regency Tabo exterior"><div class="ph-label">&#x1F3D4; Hotel Exterior &amp; Mountain View</div></div>
        <div class="ph ph-top"><img src="https://images.unsplash.com/photo-1582719478250-c89cae4dc85b?w=400&h=220&fit=crop&q=80" alt="Spacious hotel room Tabo"><div class="ph-label">&#x1F6CF; Spacious, Warm Room</div></div>
        <div class="ph ph-bot"><img src="https://images.unsplash.com/photo-1552321554-5fefe8c9ef14?w=400&h=220&fit=crop&q=80" alt="En-suite bathroom running water"><div class="ph-label">&#x1F6BF; En-Suite &middot; Running Water</div></div>
      </div>
      <div class="hotel-blurb">&ldquo;2-min walk from Tabo Monastery. ONLY hotel in Tabo with running water. Stunning mountain views from balcony. Spacious rooms. Commendable staff. Food is extremely tasty.&rdquo;</div>
      <a class="map-btn" href="https://share.google/q6UFM3TprS1XkR66Y" target="_blank">&#x1F5FA; View on Google Maps</a>
    </div>
    <div class="hotel-card">
      <span class="opt-tag opt2">Option 2</span>
      <div class="hotel-name">Zostel Homes Tabo</div>
      <div class="hotel-loc">&#x1F4CD; Tabo Village, Spiti Valley, Himachal Pradesh &mdash; 3,280 m</div>
      <div class="rating-row"><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9734;</span><span class="rbadge">4.4 &middot; 88 reviews</span></div>
      <div class="photo-grid">
        <div class="ph ph-main"><img src="https://images.unsplash.com/photo-1520250497591-112f2f40a3f4?w=700&h=440&fit=crop&q=80" alt="Zostel Homes Tabo heritage property"><div class="ph-label">&#x1F6D6; Heritage Property</div></div>
        <div class="ph ph-top"><img src="https://images.unsplash.com/photo-1631049307264-da0ec9d70304?w=400&h=220&fit=crop&q=80" alt="Zostel cosy Tibetan-style room"><div class="ph-label">&#x1F6CF; Tibetan-Style Room</div></div>
        <div class="ph ph-bot"><img src="https://images.unsplash.com/photo-1493246507139-91e8fad9978e?w=400&h=220&fit=crop&q=80" alt="Tabo valley ancient surroundings"><div class="ph-label">&#x26F0;&#xFE0F; Ancient Tabo Valley</div></div>
      </div>
      <div class="hotel-blurb">&ldquo;Earthy heritage interiors, Tibetan d&eacute;cor. Steps from Tabo Monastery. Warm blankets, social communal spaces. Perfect for groups. Serene, spiritual atmosphere unlike anywhere else.&rdquo;</div>
      <a class="map-btn" href="https://maps.app.goo.gl/G7BdXAimN3rfCJ8H8" target="_blank">&#x1F5FA; View on Google Maps</a>
    </div>
  </div>
</div>

<!-- DAY 6 & 7 KAZA -->
<div class="day-section">
  <div class="day-header th-d67">
    <div class="day-badge">Day 6 &amp; 7</div>
    <div class="day-title">
      <h2>&#x1F3E8; Stay: Kaza, Spiti Valley &nbsp;<span style="font-weight:400;font-size:15px">(2 Nights)</span></h2>
      <div class="sub">Day 6: Tabo 8 AM &rarr; Kaza 6:30 PM via Dhankar Monastery &nbsp;&middot;&nbsp; Day 7: Full Kaza local circuit &mdash; return same hotel</div>
    </div>
    <div class="pills"><span class="pill">Altitude 3,800 m</span><span class="pill">Circuit Base</span><span class="pill">2 Nights Same Hotel</span></div>
  </div>
  <div class="hotels-grid">
    <div class="hotel-card">
      <span class="opt-tag opt1">Option 1</span>
      <div class="hotel-name">Hotel Kaza &mdash; Main Market</div>
      <div class="hotel-loc">&#x1F4CD; Main Market, opp. Old PWD Rest House, Kaza, Spiti Valley, HP &mdash; 3,800 m</div>
      <div class="rating-row"><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9734;</span><span class="rbadge">4.1 &middot; 34 reviews</span></div>
      <div class="photo-grid">
        <div class="ph ph-main"><img src="https://images.unsplash.com/photo-1578683010236-d716f9a3f461?w=700&h=440&fit=crop&q=80" alt="Hotel Kaza exterior panoramic mountain views"><div class="ph-label">&#x1F3D4; Panoramic Snow-Peak Views</div></div>
        <div class="ph ph-top"><img src="https://images.unsplash.com/photo-1614871329490-28e96491ae62?w=400&h=220&fit=crop&q=80" alt="Comfortable mountain hotel room"><div class="ph-label">&#x1F6CF; Comfortable Room</div></div>
        <div class="ph ph-bot"><img src="https://images.unsplash.com/photo-1584132967334-10e028bd69f7?w=400&h=220&fit=crop&q=80" alt="Clean hotel bathroom hot water"><div class="ph-label">&#x1F6BF; Clean Washroom</div></div>
      </div>
      <div class="hotel-blurb">&ldquo;Panoramic snow-capped Himalayan views from balcony. Electric blankets, kettle, constant hot water. 1 min from market. Very warm and helpful staff. Excellent food.&rdquo;</div>
      <a class="map-btn" href="https://www.google.com/travel/search?ts=CAESCgoCCAMKAggDEAAaHBIaEhQKBwjqDxADGAESBwjqDxADGAIYATICEAAqBwoFOgNJTlI" target="_blank">&#x1F5FA; View on Google Maps</a>
    </div>
    <div class="hotel-card">
      <span class="opt-tag opt2">Option 2</span>
      <div class="hotel-name">Spiti River View Home Stay</div>
      <div class="hotel-loc">&#x1F4CD; Near Ice Hockey Ground, Spiti Riverbank, Kaza, Spiti Valley, HP &mdash; 3,800 m</div>
      <div class="rating-row"><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</span><span class="rbadge">5.0 &middot; 100 reviews</span></div>
      <div class="photo-grid">
        <div class="ph ph-main"><img src="https://images.unsplash.com/photo-1598979072691-4ede12e71e86?w=700&h=440&fit=crop&q=80" alt="Spiti River View Homestay riverside Kaza"><div class="ph-label">&#x1F3DE; Directly on the Spiti River Banks</div></div>
        <div class="ph ph-top"><img src="https://images.unsplash.com/photo-1595576508898-0ad5c879a061?w=400&h=220&fit=crop&q=80" alt="River view room homestay Kaza"><div class="ph-label">&#x1F6CF; River-View Room</div></div>
        <div class="ph ph-bot"><img src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?w=400&h=220&fit=crop&q=80" alt="Spiti River valley surroundings"><div class="ph-label">&#x1F30A; Spiti River &amp; Valley</div></div>
      </div>
      <div class="hotel-blurb">&ldquo;Located RIGHT on the banks of the Spiti River. Waking up to the sound of flowing water with panoramic valley views is absolutely surreal. Host Sam Bhaiji is incredibly warm. Food tastes just like home.&rdquo;</div>
      <a class="map-btn" href="https://share.google/nHoOFTNzOppifMTlK" target="_blank">&#x1F5FA; View on Google Maps</a>
    </div>
  </div>
  <div class="note-box">&#x26A0;&#xFE0F; Same hotel for both nights (Day 6 &amp; Day 7). Day 7 is the Kaza Local Circuit (Key &rarr; Kibber &rarr; Chicham Bridge &rarr; Hikkim &rarr; Komic &rarr; Langza) &mdash; you return to the same room each evening.</div>
</div>

<!-- DAY 8 CHANDRATAL -->
<div class="day-section">
  <div class="day-header th-d8">
    <div class="day-badge">Day 8</div>
    <div class="day-title">
      <h2>&#x26FA;&#xFE0F; Camp: Chandratal &mdash; The Moon Lake</h2>
      <div class="sub">Kaza 8:00 AM &rarr; Losar &rarr; Kunzum Pass &rarr; Chandratal 4:30 PM &nbsp;&middot;&nbsp; Lakeside tent stay at 14,100 ft</div>
    </div>
    <div class="pills"><span class="pill">Altitude 4,300 m</span><span class="pill">Tent Camp</span><span class="pill">Star Gazing</span><span class="pill">14,100 ft</span></div>
  </div>
  <div class="hotels-grid">
    <div class="hotel-card">
      <span class="opt-tag opt1">Option 1</span>
      <div class="hotel-name">Sakya Camp &mdash; Chandratal</div>
      <div class="hotel-loc">&#x1F4CD; Chandratal Road, near Chandratal Lake, Spiti, HP &mdash; 4,300 m / 14,100 ft</div>
      <div class="rating-row"><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9735;</span><span class="rbadge">4.6 &middot; 101 reviews</span></div>
      <div class="photo-grid">
        <div class="ph ph-main"><img src="https://images.unsplash.com/photo-1504280390367-361c6d9f38f4?w=700&h=440&fit=crop&q=80" alt="Sakya Camp Chandratal lakeside tents"><div class="ph-label">&#x26FA; Lakeside Camp at 4,300 m</div></div>
        <div class="ph ph-top"><img src="https://images.unsplash.com/photo-1478827536114-da961b7f86d2?w=400&h=220&fit=crop&q=80" alt="Tent interior warm beds blankets"><div class="ph-label">&#x1F9F3; Warm Tent Interior</div></div>
        <div class="ph ph-bot"><img src="https://images.unsplash.com/photo-1502126324834-38f8e02d7160?w=400&h=220&fit=crop&q=80" alt="Chandratal starlit night sky milky way"><div class="ph-label">&#x2728; Starlit Night Sky</div></div>
      </div>
      <div class="hotel-blurb">&ldquo;Comfortable tents right beside Moon Lake. Warm blankets, attached washrooms. Bonfire evenings under the clearest sky you&rsquo;ve ever seen. Hearty Himalayan meals. Truly once-in-a-lifetime.&rdquo;</div>
      <a class="map-btn" href="https://www.google.com/travel/search?ts=CAESCgoCCAMKAggDEAAaHBIaEhQKBwjqDxADGAESBwjqDxADGAIYATICEAAqBwoFOgNJTlI" target="_blank">&#x1F5FA; View on Google Maps</a>
    </div>
    <div class="hotel-card">
      <span class="opt-tag opt2">Option 2</span>
      <div class="hotel-name">Samsong Camp &mdash; Chandratal</div>
      <div class="hotel-loc">&#x1F4CD; Near Chandratal Lake, Spiti Valley, HP &mdash; 4,300 m / 14,100 ft</div>
      <div class="rating-row"><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9735;</span><span class="rbadge">4.7 &middot; 273 reviews</span></div>
      <div class="photo-grid">
        <div class="ph ph-main"><img src="https://images.unsplash.com/photo-1537225228614-56cc3556d7ed?w=700&h=440&fit=crop&q=80" alt="Samsong Camp tents mountain backdrop Chandratal"><div class="ph-label">&#x26FA; Camp with Himalayan Backdrop</div></div>
        <div class="ph ph-top"><img src="https://images.unsplash.com/photo-1523987355523-c7b5b0dd90a7?w=400&h=220&fit=crop&q=80" alt="Cosy tent beds inside quilts"><div class="ph-label">&#x1F6CF; Cosy Tent Beds &amp; Quilts</div></div>
        <div class="ph ph-bot"><img src="https://images.unsplash.com/photo-1500534314209-a25ddb2bd429?w=400&h=220&fit=crop&q=80" alt="Chandratal Moon Lake morning sunrise"><div class="ph-label">&#x1F305; Moon Lake at Sunrise</div></div>
      </div>
      <div class="hotel-blurb">&ldquo;Easily the best night of the entire trip. Cosy tents with attached bathrooms. Common food tent &mdash; great camaraderie with fellow travellers. Magical stargazing after 8 PM.&rdquo;</div>
      <a class="map-btn" href="https://share.google/nHoOFTNzOppifMTlK" target="_blank">&#x1F5FA; View on Google Maps</a>
    </div>
  </div>
</div>

<!-- DAY 9 BUS -->
<div class="transport-section">
  <div class="day-header th-d9">
    <div class="day-badge">Day 9</div>
    <div class="day-title"><h2>&#x1F68C; Chandratal &rarr; Manali &rarr; Delhi (Overnight Bus)</h2><div class="sub">Chandratal 7:30 AM &rarr; Manali 3:30 PM &middot; Hadimba Devi Temple &middot; Mall Road &middot; Bus dep. 5 PM &rarr; Delhi 5 AM</div></div>
    <div class="pills"><span class="pill">Via Atal Tunnel</span><span class="pill">Overnight Bus</span></div>
  </div>
  <div class="transport-inner">
    <div class="t-icon">&#x1F68C;</div>
    <div class="t-info"><h3>Manali &rarr; Delhi Overnight Volvo Bus</h3><p>Arrive Manali by 3:30 PM. Explore Mall Road and Hadimba Devi Temple before boarding the overnight Volvo bus at 5:00 PM. Arrive Delhi at 5:00 AM Day 10.</p></div>
    <div class="t-time">Dep Manali: 5:00 PM<br>Arr Delhi: 5:00 AM</div>
  </div>
</div>

<!-- DAY 10-11 TRAIN -->
<div class="transport-section">
  <div class="day-header th-train">
    <div class="day-badge">Day 10&ndash;11</div>
    <div class="day-title"><h2>&#x1F682; Train Home &mdash; Delhi &rarr; Pune</h2><div class="sub">Delhi 6:16 AM (Day 10) &rarr; Pune 2:10 AM (Day 11) &nbsp;&middot;&nbsp; Journey complete!</div></div>
    <div class="pills"><span class="pill">Dep 6:16 AM</span><span class="pill">Arr 2:10 AM (+1)</span></div>
  </div>
  <div class="transport-inner">
    <div class="t-icon">&#x1F682;</div>
    <div class="t-info"><h3>Delhi &rarr; Pune Overnight Train</h3><p>Journey home carrying your photos, your memories, and a story worth telling for a lifetime. See you on the next expedition! &#x1F3D4;&#xFE0F;</p></div>
    <div class="t-time">Dep: 6:16 AM<br>Arr: 2:10 AM (+1)</div>
  </div>
</div>

</div>

<div class="page-footer">
  <strong>Spiti Valley Expedition &mdash; Hotel Guide</strong>
  All stays include Breakfast &amp; Dinner &nbsp;&middot;&nbsp; Triple Sharing (2 beds + 1 mattress) &nbsp;&middot;&nbsp; 3-Star / Best Available
  <div class="footnote">Photos are representative of property type and surroundings. Final allocation subject to availability. Early booking guarantees the same property for all travellers.</div>
</div>

</body>
</html>
