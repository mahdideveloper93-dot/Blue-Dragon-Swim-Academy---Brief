# Blue-Dragon-Swim-Academy---Brief
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Blue Dragon Swim Academy — Creative Brief | Ahmed El-Mahdi</title>
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800;900&display=swap" rel="stylesheet">
<style>
* { box-sizing: border-box; margin: 0; padding: 0; }

body {
  font-family: 'Tajawal', sans-serif;
  background: #0a1628;
  color: #e8f1f8;
  line-height: 1.9;
  direction: rtl;
}

.container {
  max-width: 900px;
  margin: 0 auto;
}

/* COVER */
.cover {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: linear-gradient(180deg, #0a1628 0%, #0d1f3c 50%, #0a2a4a 100%);
  position: relative;
  overflow: hidden;
  padding: 40px 30px 50px;
}

.cover::before {
  content: '';
  position: absolute;
  top: -150px; right: -150px;
  width: 400px; height: 400px;
  background: radial-gradient(circle, rgba(0,168,255,0.08) 0%, transparent 70%);
  border-radius: 50%;
}

.cover-glow {
  position: absolute;
  bottom: -150px; left: -150px;
  width: 400px; height: 400px;
  background: radial-gradient(circle, rgba(0,229,201,0.06) 0%, transparent 70%);
  border-radius: 50%;
}

.cover-logo {
  width: 160px; height: 160px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 20px;
  position: relative; z-index: 1;
  border: 3px solid rgba(0,168,255,0.3);
  box-shadow: 0 0 40px rgba(0,168,255,0.2);
  background: #fff;
  padding: 6px;
}

.cover-tag {
  font-size: 12px; font-weight: 700;
  letter-spacing: 5px; color: #00a8ff;
  margin-bottom: 16px;
  position: relative; z-index: 1;
  border: 1px solid rgba(0,168,255,0.3);
  padding: 6px 20px; border-radius: 30px;
}

.cover-title {
  font-size: 36px; font-weight: 900;
  color: #fff; margin-bottom: 6px;
  position: relative; z-index: 1;
  line-height: 1.2;
}

.cover-subtitle {
  font-size: 17px; font-weight: 300;
  color: #7eb8e8; margin-bottom: 28px;
  position: relative; z-index: 1;
  letter-spacing: 2px;
}

.cover-divider {
  width: 70px; height: 3px;
  background: linear-gradient(90deg, #00a8ff, #00d4ff, #00e5c9);
  border-radius: 2px; margin-bottom: 28px;
  position: relative; z-index: 1;
}

.cover-name {
  font-size: 24px; font-weight: 800;
  color: #fff; margin-bottom: 6px;
  position: relative; z-index: 1;
}

.cover-role {
  font-size: 14px; font-weight: 400;
  color: #7eb8e8;
  position: relative; z-index: 1;
  line-height: 1.7;
}

.cover-motto {
  margin-top: 35px;
  font-size: 15px; font-weight: 500;
  color: #a8d4f0; font-style: italic;
  position: relative; z-index: 1;
  max-width: 450px; line-height: 1.8;
  border-right: 3px solid #00a8ff;
  padding-right: 18px;
}

.cover-date {
  margin-top: 40px;
  font-size: 11px; color: #5a8ab0;
  letter-spacing: 2px;
  position: relative; z-index: 1;
}

/* SECTIONS */
.section {
  padding: 40px 35px;
  background: #0d1f3c;
  border-bottom: 1px solid rgba(0,168,255,0.06);
}

.section-alt { background: #0a1628; }

.section-header {
  display: flex; align-items: center;
  gap: 12px; margin-bottom: 24px;
}

.section-number {
  width: 40px; height: 40px;
  background: linear-gradient(135deg, #00a8ff, #00d4ff);
  border-radius: 10px;
  display: flex; align-items: center;
  justify-content: center;
  font-size: 16px; font-weight: 900;
  color: #0a1628; flex-shrink: 0;
}

.section-title {
  font-size: 22px; font-weight: 800;
  color: #fff;
}

.section-subtitle {
  font-size: 12px; color: #7eb8e8;
  font-weight: 400; margin-top: 2px;
}

/* CONTENT */
.highlight-box {
  background: linear-gradient(135deg, rgba(0,168,255,0.08), rgba(0,229,201,0.04));
  border: 1px solid rgba(0,168,255,0.15);
  border-radius: 14px;
  padding: 20px 24px;
  margin: 16px 0;
}

.highlight-box p {
  font-size: 14px; color: #c8ddf0;
  line-height: 1.9;
}

.highlight-box strong { color: #fff; font-weight: 700; }

.quote-box {
  background: rgba(0,168,255,0.06);
  border-right: 4px solid #00a8ff;
  padding: 16px 20px;
  border-radius: 0 10px 10px 0;
  margin: 20px 0;
  font-size: 14px; font-weight: 500;
  color: #a8d4f0; font-style: italic;
  line-height: 1.9;
}

.sub-heading {
  font-size: 16px; color: #00a8ff;
  margin: 22px 0 12px 0;
  font-weight: 800;
}

/* LISTS */
.feature-list {
  list-style: none; padding: 0;
}

.feature-list li {
  padding: 10px 0; padding-right: 30px;
  position: relative;
  font-size: 13px; color: #c8ddf0;
  border-bottom: 1px solid rgba(255,255,255,0.04);
}

.feature-list li:last-child { border-bottom: none; }

.feature-list li::before {
  content: '▸'; position: absolute;
  right: 0; color: #00a8ff;
  font-size: 16px; font-weight: bold;
}

/* CARDS */
.cards-grid-2 {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 14px; margin: 14px 0;
}

.cards-grid-3 {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 12px; margin: 14px 0;
}

.card {
  background: rgba(255,255,255,0.03);
  border: 1px solid rgba(0,168,255,0.1);
  border-radius: 12px;
  padding: 16px;
  transition: all 0.3s ease;
}

.card:hover {
  background: rgba(0,168,255,0.05);
  border-color: rgba(0,168,255,0.2);
}

.card.center { text-align: center; }

.card-full { grid-column: span 2; }

.card-icon {
  font-size: 24px; margin-bottom: 8px;
}

.card-title {
  font-size: 14px; font-weight: 800;
  color: #fff; margin-bottom: 6px;
}

.card-text {
  font-size: 12px; color: #7eb8e8;
  line-height: 1.6;
}

/* TAGS */
.tag-row {
  display: flex; flex-wrap: wrap;
  gap: 6px; margin: 12px 0;
}

.tag {
  font-size: 11px; font-weight: 500;
  color: #a8d4f0;
  background: rgba(0,168,255,0.08);
  border: 1px solid rgba(0,168,255,0.15);
  padding: 5px 12px; border-radius: 18px;
}

.tag-primary {
  background: linear-gradient(135deg, rgba(0,168,255,0.15), rgba(0,229,201,0.1));
  border-color: rgba(0,168,255,0.25);
  color: #fff; font-weight: 700;
}

/* TIMELINE */
.timeline {
  position: relative;
  margin: 24px 0; padding-right: 24px;
}

.timeline::before {
  content: '';
  position: absolute;
  right: 6px; top: 0; bottom: 0;
  width: 2px;
  background: linear-gradient(180deg, #00a8ff, #00d4ff, #00e5c9);
  border-radius: 1px;
}

.timeline-item {
  position: relative;
  margin-bottom: 20px; padding-right: 22px;
}

.timeline-dot {
  position: absolute;
  right: -23px; top: 5px;
  width: 12px; height: 12px;
  background: #00a8ff; border-radius: 50%;
  border: 3px solid #0d1f3c;
  box-shadow: 0 0 8px rgba(0,168,255,0.4);
}

.timeline-dot-final {
  background: #00e5c9;
  box-shadow: 0 0 10px rgba(0,229,201,0.5);
}

.timeline-year {
  font-size: 12px; font-weight: 700;
  color: #00a8ff; margin-bottom: 3px;
}

.timeline-title {
  font-size: 14px; font-weight: 700;
  color: #fff; margin-bottom: 3px;
}

.timeline-desc {
  font-size: 12px; color: #7eb8e8;
  line-height: 1.6;
}

/* LOGO SHOWCASE */
.logo-showcase {
  text-align: center;
  padding: 30px;
  background: linear-gradient(135deg, rgba(0,168,255,0.05), rgba(0,229,201,0.02));
  border: 1px solid rgba(0,168,255,0.1);
  border-radius: 16px;
  margin: 16px 0;
}

.logo-showcase img {
  width: 160px; height: 160px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid rgba(0,168,255,0.2);
  box-shadow: 0 0 40px rgba(0,168,255,0.12);
  background: #fff;
  padding: 8px;
}

.logo-colors {
  display: flex;
  justify-content: center;
  gap: 16px;
  margin-top: 20px;
  flex-wrap: wrap;
}

.color-swatch { text-align: center; }

.color-circle {
  width: 42px; height: 42px;
  border-radius: 50%;
  margin: 0 auto 6px;
  border: 2px solid rgba(255,255,255,0.1);
}

.color-name {
  font-size: 10px; color: #7eb8e8;
  font-weight: 500;
}

.color-code {
  font-size: 9px; color: #5a8ab0;
  font-family: monospace;
}

/* TABLE */
.info-table {
  width: 100%;
  border-collapse: collapse;
  margin: 16px 0;
  font-size: 13px;
}

.info-table th {
  background: rgba(0,168,255,0.1);
  color: #00a8ff; font-weight: 700;
  padding: 12px 14px;
  text-align: right;
  border-bottom: 2px solid rgba(0,168,255,0.2);
}

.info-table td {
  padding: 12px 14px;
  border-bottom: 1px solid rgba(255,255,255,0.05);
  color: #c8ddf0;
}

.info-table tr:hover td {
  background: rgba(0,168,255,0.03);
}

/* FOOTER */
.page-footer {
  text-align: center;
  padding: 24px 30px;
  background: #0a1628;
  border-top: 1px solid rgba(0,168,255,0.1);
}

.page-footer p {
  font-size: 11px; color: #5a8ab0;
  letter-spacing: 1px;
}

/* RESPONSIVE */
@media (max-width: 600px) {
  .cards-grid-2, .cards-grid-3 { grid-template-columns: 1fr; }
  .card-full { grid-column: span 1; }
  .cover-title { font-size: 28px; }
  .section { padding: 28px 20px; }
  .cover-logo { width: 120px; height: 120px; }
}
</style>
</head>
<body>

<div class="container">

<!-- COVER -->
<div class="cover">
  <div class="cover-glow"></div>
  <img src="1000392921.jpg" alt="Blue Dragon Logo" class="cover-logo">
  <div class="cover-tag">CREATIVE BRIEF</div>
  <h1 class="cover-title">بريف الإنتاج الإبداعي</h1>
  <p class="cover-subtitle">Content Creator & Production Team Brief</p>
  <div class="cover-divider"></div>
  <div class="cover-name">أحمد المهدي</div>
  <p class="cover-role">مؤسس ومدير أكاديمية Blue Dragon Swim Academy</p>
  <div class="cover-motto">
    "نحن لا نعلم السباحة فقط...<br>
    نحن نبني سباحين، ونصنع مدربين، ونترك أثرًا."
  </div>
  <div class="cover-date">يوليو 2026 | Confidential</div>
</div>

<!-- SECTION 1 -->
<div class="section">
  <div class="section-header">
    <div class="section-number">01</div>
    <div>
      <div class="section-title">من هو أحمد المهدي؟</div>
      <div class="section-subtitle">The Man Behind The Brand</div>
    </div>
  </div>
  <div class="highlight-box">
    <p>أنا <strong>أحمد المهدي</strong>، مؤسس ومدير <strong>Blue Dragon Swim Academy</strong>. أعمل في مجال السباحة والتدريب الرياضي منذ عمر مبكر، وهو المجال الذي بدأت فيه رحلتي منذ الصغر، وأصبح جزءًا أساسيًا من شخصيتي وحياتي.</p>
    <p style="margin-top:12px;">أؤمن أن <strong>النجاح الحقيقي</strong> لا يكون فقط في تحقيق نتائج شخصية، ولكن في بناء شيء يستمر بعدك، وفي ترك <strong>أثر واضح</strong> في حياة الأشخاص الذين تعمل معهم.</p>
  </div>
  <div class="quote-box">"كن نافعًا للآخرين."</div>
  <h3 class="sub-heading">🎯 الشخصية اللي عاوزها تظهر في المحتوى:</h3>
  <div class="cards-grid-2">
    <div class="card"><div class="card-icon">👨‍🏫</div><div class="card-title">مدرب صاحب خبرة</div><div class="card-text">بدأت السباحة من عمر 7 سنين. انتقلت من لاعب لمدرب. خبرة في كل الفئات والمستويات.</div></div>
    <div class="card"><div class="card-icon">🏊</div><div class="card-title">متخصص في السباحة</div><div class="card-text">تعليم، تطوير، منافسات، علاج مائي، ذوي احتياجات خاصة — خبرة شاملة في كل جوانب السباحة.</div></div>
    <div class="card"><div class="card-icon">🚀</div><div class="card-title">رجل أعمال لديه رؤية</div><div class="card-text">مؤسس Blue Dragon Swim Academy برؤية واضحة لبناء أكبر اسم عربي في مجال السباحة.</div></div>
    <div class="card"><div class="card-icon">📚</div><div class="card-title">ينقل العلم والخبرة</div><div class="card-text">صنعت 30 مدرب سباحة في 4 سنين. المدربين أهم من أي رقم آخر.</div></div>
    <div class="card card-full"><div class="card-icon">❤️</div><div class="card-title">يهتم بالناس قبل الأرباح</div><div class="card-text">كل شخص أساعده — طفل يتعلم لأول مرة، سباح يحقق هدفه، مدرب يبدأ حياته، شخص يستعيد قدرته — كلهم جزء من النجاح الحقيقي.</div></div>
  </div>
</div>

<!-- SECTION 2 -->
<div class="section section-alt">
  <div class="section-header">
    <div class="section-number">02</div>
    <div>
      <div class="section-title">رحلتي المهنية</div>
      <div class="section-subtitle">Professional Career Journey</div>
    </div>
  </div>
  <div class="highlight-box">
    <p>رحلتي في السباحة بدأت منذ <strong>عمر 7 سنين</strong>. كانت السباحة أكثر من مجرد رياضة — كانت <strong>مدرسة</strong> تعلمت منها الالتزام والانضباط والصبر وتحمل المسؤولية.</p>
    <p style="margin-top:12px;">انتقلت من مرحلة <strong>اللاعب</strong> لمرحلة <strong>المدرب</strong>، واكتشفت إن شغفي الحقيقي مش في السباحة نفسها، ولكن في <strong>تعليم الآخرين</strong> وتطوير مستواهم ورؤية التغيير اللي بيحصل لهم.</p>
  </div>
  <h3 class="sub-heading">📍 مسيرتي المهنية:</h3>
  <div class="timeline">
    <div class="timeline-item"><div class="timeline-dot"></div><div class="timeline-year">🥇 البداية</div><div class="timeline-title">سباح وبطل جمهورية</div><div class="timeline-desc">بدأت رحلتي كلاعب سباحة، وحققت بطولة الجمهورية — ده اللي بنى الأساس الفني والذهني اللي بشتغل عليه لحد النهاردة.</div></div>
    <div class="timeline-item"><div class="timeline-dot"></div><div class="timeline-year">2016</div><div class="timeline-title">مدرب عام — نادي غزل المحلة</div><div class="timeline-desc">أول خطوة احترافية في التدريب. اكتسبت خبرة في التعامل مع مجموعات كبيرة وبيئات رياضية متنوعة.</div></div>
    <div class="timeline-item"><div class="timeline-dot"></div><div class="timeline-year">فترة العمل الدولي</div><div class="timeline-title">مدرب في أكاديمية بوسايدون — دولة الكويت</div><div class="timeline-desc">خبرة دولية في بيئة تدريبية مختلفة. تعلمت أساليب تدريب عالمية واكتسبت فهم أعمق لصناعة السباحة على المستوى الإقليمي.</div></div>
    <div class="timeline-item"><div class="timeline-dot"></div><div class="timeline-year">الأندية المصرية الكبرى</div><div class="timeline-title">النادي الأهلي والزمالك — مصر</div><div class="timeline-desc">اشتغلت في أكبر وأعرق الأندية الرياضية في مصر. ده أعطاني خبرة في التعامل مع بيئات احترافية عالية المستوى ومعايير تدريب محلية وعربية رفيعة.</div></div>
    <div class="timeline-item"><div class="timeline-dot"></div><div class="timeline-year">العمل في الإمارات</div><div class="timeline-title">كلية الشرطة — أبوظبي</div><div class="timeline-desc">خبرة تدريبية في بيئة عسكرية-رياضية متقدمة في أبوظبي. اكتسبت خبرة في التدريب تحت ضغط ومعايير صارمة.</div></div>
    <div class="timeline-item"><div class="timeline-dot"></div><div class="timeline-year">الفاعليات والبطولات</div><div class="timeline-title">تنظيم فاعليات وبطولات سباحة في أبوظبي ومصر</div><div class="timeline-desc">أكتر من فاعلية وبطولة سباحة تم تنظيمها بنجاح — ده أثبت إن خبرتي مش بس في التدريب، ولكن في إدارة الفعاليات الرياضية بشكل احترافي على مستوى دولي.</div></div>
    <div class="timeline-item"><div class="timeline-dot timeline-dot-final"></div><div class="timeline-year">التأسيس</div><div class="timeline-title">مؤسس ومدير — Blue Dragon Swim Academy</div><div class="timeline-desc">الخطوة الأكبر. تأسيس أكاديمية بروح مختلفة — مش مجرد تعليم سباحة، ده بناء جيل من السباحين والمدربين.</div></div>
  </div>
  <div class="quote-box">"المدرب الناجح ليس فقط شخص يعرف الحركات الفنية داخل الماء، ولكنه شخص يعرف كيف يتعامل مع الإنسان قبل السباح."</div>
</div>

<!-- SECTION 3 -->
<div class="section">
  <div class="section-header">
    <div class="section-number">03</div>
    <div>
      <div class="section-title">خبرتي ومجالات تخصصي</div>
      <div class="section-subtitle">Areas of Expertise</div>
    </div>
  </div>
  <div class="cards-grid-2">
    <div class="card"><div class="card-icon">🏊</div><div class="card-title">تعليم أساسيات السباحة</div><div class="card-text">لجميع الفئات العمرية — من عمر 3 سنين للكبار</div></div>
    <div class="card"><div class="card-icon">📈</div><div class="card-title">تطوير مهارات السباحين</div><div class="card-text">من المستوى المبتدئ للمتقدم والاحترافي</div></div>
    <div class="card"><div class="card-icon">🏆</div><div class="card-title">إعداد اللاعبين للمنافسات</div><div class="card-text">خطة تدريبية مكثفة للبطولات والمنافسات</div></div>
    <div class="card"><div class="card-icon">📋</div><div class="card-title">وضع الخطط التدريبية</div><div class="card-text">خطط مخصصة حسب كل سباح وهدفه</div></div>
    <div class="card"><div class="card-icon">👶</div><div class="card-title">التعامل مع الأطفال بطريقة تربوية</div><div class="card-text">فهم نفسية الطفل وكسب ثقته داخل الماء</div></div>
    <div class="card"><div class="card-icon">♿</div><div class="card-title">تدريب ذوي الاحتياجات الخاصة</div><div class="card-text">خبرة متخصصة في التعامل مع مختلف الاحتياجات</div></div>
    <div class="card"><div class="card-icon">💧</div><div class="card-title">العلاج المائي</div><div class="card-text">تأهيل وعلاج من خلال السباحة والتمارين المائية</div></div>
    <div class="card"><div class="card-icon">🎓</div><div class="card-title">تدريب وتأهيل مدربي السباحة</div><div class="card-text">30 مدرب تم تأهيلهم خلال 4 سنين</div></div>
  </div>
  <h3 class="sub-heading">👥 الفئات اللي اشتغلت معاها:</h3>
  <ul class="feature-list">
    <li>الأطفال المبتدئين</li>
    <li>الكبار اللي عاوزين يتعلموا السباحة</li>
    <li>السباحين الراغبين في المنافسة</li>
    <li>ذوي الاحتياجات الخاصة</li>
    <li>حالات العلاج المائي والتأهيل</li>
  </ul>
</div>

<!-- SECTION 4 -->
<div class="section section-alt">
  <div class="section-header">
    <div class="section-number">04</div>
    <div>
      <div class="section-title">Blue Dragon Swim Academy</div>
      <div class="section-subtitle">The Academy — Vision, Mission & Identity</div>
    </div>
  </div>
  <div class="logo-showcase">
    <img src="1000392921.jpg" alt="Blue Dragon Logo">
    <div class="logo-colors">
      <div class="color-swatch"><div class="color-circle" style="background:#003B6D;"></div><div class="color-name">أزرق غامق</div><div class="color-code">#003B6D</div></div>
      <div class="color-swatch"><div class="color-circle" style="background:#0077B6;"></div><div class="color-name">أزرق متوسط</div><div class="color-code">#0077B6</div></div>
      <div class="color-swatch"><div class="color-circle" style="background:#00B4D8;"></div><div class="color-name">سماوي فاتح</div><div class="color-code">#00B4D8</div></div>
      <div class="color-swatch"><div class="color-circle" style="background:#E8F1F8;border:1px solid rgba(255,255,255,0.2);"></div><div class="color-name">أبيض/فضي</div><div class="color-code">#E8F1F8</div></div>
    </div>
  </div>
  <div class="highlight-box">
    <p><strong>الأكاديمية ليست مجرد مكان لتعليم الأطفال السباحة</strong> — دي مشروع له رؤية ورسالة. نهتم إن تجربة الطفل تكون مختلفة، بداية من أول حصة لحد الوصول لمستوى متقدم.</p>
  </div>
  <h3 class="sub-heading">🎯 رؤيتنا:</h3>
  <div class="cards-grid-3">
    <div class="card center"><div class="card-icon">🎯</div><div class="card-title">المهارة</div></div>
    <div class="card center"><div class="card-icon">💪</div><div class="card-title">الثقة بالنفس</div></div>
    <div class="card center"><div class="card-icon">📏</div><div class="card-title">الانضباط</div></div>
    <div class="card center"><div class="card-icon">❤️</div><div class="card-title">حب الرياضة</div></div>
    <div class="card center"><div class="card-icon">📈</div><div class="card-title">القدرة على التطور</div></div>
  </div>
  <h3 class="sub-heading">⭐ أهم مميزات الأكاديمية:</h3>
  <div style="margin-bottom:16px;">
    <h4 style="font-size:15px;color:#fff;margin-bottom:8px;font-weight:700;">1️⃣ الخبرة والتخصص</h4>
    <p style="font-size:13px;color:#7eb8e8;line-height:1.7;">خبرة حقيقية في مجال السباحة والتدريب، مش مجرد تعليم حركات أساسية. فهم كامل لمراحل تطور السباح من البداية لحد الاحتراف — بناءً على سنوات من العمل في الأهلي والزمالك في مصر، وكلية الشرطة في أبوظبي، وأكاديمية بوسايدون في الكويت.</p>
  </div>
  <div style="margin-bottom:16px;">
    <h4 style="font-size:15px;color:#fff;margin-bottom:8px;font-weight:700;">2️⃣ برامج تدريبية لجميع الفئات</h4>
    <div class="tag-row">
      <span class="tag">🏊 أطفال من 3 سنين</span>
      <span class="tag">🏊‍♂️ كبار ومبتدئين</span>
      <span class="tag">🏆 سباحين منافسين</span>
      <span class="tag">♿ ذوي الاحتياجات الخاصة</span>
      <span class="tag">💧 علاج مائي</span>
      <span class="tag">👤 تدريب خاص</span>
    </div>
  </div>
  <div style="margin-bottom:16px;">
    <h4 style="font-size:15px;color:#fff;margin-bottom:8px;font-weight:700;">3️⃣ الاهتمام بذوي الاحتياجات الخاصة</h4>
    <p style="font-size:13px;color:#7eb8e8;line-height:1.7;">ما بنتعاملش معاهم كحالات مختلفة — بنتعامل معاهم كأشخاص عندهم قدرات يمكن تطويرها. هدفنا: زيادة الثقة بالنفس، تحسين الحركة، تطوير المهارات، الاستمتاع بالرياضة.</p>
  </div>
  <div style="margin-bottom:16px;">
    <h4 style="font-size:15px;color:#fff;margin-bottom:8px;font-weight:700;">4️⃣ صناعة المدربين</h4>
    <div class="highlight-box" style="background: linear-gradient(135deg, rgba(0,168,255,0.12), rgba(0,229,201,0.06));">
      <p style="font-size:15px;font-weight:700;color:#fff;">🎓 30 مدرب سباحة تم تطويرهم وتعليمهم خلال 4 سنين</p>
      <p style="margin-top:8px;font-size:13px;">"كما تعلمت من مدربين سابقين، أريد أن أنقل خبرتي لجيل جديد من المدربين المحترفين."</p>
    </div>
  </div>
  <h3 class="sub-heading">📍 معلومات الأكاديمية:</h3>
  <table class="info-table">
    <tr><th>الاسم</th><td>Blue Dragon Swim Academy</td></tr>
    <tr><th>المدينة</th><td>المحلة الكبرى، مصر</td></tr>
    <tr><th>الفروع</th><td>نادي العدوي | نادي الشرطة</td></tr>
    <tr><th>المؤسس والمدير</th><td>أحمد المهدي</td></tr>
    <tr><th>الفئة العمرية (أطفال)</th><td>3 – 16 سنة</td></tr>
    <tr><th>الفئة العمرية (أولياء الأمور)</th><td>25 – 45 سنة</td></tr>
    <tr><th>الفئة الاقتصادية</th><td>A / B / C+</td></tr>
    <tr><th>الشعار</th><td>"نحن لا نعلم السباحة فقط... نحن نبني سباحين، ونصنع مدربين، ونترك أثرًا."</td></tr>
  </table>
</div>

<!-- SECTION 5 -->
<div class="section">
  <div class="section-header">
    <div class="section-number">05</div>
    <div>
      <div class="section-title">الجمهور المستهدف</div>
      <div class="section-subtitle">Target Audience Profile</div>
    </div>
  </div>
  <div class="highlight-box">
    <p><strong>العميل المثالي:</strong> أولياء أمور يبحثون عن أكاديمية سباحة <strong>احترافية وآمنة</strong> لأبنائهم، تقدم تعليم سباحة بجودة عالية، ومدربين متخصصين، مع متابعة حقيقية لتطور الطفل.</p>
  </div>
  <h3 class="sub-heading">❤️ اهتمامات الجمهور:</h3>
  <div class="tag-row">
    <span class="tag tag-primary">تعليم السباحة للأطفال</span>
    <span class="tag tag-primary">تنمية مهارات الأطفال</span>
    <span class="tag tag-primary">الأنشطة الرياضية</span>
    <span class="tag tag-primary">اللياقة البدنية</span>
    <span class="tag tag-primary">الأمان داخل الماء</span>
    <span class="tag tag-primary">البطولات الرياضية</span>
    <span class="tag tag-primary">ذوي الاحتياجات الخاصة</span>
    <span class="tag tag-primary">العلاج المائي</span>
    <span class="tag tag-primary">تطوير المهارات</span>
  </div>
  <h3 class="sub-heading">🔑 الكلمات المفتاحية:</h3>
  <div class="tag-row">
    <span class="tag">Swimming Academy</span>
    <span class="tag">Kids Swimming</span>
    <span class="tag">Swimming Lessons</span>
    <span class="tag">Swimming Coach</span>
    <span class="tag">Special Needs Swimming</span>
    <span class="tag">Hydrotherapy</span>
    <span class="tag">Sports Academy</span>
    <span class="tag">Kids Activities</span>
    <span class="tag">Water Safety</span>
    <span class="tag">Competitive Swimming</span>
  </div>
</div>

<!-- SECTION 6 -->
<div class="section section-alt">
  <div class="section-header">
    <div class="section-number">06</div>
    <div>
      <div class="section-title">استراتيجية المحتوى</div>
      <div class="section-subtitle">Content Pillars & Direction</div>
    </div>
  </div>
  <div class="quote-box" style="border-color:#00e5c9;">
    <strong>ملاحظة مهمة:</strong> أنا لا أريد أن أظهر كـ Influencer أو صانع محتوى. الهدف من المحتوى هو <strong>بناء الثقة وإظهار الخبرة</strong>.
  </div>
  <h3 class="sub-heading">📊 المحاور الثلاثة للمحتوى:</h3>
  <div class="card" style="margin-bottom:12px;border-right:4px solid #00a8ff;">
    <div class="card-title" style="font-size:17px;">🥇 المحور الأول: إبراز الأكاديمية</div>
    <div class="card-text" style="margin-top:8px;">
      <ul class="feature-list">
        <li>قصص نجاح الأطفال</li>
        <li>تطور مستوى السباحين</li>
        <li>يوم داخل الأكاديمية</li>
        <li>طرق التدريب</li>
        <li>الفرق بين التدريب العادي والتدريب الاحترافي</li>
        <li>حياة المدرب داخل حمام السباحة</li>
      </ul>
    </div>
  </div>
  <div class="card" style="margin-bottom:12px;border-right:4px solid #00d4ff;">
    <div class="card-title" style="font-size:17px;">🥈 المحور الثاني: إبراز الخبرة</div>
    <div class="card-text" style="margin-top:8px;">
      <ul class="feature-list">
        <li>أخطاء أولياء الأمور في تعليم السباحة</li>
        <li>نصائح للمدربين الجدد</li>
        <li>مواقف من سنوات التدريب في الأهلي والزمالك (مصر) وأبوظبي والكويت</li>
        <li>الفرق بين المدرب العادي والمدرب المحترف</li>
        <li>كيف تصبح مدرب سباحة ناجح</li>
        <li>لحظات من تنظيم البطولات والفاعليات في أبوظبي ومصر</li>
      </ul>
    </div>
  </div>
  <div class="card" style="margin-bottom:12px;border-right:4px solid #00e5c9;">
    <div class="card-title" style="font-size:17px;">🥉 المحور الثالث: محتوى كوميدي رياضي</div>
    <div class="card-text" style="margin-top:8px;">
      <p style="margin-bottom:10px;color:#7eb8e8;font-size:13px;"><strong>ملاحظة:</strong> الكوميديا تكون مرتبطة بالسباحة وليس مجرد ترند.</p>
      <ul class="feature-list">
        <li>أنواع أولياء الأمور في تمرين السباحة</li>
        <li>لما الطفل يقول "أنا بعرف أعوم"</li>
        <li>الفرق بين أول يوم سباحة وبعد شهر</li>
        <li>أنواع المدربين في حمام السباحة</li>
        <li>توقعات الأهل قبل التمرين والحقيقة</li>
      </ul>
    </div>
  </div>
</div>

<!-- SECTION 7 -->
<div class="section">
  <div class="section-header">
    <div class="section-number">07</div>
    <div>
      <div class="section-title">التوجيه البصري والتصوير</div>
      <div class="section-subtitle">Visual Direction & Production Guidelines</div>
    </div>
  </div>
  <div class="quote-box">الهدف: يشعر المشاهد أنه <strong>يرى عالم Blue Dragon من الداخل</strong>.</div>
  <h3 class="sub-heading">🎬 شكل التصوير المطلوب:</h3>
  <div class="cards-grid-2">
    <div class="card"><div class="card-icon">🎥</div><div class="card-title">لقطات سينمائية</div><div class="card-text">داخل حمام السباحة — إضاءة احترافية، زوايا مبتكرة</div></div>
    <div class="card"><div class="card-icon">🏊</div><div class="card-title">تصوير التدريب الحقيقي</div><div class="card-text">لحظات حقيقية مش تمثيل — الطاقة والتفاعل بين المدرب والطفل</div></div>
    <div class="card"><div class="card-icon">👶</div><div class="card-title">تصوير الأطفال أثناء التطور</div><div class="card-text">Before & After — لحظات النجاح والفرحة</div></div>
    <div class="card"><div class="card-icon">⏱️</div><div class="card-title">Slow Motion</div><div class="card-text">للحركات داخل الماء، المياه، الانغماس — جمال بصري</div></div>
    <div class="card"><div class="card-icon">🎤</div><div class="card-title">مقابلات قصيرة</div><div class="card-text">مع أولياء الأمور — شهادات حقيقية وعفوية</div></div>
    <div class="card"><div class="card-icon">⭐</div><div class="card-title">قصص نجاح حقيقية</div><div class="card-text">Documentary style — رحلة الطفل من الخوف للثقة</div></div>
  </div>
  <h3 class="sub-heading">🎨 الهوية البصرية:</h3>
  <div class="cards-grid-3">
    <div class="card center"><div style="width:45px;height:45px;background:linear-gradient(135deg,#003B6D,#002a4d);border-radius:10px;margin:0 auto 8px;"></div><div class="card-title">أزرق غامق</div><div class="card-text">#003B6D — الثقة، العمق، الاستقرار</div></div>
    <div class="card center"><div style="width:45px;height:45px;background:linear-gradient(135deg,#0077B6,#005a8a);border-radius:10px;margin:0 auto 8px;"></div><div class="card-title">أزرق متوسط</div><div class="card-text">#0077B6 — الماء، الاحترافية</div></div>
    <div class="card center"><div style="width:45px;height:45px;background:linear-gradient(135deg,#00B4D8,#0096b4);border-radius:10px;margin:0 auto 8px;"></div><div class="card-title">سماوي فاتح</div><div class="card-text">#00B4D8 — النقاء، الطاقة، التطور</div></div>
  </div>
  <h3 class="sub-heading">📐 التصميم العام:</h3>
  <ul class="feature-list">
    <li>Premium Design — يشبه عروض وكالات التسويق العالمية</li>
    <li>أيقونات بسيطة وحديثة</li>
    <li>نص مختصر وواضح — لا ازدحام</li>
    <li>مناسب للعرض على العميل ولفريق التسويق الداخلي</li>
    <li>خلفيات داكنة مع لمسات إضاءة زرقاء</li>
    <li>استخدام شعار Blue Dragon Swim Academy في كل المحتوى</li>
  </ul>
</div>

<!-- SECTION 8 -->
<div class="section section-alt">
  <div class="section-header">
    <div class="section-number">08</div>
    <div>
      <div class="section-title">الهدف النهائي</div>
      <div class="section-subtitle">The Ultimate Vision</div>
    </div>
  </div>
  <div class="highlight-box" style="background:linear-gradient(135deg,rgba(0,168,255,0.12),rgba(0,229,201,0.08));border-color:rgba(0,168,255,0.3);">
    <p style="font-size:17px;font-weight:800;color:#fff;text-align:center;line-height:2;">بناء <strong>أكبر اسم عربي</strong> في مجال السباحة والتدريب</p>
  </div>
  <h3 class="sub-heading">🎯 أحمد المهدي = مرتبط بـ:</h3>
  <div class="cards-grid-2">
    <div class="card"><div class="card-icon">🎓</div><div class="card-title">الخبرة</div><div class="card-text">سنوات من التدريب في مصر (الأهلي، الزمالك، غزل المحلة) والكويت (بوسايدون) وأبوظبي (كلية الشرطة)</div></div>
    <div class="card"><div class="card-icon">📚</div><div class="card-title">التعليم</div><div class="card-text">نقل المعرفة للأجيال القادمة من السباحين والمدربين</div></div>
    <div class="card"><div class="card-icon">🏭</div><div class="card-title">صناعة المدربين</div><div class="card-text">30 مدرب وعددنا في زيادة — نبني جيل كامل من المدربين المحترفين</div></div>
    <div class="card"><div class="card-icon">📈</div><div class="card-title">تطوير السباحين</div><div class="card-text">من أول غطسة للبطولات — كل مرحلة لها خطة واهتمام</div></div>
    <div class="card card-full"><div class="card-icon">🏛️</div><div class="card-title">بناء أكاديميات ناجحة</div><div class="card-text">Blue Dragon Swim Academy نموذج يحتذى به في الوطن العربي — مصنع للسباحين، مدرسة للمدربين، مركز للخبرة والتطوير</div></div>
  </div>
  <div class="quote-box" style="border-color:#00e5c9;background:linear-gradient(135deg,rgba(0,168,255,0.08),rgba(0,229,201,0.06));">
    <p style="font-size:18px;font-weight:800;color:#fff;text-align:center;font-style:normal;">"نحن لا نعلم السباحة فقط...<br>نحن نبني سباحين، ونصنع مدربين، ونترك أثرًا."</p>
  </div>
</div>

<!-- SECTION 9 -->
<div class="section">
  <div class="section-header">
    <div class="section-number">09</div>
    <div>
      <div class="section-title">ما يُفعل وما لا يُفعل</div>
      <div class="section-subtitle">Do's & Don'ts</div>
    </div>
  </div>
  <div class="cards-grid-2">
    <div class="card" style="border-right:4px solid #00e5c9;">
      <div class="card-title" style="color:#00e5c9;font-size:17px;">✅ DO's — اعملها</div>
      <div class="card-text" style="margin-top:12px;">
        <ul class="feature-list">
          <li>أظهر <strong>اللحظات الحقيقية</strong> — مش تمثيل</li>
          <li>ركز على <strong>التفاعل الإنساني</strong> بين المدرب والطفل</li>
          <li>استخدم <strong>Slow Motion</strong> للحركات والمياه</li>
          <li>صور <strong>قصص النجاح</strong> بشكل Documentary</li>
          <li>خلّي الكوميديا <strong>مرتبطة بالسباحة</strong> مش ترندات فارغة</li>
          <li>استخدم <strong>ألوان الهوية</strong> بشكل متناسق</li>
          <li>خلّي النص <strong>مختصر وواضح</strong></li>
          <li>ركز على <strong>ذوي الاحتياجات الخاصة</strong> بشكل إنساني</li>
          <li>أظهر <strong>صناعة المدربين</strong> كإنجاز حقيقي</li>
          <li>أبرز <strong>خبرتي في الأندية الكبرى</strong></li>
          <li>استخدم <strong>شعار Blue Dragon</strong> في كل المحتوى</li>
          <li>خلّي كل محتوى يبني <strong>الثقة</strong></li>
        </ul>
      </div>
    </div>
    <div class="card" style="border-right:4px solid #ff4757;">
      <div class="card-title" style="color:#ff4757;font-size:17px;">❌ DON'Ts — متعملهاش</div>
      <div class="card-text" style="margin-top:12px;">
        <ul class="feature-list">
          <li>متعملش محتوى <strong>Influencer style</strong></li>
          <li>متستخدمش <strong>ترندات ملهاش علاقة</strong> بالسباحة</li>
          <li>متصورش <strong>لقطات مفتعلة</strong> أو تمثيل سيئ</li>
          <li>متعملش تصميم <strong>مزدحم أو عادي</strong></li>
          <li>متقللش من <strong>ذوي الاحتياجات الخاصة</strong></li>
          <li>متبعدش عن <strong>الهوية البصرية</strong> المحددة</li>
          <li>متعملش محتوى <strong>تعليمي جاف</strong></li>
          <li>متنساش <strong>الرسالة الإنسانية</strong></li>
          <li>متظهرش <strong>الأرباح</strong> كهدف رئيسي</li>
          <li>متعملش محتوى <strong>مكرر</strong></li>
          <li>متذكرش <strong>شركات أو أندية تانية</strong> — Blue Dragon بس</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<!-- SECTION 10 -->
<div class="section section-alt">
  <div class="section-header">
    <div class="section-number">10</div>
    <div>
      <div class="section-title">ملخص تنفيذي للفريق</div>
      <div class="section-subtitle">Executive Summary</div>
    </div>
  </div>
  <div class="highlight-box" style="background:linear-gradient(135deg,rgba(0,168,255,0.1),rgba(0,229,201,0.05));">
    <p style="font-size:15px;font-weight:700;color:#fff;margin-bottom:12px;">🎯 هذا البريف موجه لفريق الإنتاج والتسويق لتنفيذ خطة محتوى متكاملة لـ Blue Dragon Swim Academy.</p>
    <p>نحن لا نبني مجرد أكاديمية سباحة — نحن نبني <strong>علامة تجارية</strong> تمثل قيمة حقيقية في مجال السباحة العربي. التركيز 100% على الأكاديمية ورسالتها ورؤيتها.</p>
  </div>
  <h3 class="sub-heading">📋 المهام المطلوبة من الفريق:</h3>
  <table class="info-table">
    <tr><th>المهمة</th><th>التفاصيل</th><th>الأولوية</th></tr>
    <tr><td>Social Media Strategy</td><td>خطة محتوى شهرية على Instagram, TikTok, Facebook</td><td style="color:#ff6b6b;font-weight:700;">🔴 عالية</td></tr>
    <tr><td>Content Production</td><td>تصوير وتصميم المحتوى حسب التوجيهات في هذا البريف</td><td style="color:#ff6b6b;font-weight:700;">🔴 عالية</td></tr>
    <tr><td>Brand Identity</td><td>تطوير الهوية البصرية الكاملة باستخدام شعار Blue Dragon</td><td style="color:#ff6b6b;font-weight:700;">🔴 عالية</td></tr>
    <tr><td>Website Development</td><td>موقع إلكتروني يعكس الرؤية والقيم</td><td style="color:#feca57;font-weight:700;">🟡 متوسطة</td></tr>
    <tr><td>SEO & Keywords</td><td>تحسين محركات البحث بالكلمات المفتاحية المحددة</td><td style="color:#feca57;font-weight:700;">🟡 متوسطة</td></tr>
    <tr><td>Paid Advertising</td><td>حملات إعلانية مستهدفة للجمهور المحدد</td><td style="color:#feca57;font-weight:700;">🟡 متوسطة</td></tr>
    <tr><td>Success Stories</td><td>توثيق قصص نجاح حقيقية بشكل Documentary</td><td style="color:#48dbfb;font-weight:700;">🟢 مستمرة</td></tr>
    <tr><td>Coach Development Content</td><td>محتوى يبرز صناعة المدربين كقيمة أساسية</td><td style="color:#48dbfb;font-weight:700;">🟢 مستمرة</td></tr>
  </table>
  <h3 class="sub-heading">📞 Contact & Approval:</h3>
  <div class="highlight-box">
    <p><strong>الشخص المسؤول:</strong> أحمد المهدي — Founder & Managing Director</p>
    <p style="margin-top:8px;"><strong>الأكاديمية:</strong> Blue Dragon Swim Academy</p>
    <p style="margin-top:8px;"><strong>الموقع:</strong> المحلة الكبرى، مصر</p>
    <p style="margin-top:8px;"><strong>الفروع:</strong> نادي العدوي | نادي الشرطة</p>
  </div>
  <div class="quote-box" style="text-align:center;">
    <p style="font-size:15px;font-weight:700;color:#fff;font-style:normal;">"أي سؤال أو استفسار — أنا متاح. المهم إننا نبني حاجة تستحق."<br><span style="color:#7eb8e8;font-weight:400;">— أحمد المهدي</span></p>
  </div>
</div>

<!-- FOOTER -->
<div class="page-footer">
  <p>© 2026 Blue Dragon Swim Academy | Confidential Creative Brief</p>
  <p style="margin-top:5px;">Prepared by Ahmed El-Mahdi | All Rights Reserved</p>
</div>

</div>

</body>
</html>
