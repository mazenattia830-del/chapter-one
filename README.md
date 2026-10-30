# chapter-one
<!doctype html>
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta name="theme-color" content="#171411">
<title>Chapter One | كافيه</title>
<style>
:root{--bg:#f4eee5;--ink:#211b16;--dark:#171411;--brown:#725039;--tan:#d8c2a4;--muted:#786f66;--white:#fffdf9;--line:#e7dccd;--gold:#c49a62}
*{box-sizing:border-box}html{scroll-behavior:smooth}body{margin:0;background:var(--bg);color:var(--ink);font-family:Tahoma,Arial,sans-serif}
button,input,textarea,select{font:inherit}button{cursor:pointer}
.top{background:var(--dark);color:#f8efe4;padding:14px 5%;display:flex;align-items:center;justify-content:space-between;gap:12px;position:sticky;top:0;z-index:5;box-shadow:0 4px 18px #0002}
.brand{font-family:Georgia,serif;font-size:24px;letter-spacing:1px;font-weight:bold}.brand small{display:block;font:11px Tahoma;color:#cbb79e;letter-spacing:3px;margin-top:3px}
.top-actions{display:flex;gap:8px;align-items:center}.pill{border:1px solid #9b8268;background:transparent;color:#fff4e6;border-radius:24px;padding:9px 14px}.cart-top{background:var(--gold);color:#1c1712;border:0;font-weight:bold}
.hero{background:linear-gradient(90deg,#171411ed,#17141185),url('https://images.unsplash.com/photo-1445116572660-236099ec97a0?auto=format&fit=crop&w=1800&q=85') center/cover;min-height:330px;color:#fff4e6;padding:64px 7%;display:flex;align-items:center}
.hero-inner{max-width:650px}.eyebrow{color:#dfbd8e;letter-spacing:3px;font-size:12px}.hero h1{font:clamp(42px,7vw,76px) Georgia,serif;margin:12px 0}.hero p{color:#eee0ce;line-height:1.9;max-width:520px}.cta{background:var(--gold);border:0;border-radius:28px;padding:13px 24px;font-weight:bold;color:#1b1712;margin-top:10px}
.wrap{max-width:1200px;margin:auto;padding:34px 5%}.section-head{display:flex;justify-content:space-between;align-items:end;gap:12px;margin-bottom:20px}.section-head h2{margin:0;font:30px Georgia,serif}.section-head p{color:var(--muted);margin:7px 0 0;font-size:13px}
.tools{display:flex;gap:10px;flex-wrap:wrap;margin:18px 0}.search{flex:1;min-width:180px;border:1px solid var(--line);border-radius:12px;padding:12px 14px;background:var(--white);outline:none}.filters{display:flex;gap:8px;overflow:auto;padding:3px 0 12px}.filter{white-space:nowrap;border:1px solid var(--line);background:var(--white);color:var(--brown);padding:9px 14px;border-radius:22px}.filter.active{background:var(--dark);color:#fff;border-color:var(--dark)}
.grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:14px}.item{background:var(--white);border:1px solid var(--line);border-radius:16px;padding:16px;display:flex;flex-direction:column;min-height:166px;box-shadow:0 5px 18px #4c32100a}.item-top{display:flex;justify-content:space-between;gap:10px;align-items:flex-start}.item h3{font-size:16px;margin:0 0 8px;line-height:1.5}.price{font-weight:bold;color:var(--brown);white-space:nowrap}.category{font-size:11px;color:var(--muted);margin-bottom:14px}.item-foot{display:flex;justify-content:space-between;align-items:center;margin-top:auto}.add{background:var(--dark);color:#fff;border:0;border-radius:10px;width:38px;height:38px;font-size:23px}.add:active{transform:scale(.95)}
.cart-panel{position:fixed;left:16px;bottom:16px;z-index:10;background:var(--dark);color:#fff;padding:12px 16px;border-radius:16px;box-shadow:0 8px 28px #0004;display:flex;gap:14px;align-items:center}.cart-panel button{background:var(--gold);border:0;border-radius:10px;padding:10px 14px;font-weight:bold}.count{background:#fff;color:var(--dark);border-radius:50%;width:24px;height:24px;display:inline-grid;place-items:center;font-size:12px}
.modal{display:none;position:fixed;inset:0;background:#0009;z-index:20;padding:16px;overflow:auto}.modal.show{display:block}.dialog{max-width:680px;margin:20px auto;background:var(--white);border-radius:20px;padding:22px;box-shadow:0 15px 50px #0004}.dialog-head{display:flex;justify-content:space-between;align-items:center}.dialog h2{margin:0}.close{border:0;background:#eee4d8;border-radius:50%;width:36px;height:36px;font-size:20px}
.cart-line{padding:12px 0;border-bottom:1px solid var(--line);display:grid;grid-template-columns:1fr auto;gap:8px}.line-title{font-weight:bold}.line-sub{font-size:12px;color:var(--muted);margin-top:4px}.qty{display:flex;gap:8px;align-items:center}.qty button{border:0;background:#eee4d8;border-radius:8px;width:28px;height:28px}.note{width:100%;padding:9px;border:1px solid var(--line);border-radius:9px;margin-top:8px;background:#fff}
.total{display:flex;justify-content:space-between;font-size:20px;font-weight:bold;padding:16px 0}.form-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px}.field{display:flex;flex-direction:column;gap:6px;margin:8px 0}.field label{font-size:13px;color:var(--muted)}.field input,.field textarea,.field select{border:1px solid var(--line);border-radius:10px;padding:11px;background:white;min-width:0}.field.full{grid-column:1/-1}.submit{width:100%;background:#218c55;color:white;border:0;border-radius:12px;padding:14px;font-weight:bold;margin-top:12px}.hint{font-size:12px;color:var(--muted);line-height:1.7}
footer{background:var(--dark);color:#e9d9c5;text-align:center;padding:30px 15px;margin-top:40px}footer strong{font:24px Georgia,serif}
.empty{text-align:center;color:var(--muted);padding:20px}
@media(max-width:760px){.grid{grid-template-columns:repeat(2,minmax(0,1fr))}.hero{min-height:280px;padding:45px 6%}.wrap{padding:26px 4%}.top{padding:12px 4%}.brand{font-size:21px}}
@media(max-width:430px){.grid{grid-template-columns:1fr 1fr;gap:9px}.item{padding:12px;min-height:155px}.item h3{font-size:14px}.price{font-size:13px}.hero h1{font-size:45px}.form-grid{grid-template-columns:1fr}.field.full{grid-column:auto}.cart-panel{left:10px;right:10px;bottom:10px;justify-content:space-between}}
</style>
</head>
<body>
<header class="top">
  <div class="brand">CHAPTER ONE<small>COFFEE • FOOD • MOMENTS</small></div>
  <div class="top-actions"><a class="pill" href="#menu" style="text-decoration:none">المنيو</a><button class="pill cart-top" onclick="openCart()">السلة <span id="topCount">0</span></button></div>
</header>
<section class="hero">
  <div class="hero-inner"><div class="eyebrow">YOUR NEXT FAVORITE CHAPTER</div><h1>Chapter One</h1><p>كل حكاية حلوة بتبدأ بفنجان قهوة. اختار مشروبك المفضل واستمتع بوقتك معانا.</p><button class="cta" onclick="document.getElementById('menu').scrollIntoView()">اكتشف المنيو</button></div>
</section>
<main class="wrap" id="menu">
  <div class="section-head"><div><h2>Our Menu</h2><p>اختار من منيو Chapter One وأضف طلبك للسلة</p></div><span class="eyebrow">CHAPTER 01 — 07</span></div>
  <div class="tools"><input id="search" class="search" placeholder="ابحث عن منتج..." oninput="renderMenu()"></div>
  <div class="filters" id="filters"></div>
  <div class="grid" id="products"></div>
</main>
<div class="cart-panel"><div>السلة <span class="count" id="cartCount">0</span> <strong id="miniTotal">0 جنيه</strong></div><button onclick="openCart()">عرض الطلب</button></div>
<footer><strong>Chapter One</strong><p>Made for coffee lovers.</p><small>جميع الأسعار بالجنيه المصري EGP</small></footer>
<div class="modal" id="cartModal" onclick="if(event.target===this)closeCart()">
 <div class="dialog">
  <div class="dialog-head"><h2>سلة الطلبات</h2><button class="close" onclick="closeCart()">×</button></div>
  <div id="cartLines"></div>
  <div class="total"><span>الإجمالي</span><span id="total">0 جنيه</span></div>
  <h3>بيانات الطلب</h3>
  <div class="form-grid">
   <div class="field"><label>اسم العميل</label><input id="customer" placeholder="اسمك"></div>
   <div class="field"><label>رقم الهاتف</label><input id="phone" inputmode="tel" placeholder="01xxxxxxxxx"></div>
   <div class="field full"><label>طريقة الاستلام</label><select id="method" onchange="toggleOrderFields()"><option value="داخل الكافيه">داخل الكافيه</option><option value="استلام من الفرع">استلام من الفرع</option><option value="توصيل للعنوان">توصيل للعنوان</option></select></div>
   <div class="field" id="tableField"><label>رقم الطاولة (إجباري)</label><input id="table" placeholder="مثال: 7" inputmode="numeric"></div>
   <div class="field" id="addressField" style="display:none"><label>عنوان التوصيل</label><input id="address" placeholder="اكتب العنوان بالتفصيل"></div>
   <div class="field full"><label>ملاحظات الطلب</label><textarea id="orderNotes" rows="2" placeholder="أي تفاصيل إضافية..."></textarea></div>
  </div>
  <p class="hint">بعد الضغط على تأكيد الطلب، هيفتح واتساب برسالة جاهزة بكل المنتجات والكميات والأسعار ورقم الطاولة. اضغط إرسال داخل واتساب لإتمام الطلب.</p>
  <button class="submit" onclick="sendWhatsApp()">تأكيد الطلب عبر واتساب</button>
 </div>
</div>
<script>
const menu = [
["Chapter 01 – المشروبات الساخنة والقهوة",[
["قهوة تركي سنجل",30],["قهوة تركي دبل",40],["قهوة فرنساوي",40],["قهوة بندق",50],["شاي",20],["شاي بحليب",30],["شاي أخضر",20],["ينسون",20],["قرفة",20],["قرفة بحليب",30],["جنزبيل",20],["كركديه",20],["ليمون",20],["كوكتيل أعشاب",40],["سحلب",50],["سحلب فواكه",60],["اندومي",25],["كوفي ميكس",25],["هوت سيدر",45],["اسبانيش لاتيه",65],["موكا",65],["فلات وايت",50],["كابتشينو",60],["ميكاتو",45],["ميكاتو دبل",50],["كرتادو",45],["نسكافيه بلاك",35],["أمريكانو",40],["اسبريسو سنجل",35],["اسبريسو دبل",45]]],
["Chapter 02 – العصائر الفريش",[
["ليمون",45],["ليمون نعناع",50],["فراولة",60],["فراولة بلبن",65],["مانجو",70],["برتقال",50],["جوافة",50],["موز بلبن",60],["أفوكادو",90],["كيوي",80],["مانجو كيوي",80],["زبادي عسل",60],["زبادي فواكه",75],["عنب",35],["فلوريدا",80]]],
["Chapter 03 – آيس كوفي وموهيتو",[
["آيس كوفي",55],["آيس لاتيه",60],["آيس موكا",70],["آيس أمريكانو",45],["آيس سبانش لاتيه",70],["آيس ريدبول كوفي",100],["موهيتو كلاسيك",60],["موهيتو فراولة",70],["موهيتو بلوبيري",70],["موهيتو ميكس بيري",75],["موهيتو باشن فروت",70],["موهيتو ريدبول",105],["صن شاين",70],["بلو أوشن",85]]],
["Chapter 04 – ميلك شيك وديزرت",[
["ميلك شيك أوريو",65],["ميلك شيك بلوبيري",65],["ميلك شيك ميكس بيري",75],["ميلك شيك لوتس",80],["ميلك شيك كراميل",60],["ميلك شيك نوتيلا",80],["ميلك شيك تشيز",95],["شوكليت فادج",70],["ريد فلفت",80],["مولتن كيك",85],["مولتن لوتس",95],["مولتن كيت كات",105],["تشيز كيك",70]]],
["Chapter 05 – آيس كريم ومشروبات غازية وإضافات",[
["آيس كريم Chapter One",50],["بيبسي",30],["فيروز",35],["كولا",30],["فيوري",35],["شويبس",30],["بيريل",35],["ريدبول",85],["مونستر",80],["تويست",35],["إضافة فليفر",10],["إضافة صوص",15],["إضافة عسل",15],["إضافة بولة آيس كريم",20],["إضافة شوت إسبريسو",25]]],
["Chapter 06 – خدمات الفرع",[
["روم 1 (شاملة بلايستيشن ساعة)",50],["روم 2 (شاملة بلايستيشن ساعة)",50],["كارت نت",12]]],
["Chapter 07 – سموذي",[
["سموذي بلوبيري",60],["سموذي فراولة",65],["سموذي مانجو",75],["سموذي بطيخ",60],["سموذي ليمون نعناع",60],["سموذي خوخ",55]]]
];
let active=0, cart={};
const money=n=>`${n} جنيه`;
function allProducts(){return menu.flatMap((cat,ci)=>cat[1].map((p,pi)=>({id:`${ci}-${pi}`,name:p[0],price:p[1],category:cat[0]})))}
const products=allProducts();
function renderFilters(){document.getElementById('filters').innerHTML=`<button class="filter ${active===-1?'active':''}" onclick="setCategory(-1)">الكل</button>`+menu.map((c,i)=>`<button class="filter ${active===i?'active':''}" onclick="setCategory(${i})">${c[0].replace(/^Chapter \\d+ – /,'')}</button>`).join('')}
function setCategory(i){active=i;renderFilters();renderMenu()}
function renderMenu(){
 const q=document.getElementById('search').value.trim().toLowerCase();
 const shown=products.filter(p=>(active===-1||p.category===menu[active][0])&&p.name.toLowerCase().includes(q));
 document.getElementById('products').innerHTML=shown.map(p=>`<article class="item"><div class="item-top"><div><h3>${p.name}</h3><div class="category">${p.category}</div></div><div class="price">${money(p.price)}</div></div><div class="item-foot"><span class="hint">متاح للطلب</span><button class="add" aria-label="إضافة ${p.name}" onclick="addItem('${p.id}')">+</button></div></article>`).join('')||'<div class="empty">مفيش منتجات مطابقة للبحث.</div>';
}
function addItem(id){if(!cart[id])cart[id]={qty:0,note:''};cart[id].qty++;updateCart()}
function changeQty(id,d){if(!cart[id])return;cart[id].qty+=d;if(cart[id].qty<=0)delete cart[id];updateCart()}
function updateNote(id,v){if(cart[id])cart[id].note=v}
function cartEntries(){return products.filter(p=>cart[p.id])}
function totalCount(){return Object.values(cart).reduce((s,x)=>s+x.qty,0)}
function totalPrice(){return cartEntries().reduce((s,p)=>s+p.price*cart[p.id].qty,0)}
function updateCart(){
 const count=totalCount(),total=totalPrice();
 ['topCount','cartCount'].forEach(id=>document.getElementById(id).textContent=count);
 document.getElementById('miniTotal').textContent=money(total);
 document.getElementById('total').textContent=money(total);
 document.getElementById('cartLines').innerHTML=cartEntries().map(p=>`<div class="cart-line"><div><div class="line-title">${p.name} — ${money(p.price)}</div><div class="line-sub">الإجمالي: ${money(p.price*cart[p.id].qty)}</div><input class="note" placeholder="ملاحظات على المنتج (اختياري)" value="${escapeAttr(cart[p.id].note)}" oninput="updateNote('${p.id}',this.value)"></div><div class="qty"><button onclick="changeQty('${p.id}',-1)">−</button><b>${cart[p.id].qty}</b><button onclick="changeQty('${p.id}',1)">+</button></div></div>`).join('')||'<div class="empty">السلة فارغة. أضف منتجات من المنيو.</div>';
}
function escapeAttr(s){return String(s).replaceAll('&','&amp;').replaceAll('"','&quot;').replaceAll('<','&lt;').replaceAll('>','&gt;')}
function openCart(){document.getElementById('cartModal').classList.add('show');updateCart()}
function closeCart(){document.getElementById('cartModal').classList.remove('show')}
function toggleOrderFields(){const m=document.getElementById('method').value;document.getElementById('tableField').style.display=m==='داخل الكافيه'?'flex':'none';document.getElementById('addressField').style.display=m==='توصيل للعنوان'?'flex':'none'}
function sendWhatsApp(){
 const entries=cartEntries();if(!entries.length){alert('السلة فارغة. أضف منتجًا أولاً.');return}
 const name=document.getElementById('customer').value.trim(),phone=document.getElementById('phone').value.trim(),method=document.getElementById('method').value,table=document.getElementById('table').value.trim(),address=document.getElementById('address').value.trim();
 if(!name||!phone){alert('من فضلك اكتب اسم العميل ورقم الهاتف.');return}
 if(method==='داخل الكافيه'&&!table){alert('من فضلك اكتب رقم الطاولة.');return}
 if(method==='توصيل للعنوان'&&!address){alert('من فضلك اكتب عنوان التوصيل.');return}
 let lines=['☕ *طلب جديد من Chapter One*','━━━━━━━━━━━━━━',`👤 الاسم: ${name}`,`📞 الهاتف: ${phone}`,`📍 نوع الطلب: ${method}`];
 if(method==='داخل الكافيه')lines.push(`🪑 رقم الطاولة: ${table}`);
 if(method==='توصيل للعنوان')lines.push(`🏠 العنوان: ${address}`);
 lines.push('','🧾 *تفاصيل الطلب:*');
 entries.forEach(p=>{lines.push(`• ${p.name} × ${cart[p.id].qty} = ${p.price*cart[p.id].qty} جنيه`);if(cart[p.id].note)lines.push(`  ملاحظة: ${cart[p.id].note}`)});
 lines.push('','━━━━━━━━━━━━━━',`💰 *الإجمالي: ${totalPrice()} جنيه*`);
 const notes=document.getElementById('orderNotes').value.trim();if(notes)lines.push(`📝 ملاحظات الطلب: ${notes}`);
 lines.push('','تم إرسال الطلب من موقع Chapter One.');
 const url='https://wa.me/201029133687?text='+encodeURIComponent(lines.join('\n'));
 window.open(url,'_blank');
}
renderFilters();renderMenu();updateCart();toggleOrderFields();
</script>
</body>
</html>