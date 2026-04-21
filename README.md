<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<title>نظام إسلام خالد حسان ERP</title>

<style>
body {
  margin:0;
  font-family: Arial;
  background: #0b1e2d;
  color: white;
}

/* الهيدر */
.header {
  padding:15px;
  text-align:center;
  font-size:22px;
  font-weight:bold;
}

/* البروفايل */
.profile {
  text-align:center;
  padding:20px;
}

.profile img {
  width:120px;
  height:120px;
  border-radius:50%;
  border:3px solid gold;
}

/* الاسم */
.name {
  font-size:24px;
  color:#f9b233;
  margin-top:10px;
}

/* الكروت */
.cards {
  display:grid;
  grid-template-columns: repeat(2,1fr);
  gap:10px;
  padding:15px;
}

.card {
  background:#122b3d;
  padding:15px;
  border-radius:10px;
  text-align:center;
}

.card h3 {
  margin:5px;
}

/* الأقسام */
.menu {
  display:grid;
  grid-template-columns: repeat(3,1fr);
  gap:10px;
  padding:15px;
}

.menu div {
  background:#16384f;
  padding:15px;
  text-align:center;
  border-radius:10px;
}

/* المشاريع */
.project {
  background:#122b3d;
  margin:10px;
  padding:10px;
  border-radius:10px;
}

.progress {
  height:6px;
  background:#333;
  border-radius:5px;
  margin-top:5px;
}

.progress span {
  display:block;
  height:100%;
  background:green;
  border-radius:5px;
}

</style>
</head>

<body>

<div class="header">لوحة التحكم</div>

<div class="profile">
  <!-- ضع صورتك هنا -->
  <img src="profile.jpg">
  <div class="name">إسلام خالد حسان</div>
  <div>مدير النظام</div>
</div>

<!-- الإحصائيات -->
<div class="cards">
  <div class="card">
    <h3>الإيرادات</h3>
    <p id="income">0</p>
  </div>

  <div class="card">
    <h3>المصروفات</h3>
    <p id="expense">0</p>
  </div>

  <div class="card">
    <h3>الربح</h3>
    <p id="profit">0</p>
  </div>

  <div class="card">
    <h3>المشاريع</h3>
    <p>5</p>
  </div>
</div>

<!-- الأقسام -->
<div class="menu">
  <div>المحاسبة</div>
  <div>المشاريع</div>
  <div>المخزون</div>
  <div>الموظفين</div>
  <div>التقارير</div>
  <div>الإعدادات</div>
</div>

<!-- المشاريع -->
<div class="project">
  مشروع مبنى إداري - 450,000 ريال
  <div class="progress"><span style="width:65%"></span></div>
</div>

<div class="project">
  مشروع سكني - 780,000 ريال
  <div class="progress"><span style="width:40%"></span></div>
</div>

<div class="project">
  فيلا خاصة - 250,000 ريال
  <div class="progress"><span style="width:90%"></span></div>
</div>

<script>

// بيانات تجريبية
let income = 256850;
let expense = 182430;

// حساب الربح تلقائي
let profit = income - expense;

document.getElementById("income").innerText = income + " ريال";
document.getElementById("expense").innerText = expense + " ريال";
document.getElementById("profit").innerText = profit + " ريال";

</script>

</body>
</html>
