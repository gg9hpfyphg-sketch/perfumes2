<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Genaro, Tomás T Gian — Fine Fragrances</title>
<meta name="description" content="Modern, bold and timeless perfumes. Browse our collection and order online.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
:root{--bg:#0e0d0c;--bg2:#171513;--card:#1c1916;--line:#2e2924;--text:#f3ece2;--muted:#a79d90;--gold:#c9a45c;--gold2:#e6c98a;--radius:18px}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--text);font-family:'Inter',system-ui,sans-serif;font-weight:300;line-height:1.6}
h1,h2,h3,.serif{font-family:'Cormorant Garamond',Georgia,serif;font-weight:500}
a{color:inherit;text-decoration:none}
button{font:inherit;cursor:pointer;border:0;background:none;color:inherit}
.wrap{max-width:1200px;margin:0 auto;padding:0 20px}

/* header */
header{position:sticky;top:0;z-index:50;background:rgba(14,13,12,.85);backdrop-filter:blur(12px);border-bottom:1px solid var(--line)}
.nav{display:flex;align-items:center;justify-content:space-between;height:70px}
.logo{font-family:'Cormorant Garamond',serif;font-size:1.45rem;font-weight:600;letter-spacing:.04em}
.logo span{color:var(--gold)}
.navlinks{display:flex;gap:28px;font-size:.85rem;letter-spacing:.12em;text-transform:uppercase}
.navlinks a{color:var(--muted);transition:.2s}.navlinks a:hover{color:var(--gold2)}
.cartbtn{position:relative;display:flex;gap:8px;align-items:center;border:1px solid var(--gold);color:var(--gold2);padding:9px 18px;border-radius:40px;font-size:.85rem;letter-spacing:.08em;text-transform:uppercase;transition:.2s}
.cartbtn:hover{background:var(--gold);color:#111}
.badge{background:var(--gold);color:#111;border-radius:50%;width:20px;height:20px;font-size:.72rem;font-weight:600;display:grid;place-items:center}
.cartbtn:hover .badge{background:#111;color:var(--gold2)}

/* hero */
.hero{position:relative;overflow:hidden;padding:110px 0 100px;background:radial-gradient(1000px 500px at 80% 20%,#3a2c17 0%,transparent 60%),radial-gradient(800px 500px at 0% 100%,#1f2a3a 0%,transparent 60%),var(--bg)}
.hero-grid{display:grid;grid-template-columns:1.1fr .9fr;gap:40px;align-items:center}
.eyebrow{color:var(--gold);letter-spacing:.3em;text-transform:uppercase;font-size:.75rem;margin-bottom:18px}
.hero h1{font-size:clamp(2.8rem,7vw,5.4rem);line-height:1;margin-bottom:22px}
.hero h1 em{color:var(--gold2);font-style:italic}
.hero p{color:var(--muted);max-width:480px;font-size:1.05rem;margin-bottom:34px}
.btn{display:inline-block;background:linear-gradient(135deg,var(--gold2),var(--gold));color:#15110b;padding:15px 36px;border-radius:40px;font-weight:500;letter-spacing:.1em;text-transform:uppercase;font-size:.82rem;transition:.25s;box-shadow:0 10px 30px -10px rgba(201,164,92,.6)}
.btn:hover{transform:translateY(-2px);box-shadow:0 14px 34px -8px rgba(201,164,92,.75)}
.btn.ghost{background:none;border:1px solid var(--line);color:var(--text);box-shadow:none;margin-left:10px}
.hero-art{display:flex;justify-content:center;gap:10px;align-items:flex-end}
.hero-art svg{filter:drop-shadow(0 30px 40px rgba(0,0,0,.6));animation:float 6s ease-in-out infinite}
.hero-art svg:nth-child(2){animation-delay:-2s;transform:scale(1.15)}
.hero-art svg:nth-child(3){animation-delay:-4s}
@keyframes float{50%{translate:0 -12px}}

.perks{display:grid;grid-template-columns:repeat(4,1fr);gap:20px;padding:34px 0;border-bottom:1px solid var(--line);text-align:center;font-size:.82rem;letter-spacing:.1em;text-transform:uppercase;color:var(--muted)}
.perks b{display:block;color:var(--gold2);font-weight:500;font-size:.9rem;margin-bottom:2px}

/* shop */
section{padding:80px 0}
.sec-head{text-align:center;margin-bottom:40px}
.sec-head h2{font-size:clamp(2rem,4vw,3rem)}
.sec-head p{color:var(--muted)}
.tools{display:flex;flex-wrap:wrap;gap:14px;justify-content:space-between;align-items:center;margin-bottom:34px}
.chips{display:flex;gap:8px;flex-wrap:wrap}
.chip{padding:9px 20px;border:1px solid var(--line);border-radius:40px;font-size:.8rem;letter-spacing:.08em;text-transform:uppercase;color:var(--muted);transition:.2s}
.chip:hover{border-color:var(--gold);color:var(--text)}
.chip.on{background:var(--gold);border-color:var(--gold);color:#15110b;font-weight:500}
.ctrls{display:flex;gap:10px;flex-wrap:wrap}
input,select,textarea{background:var(--bg2);border:1px solid var(--line);color:var(--text);padding:11px 16px;border-radius:12px;font:inherit;font-size:.9rem;outline:none;transition:.2s;width:100%}
.ctrls input,.ctrls select{width:auto;min-width:170px}
input:focus,select:focus,textarea:focus{border-color:var(--gold)}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:24px}
.card{background:var(--card);border:1px solid var(--line);border-radius:var(--radius);overflow:hidden;display:flex;flex-direction:column;transition:.3s}
.card:hover{transform:translateY(-6px);border-color:#4a3e2a;box-shadow:0 24px 50px -24px rgba(0,0,0,.8)}
.thumb{display:grid;place-items:center;padding:28px 0 12px;background:radial-gradient(circle at 50% 60%,var(--glow) 0%,transparent 70%),var(--bg2);position:relative}
.tag{position:absolute;top:14px;left:14px;font-size:.68rem;letter-spacing:.14em;text-transform:uppercase;background:rgba(0,0,0,.45);padding:4px 10px;border-radius:20px;color:var(--gold2)}
.info{padding:18px 20px 22px;display:flex;flex-direction:column;gap:6px;flex:1}
.fam{font-size:.72rem;letter-spacing:.16em;text-transform:uppercase;color:var(--gold)}
.info h3{font-size:1.6rem;line-height:1.1}
.notes{color:var(--muted);font-size:.84rem;flex:1}
.sizes{display:flex;gap:6px;margin:8px 0 4px}
.sz{flex:1;padding:7px 0;border:1px solid var(--line);border-radius:10px;font-size:.78rem;color:var(--muted);transition:.2s}
.sz.on{border-color:var(--gold);color:var(--gold2);background:rgba(201,164,92,.08)}
.buy{display:flex;align-items:center;justify-content:space-between;margin-top:8px}
.price{font-family:'Cormorant Garamond',serif;font-size:1.7rem;font-weight:600}
.add{background:var(--gold);color:#15110b;padding:10px 18px;border-radius:30px;font-size:.78rem;letter-spacing:.1em;text-transform:uppercase;font-weight:500;transition:.2s}
.add:hover{background:var(--gold2)}
.empty{text-align:center;color:var(--muted);padding:60px 0;grid-column:1/-1}

/* story */
.story{background:var(--bg2);border-block:1px solid var(--line)}
.story-grid{display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center}
.story h2{font-size:clamp(2rem,4vw,3.2rem);margin-bottom:18px}
.story p{color:var(--muted);margin-bottom:14px}
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:26px}
.stats div{border:1px solid var(--line);border-radius:14px;padding:18px;text-align:center}
.stats b{display:block;font-family:'Cormorant Garamond',serif;font-size:2rem;color:var(--gold2);font-weight:600}
.stats span{font-size:.75rem;letter-spacing:.1em;text-transform:uppercase;color:var(--muted)}

footer{padding:50px 0 30px;text-align:center;color:var(--muted);font-size:.85rem}
footer .logo{display:block;margin-bottom:10px;color:var(--text)}
footer .links{display:flex;justify-content:center;gap:24px;margin:14px 0 22px}

/* cart drawer */
.overlay{position:fixed;inset:0;background:rgba(0,0,0,.6);opacity:0;pointer-events:none;transition:.3s;z-index:90}
.overlay.on{opacity:1;pointer-events:auto}
.drawer{position:fixed;top:0;right:0;height:100%;width:min(440px,100%);background:var(--bg2);border-left:1px solid var(--line);z-index:100;transform:translateX(100%);transition:.35s cubic-bezier(.2,.8,.2,1);display:flex;flex-direction:column}
.drawer.on{transform:none}
.d-head{display:flex;justify-content:space-between;align-items:center;padding:22px 24px;border-bottom:1px solid var(--line)}
.d-head h3{font-size:1.7rem}
.x{font-size:1.6rem;color:var(--muted);line-height:1}
.d-body{flex:1;overflow:auto;padding:16px 24px}
.item{display:grid;grid-template-columns:56px 1fr auto;gap:14px;align-items:center;padding:14px 0;border-bottom:1px solid var(--line)}
.item .mini{background:var(--card);border-radius:10px;display:grid;place-items:center;height:70px}
.item h4{font-family:'Cormorant Garamond',serif;font-size:1.2rem;font-weight:600;line-height:1.1}
.item small{color:var(--muted)}
.qty{display:inline-flex;align-items:center;gap:10px;margin-top:6px;border:1px solid var(--line);border-radius:20px;padding:2px 10px}
.qty button{font-size:1.1rem;color:var(--gold2);width:18px}
.rm{color:var(--muted);font-size:.75rem;text-decoration:underline;display:block;margin-top:4px;text-align:right}
.d-foot{padding:20px 24px;border-top:1px solid var(--line);background:var(--bg)}
.tot{display:flex;justify-content:space-between;font-size:1.1rem;margin-bottom:14px}
.tot b{font-family:'Cormorant Garamond',serif;font-size:1.8rem;color:var(--gold2)}
.d-foot .btn{width:100%;text-align:center;border:0}
.note-free{font-size:.78rem;color:var(--muted);margin-bottom:12px}
.form{display:grid;gap:10px;margin-top:6px}
.form.hide,.hide{display:none}
.row2{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.back{color:var(--muted);font-size:.82rem;text-decoration:underline;margin-bottom:6px}
.toast{position:fixed;bottom:26px;left:50%;translate:-50% 120px;background:var(--gold);color:#15110b;padding:12px 26px;border-radius:40px;font-weight:500;z-index:200;transition:.4s;font-size:.9rem}
.toast.on{translate:-50% 0}
@media(max-width:820px){
 .navlinks{display:none}.hero-grid,.story-grid{grid-template-columns:1fr}.hero{padding:70px 0}.hero-art{order:-1}
 .perks{grid-template-columns:repeat(2,1fr)}section{padding:56px 0}.ctrls input,.ctrls select{flex:1;min-width:0}.btn.ghost{margin:10px 0 0}
}
</style>
</head>
<body>

<header>
 <div class="wrap nav">
  <a href="#top" class="logo">Genaro, Tomás <span>T</span> Gian</a>
  <nav class="navlinks"><a href="#shop">Shop</a><a href="#story">Our Story</a><a href="#contact">Contact</a></nav>
  <button class="cartbtn" id="openCart" aria-label="Open cart">Cart <span class="badge" id="count">0</span></button>
 </div>
</header>

<main id="top">
<div class="hero">
 <div class="wrap hero-grid">
  <div>
   <div class="eyebrow">Eau de Parfum · New Season</div>
   <h1>Wear your <em>signature.</em></h1>
   <p>Bold, modern and unforgettable fragrances — from creamy tonka and sparkling bergamot to deep smoky woods. Find the scent that speaks before you do.</p>
   <a href="#shop" class="btn">Shop the collection</a>
   <a href="#story" class="btn ghost">Our story</a>
  </div>
  <div class="hero-art" id="heroArt"></div>
 </div>
</div>

<div class="wrap perks">
 <div><b>Authentic Quality</b>Long-lasting formulas</div>
 <div><b>Free Samples</b>With every order</div>
 <div><b>Fast Shipping</b>Packed with care</div>
 <div><b>Gift Ready</b>Premium packaging</div>
</div>

<section id="shop">
 <div class="wrap">
  <div class="sec-head"><div class="eyebrow">The Collection</div><h2>Find your scent</h2><p>24 fragrances · 50 ml &amp; 100 ml · Prices in USD</p></div>
  <div class="tools">
   <div class="chips" id="chips"></div>
   <div class="ctrls">
    <input id="q" type="search" placeholder="Search name or notes…">
    <select id="sort">
     <option value="feat">Featured</option>
     <option value="asc">Price: low to high</option>
     <option value="desc">Price: high to low</option>
     <option value="az">Name: A–Z</option>
    </select>
   </div>
  </div>
  <div class="grid" id="grid"></div>
 </div>
</section>

<section class="story" id="story">
 <div class="wrap story-grid">
  <div>
   <div class="eyebrow">Our Story</div>
   <h2>Three friends. One obsession.</h2>
   <p>We're Genaro, Tomás and Gian. What started as a shared passion for rare ingredients and bold compositions became a place where fragrance lovers find something truly theirs.</p>
   <p>Every scent in our collection is chosen for its character, its longevity and the way it makes you feel when you walk into a room.</p>
   <div class="stats"><div><b>24</b><span>Fragrances</span></div><div><b>6</b><span>Families</span></div><div><b>3</b><span>Founders</span></div></div>
  </div>
  <div class="hero-art" id="storyArt"></div>
 </div>
</section>
</main>

<footer id="contact">
 <div class="wrap">
  <span class="logo">Genaro, Tomás T Gian</span>
  <div>Questions or special orders? Write to us.</div>
  <div class="links"><a id="waLink" href="#">WhatsApp</a><a id="mailLink" href="#">Email</a></div>
  <div>© 2026 Genaro, Tomás T Gian. All rights reserved.</div>
 </div>
</footer>

<div class="overlay" id="overlay"></div>
<aside class="drawer" id="drawer" aria-label="Shopping cart">
 <div class="d-head"><h3 id="dTitle">Your cart</h3><button class="x" id="closeCart" aria-label="Close">×</button></div>
 <div class="d-body" id="dBody"></div>
 <div class="d-foot" id="dFoot"></div>
</aside>
<div class="toast" id="toast"></div>

<script>
/* ============ SETTINGS — EDIT THESE ============ */
const WHATSAPP_NUMBER = "5491100000000";   // country code + number, digits only (e.g. 54911...)
const STORE_EMAIL     = "orders@example.com";
const CURRENCY        = "$";
const FREE_SHIPPING_OVER = 150;
/* =============================================== */

const P=[
{n:"Noir Tonka",f:"Woody Gourmand",g:"Men",p:89,c:["#17172a","#c9a45c"],t:"Bergamot · Tonka bean · Cedar",tag:"Bestseller"},
{n:"Coco Velvet",f:"Creamy Coconut",g:"Unisex",p:95,c:["#e8dcc6","#8a6a3b"],t:"Coconut milk · Vanilla · Sandalwood",tag:"Bestseller"},
{n:"Midnight Lavender",f:"Aromatic Fougère",g:"Men",p:79,c:["#2a1f4d","#a78bfa"],t:"Lavender · Mint · Amber"},
{n:"Rosa Eterna",f:"Floral",g:"Women",p:112,c:["#7a1f3d","#f4a6b8"],t:"Damask rose · Peony · Musk",tag:"New"},
{n:"Ambre Sauvage",f:"Amber Spicy",g:"Unisex",p:129,c:["#5a2d0c","#e0902b"],t:"Amber · Cardamom · Labdanum"},
{n:"Citrus Riviera",f:"Fresh Citrus",g:"Unisex",p:55,c:["#c98d00","#fbe27a"],t:"Lemon · Grapefruit · Neroli"},
{n:"Oud Imperial",f:"Oriental Oud",g:"Unisex",p:249,c:["#120d0a","#b3402a"],t:"Oud · Saffron · Leather",tag:"Luxury"},
{n:"Vanille Étoile",f:"Sweet Vanilla",g:"Women",p:98,c:["#f0d9b5","#b0773a"],t:"Madagascar vanilla · Caramel · Praline"},
{n:"Blue Horizon",f:"Aquatic Fresh",g:"Men",p:62,c:["#0b3a6b","#6ec6ff"],t:"Sea salt · Marine accord · Vetiver"},
{n:"Jasmin Nuit",f:"White Floral",g:"Women",p:118,c:["#222036","#f6efe2"],t:"Night jasmine · Tuberose · Ylang"},
{n:"Smoked Vetiver",f:"Woody Smoky",g:"Men",p:104,c:["#202a22","#7fa384"],t:"Vetiver · Birch tar · Black pepper"},
{n:"Pink Pepper Dream",f:"Fruity Spicy",g:"Women",p:72,c:["#b83b6c","#ffd1dc"],t:"Pink pepper · Raspberry · Praline"},
{n:"Santal Royale",f:"Creamy Woody",g:"Unisex",p:165,c:["#4a2f1a","#d9b383"],t:"Mysore sandalwood · Cashmeran · Iris"},
{n:"Electric Mint",f:"Fresh Aromatic",g:"Men",p:48,c:["#0f6b5b","#9ff5d8"],t:"Spearmint · Green apple · Musk"},
{n:"Cherry Noir",f:"Gourmand Fruity",g:"Women",p:109,c:["#3b0614","#e0245e"],t:"Black cherry · Almond · Tonka",tag:"New"},
{n:"Cuir Absolu",f:"Leather",g:"Men",p:138,c:["#2b1608","#a0522d"],t:"Suede · Birch · Incense"},
{n:"Fleur de Soleil",f:"Floral Fresh",g:"Women",p:66,c:["#e6a800","#fff3b0"],t:"Mimosa · Freesia · Pear"},
{n:"Iris Blanc",f:"Powdery Floral",g:"Women",p:145,c:["#d9d6e6","#6d6a8f"],t:"Orris butter · Violet · White musk"},
{n:"Black Rum",f:"Boozy Spicy",g:"Men",p:119,c:["#1a0d0a","#c06a2b"],t:"Dark rum · Cinnamon · Tobacco leaf"},
{n:"Mediterranean Fig",f:"Green Fruity",g:"Unisex",p:84,c:["#2e4a2c","#b9d58a"],t:"Fig leaf · Coconut water · Cedar"},
{n:"Rose Oud Gold",f:"Floral Oud",g:"Unisex",p:279,c:["#3a0a1c","#e6c98a"],t:"Bulgarian rose · Oud · Gold amber",tag:"Luxury"},
{n:"Cotton Cloud",f:"Soft Musk",g:"Unisex",p:42,c:["#cfe3f5","#ffffff"],t:"Cotton flower · White musk · Pear"},
{n:"Honey & Tobacco",f:"Sweet Tobacco",g:"Men",p:99,c:["#4a3008","#f0b23d"],t:"Honey · Tobacco · Vanilla bean"},
{n:"Orchidée Mystère",f:"Exotic Floral",g:"Women",p:132,c:["#3d1a52","#d79bff"],t:"Black orchid · Patchouli · Dark chocolate"}
].map((x,i)=>({...x,id:i+1}));

const SIZES=[{ml:50,m:1},{ml:100,m:1.7}];
const price=(p,ml)=>Math.round(p.p*SIZES.find(s=>s.ml===ml).m);
const fmt=n=>CURRENCY+n.toFixed(0);

function bottle(c,w=110,uid="b"){
 const [a,b]=c;
 return `<svg width="${w}" viewBox="0 0 120 170" aria-hidden="true">
 <defs><linearGradient id="g${uid}" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="${a}"/><stop offset="1" stop-color="${b}"/></linearGradient>
 <linearGradient id="s${uid}" x1="0" x2="1"><stop offset="0" stop-color="#fff" stop-opacity=".35"/><stop offset=".3" stop-color="#fff" stop-opacity="0"/><stop offset="1" stop-color="#000" stop-opacity=".25"/></linearGradient></defs>
 <rect x="46" y="6" width="28" height="22" rx="4" fill="#d8b46a"/><rect x="46" y="6" width="28" height="22" rx="4" fill="url(#s${uid})"/>
 <rect x="54" y="26" width="12" height="12" fill="#bfa159"/>
 <rect x="16" y="38" width="88" height="124" rx="16" fill="url(#g${uid})" stroke="rgba(255,255,255,.25)"/>
 <rect x="16" y="38" width="88" height="124" rx="16" fill="url(#s${uid})"/>
 <rect x="30" y="78" width="60" height="50" rx="4" fill="rgba(0,0,0,.18)" stroke="rgba(255,255,255,.35)" stroke-width=".7"/>
 <line x1="38" y1="96" x2="82" y2="96" stroke="rgba(255,255,255,.5)" stroke-width=".8"/>
 <circle cx="60" cy="108" r="3" fill="rgba(255,255,255,.6)"/>
 </svg>`;
}

/* state */
let cart=[];try{cart=JSON.parse(localStorage.getItem("cart")||"[]")}catch(e){}
const saveCart=()=>{try{localStorage.setItem("cart",JSON.stringify(cart))}catch(e){}};
let filter="All",sel={};
const $=id=>document.getElementById(id);

/* hero art */
const heroPicks=[P[1],P[6],P[0]];
$("heroArt").innerHTML=heroPicks.map((p,i)=>bottle(p.c,i===1?150:120,"h"+i)).join("");
$("storyArt").innerHTML=[P[3],P[20],P[8]].map((p,i)=>bottle(p.c,i===1?170:130,"s"+i)).join("");

/* chips */
const cats=["All","Women","Men","Unisex"];
$("chips").innerHTML=cats.map(c=>`<button class="chip ${c==="All"?"on":""}" data-c="${c}">${c}</button>`).join("");
$("chips").onclick=e=>{const c=e.target.dataset.c;if(!c)return;filter=c;[...$("chips").children].forEach(b=>b.classList.toggle("on",b.dataset.c===c));render()};
$("q").oninput=render;$("sort").onchange=render;

function render(){
 const q=$("q").value.trim().toLowerCase();
 let list=P.filter(p=>(filter==="All"||p.g===filter)&&(!q||(p.n+p.t+p.f).toLowerCase().includes(q)));
 const s=$("sort").value;
 if(s==="asc")list.sort((a,b)=>a.p-b.p);if(s==="desc")list.sort((a,b)=>b.p-a.p);if(s==="az")list.sort((a,b)=>a.n.localeCompare(b.n));
 $("grid").innerHTML=list.length?list.map(p=>{
  const ml=sel[p.id]||50;
  return `<article class="card"><div class="thumb" style="--glow:${p.c[1]}33">${p.tag?`<span class="tag">${p.tag}</span>`:""}${bottle(p.c,104,"p"+p.id)}</div>
  <div class="info"><span class="fam">${p.f} · ${p.g}</span><h3>${p.n}</h3><div class="notes">${p.t}</div>
  <div class="sizes">${SIZES.map(z=>`<button class="sz ${z.ml===ml?"on":""}" data-id="${p.id}" data-ml="${z.ml}">${z.ml} ml</button>`).join("")}</div>
  <div class="buy"><span class="price">${fmt(price(p,ml))}</span><button class="add" data-add="${p.id}">Add to cart</button></div></div></article>`}).join(""):`<div class="empty">No fragrances found. Try another search.</div>`;
}
$("grid").onclick=e=>{
 const z=e.target.closest(".sz");if(z){sel[z.dataset.id]=+z.dataset.ml;render();return}
 const a=e.target.closest("[data-add]");if(a){add(+a.dataset.add)}
};

/* cart */
function add(id){
 const ml=sel[id]||50,k=id+"-"+ml,it=cart.find(i=>i.k===k);
 it?it.q++:cart.push({k,id,ml,q:1});
 saveCart();updateCount();toast(P.find(p=>p.id===id).n+" added to cart");
 if(drawerOpen)renderCart();
}
const total=()=>cart.reduce((s,i)=>s+price(P.find(p=>p.id===i.id),i.ml)*i.q,0);
function updateCount(){$("count").textContent=cart.reduce((s,i)=>s+i.q,0)}
let drawerOpen=false,step="cart";
function openCart(){drawerOpen=true;step="cart";renderCart();$("drawer").classList.add("on");$("overlay").classList.add("on")}
function closeCart(){drawerOpen=false;$("drawer").classList.remove("on");$("overlay").classList.remove("on")}
$("openCart").onclick=openCart;$("closeCart").onclick=closeCart;$("overlay").onclick=closeCart;
document.addEventListener("keydown",e=>{if(e.key==="Escape")closeCart()});

function renderCart(){
 const body=$("dBody"),foot=$("dFoot");
 if(step==="done"){$("dTitle").textContent="Thank you!";body.innerHTML=`<p style="margin-top:30px;color:var(--muted)">Your order was prepared and sent. We'll confirm availability, shipping and payment details with you shortly.</p>`;foot.innerHTML=`<button class="btn" id="cont">Continue shopping</button>`;$("cont").onclick=closeCart;return}
 if(step==="checkout"){
  $("dTitle").textContent="Checkout";
  body.innerHTML=`<button class="back" id="bk">← Back to cart</button>
  <form class="form" id="f">
   <input required name="name" placeholder="Full name" autocomplete="name">
   <div class="row2"><input required type="email" name="email" placeholder="Email" autocomplete="email"><input required name="phone" placeholder="Phone / WhatsApp" autocomplete="tel"></div>
   <input required name="addr" placeholder="Street address" autocomplete="street-address">
   <div class="row2"><input required name="city" placeholder="City"><input required name="zip" placeholder="Postal code"></div>
   <input required name="country" placeholder="Country" autocomplete="country-name">
   <textarea name="notes" rows="2" placeholder="Notes (gift message, delivery instructions…)"></textarea>
   <select name="via"><option value="wa">Send my order via WhatsApp</option><option value="mail">Send my order via Email</option></select>
  </form>`;
  foot.innerHTML=`<div class="tot"><span>Total</span><b>${fmt(total())}</b></div><button class="btn" id="place" style="border:0">Place order</button>`;
  $("bk").onclick=()=>{step="cart";renderCart()};
  $("place").onclick=()=>{const f=$("f");if(!f.reportValidity())return;placeOrder(Object.fromEntries(new FormData(f)))};
  return;
 }
 $("dTitle").textContent="Your cart";
 if(!cart.length){body.innerHTML=`<p style="color:var(--muted);margin-top:30px;text-align:center">Your cart is empty.</p>`;foot.innerHTML=`<button class="btn" id="cont">Browse perfumes</button>`;$("cont").onclick=()=>{closeCart();location.hash="#shop"};return}
 body.innerHTML=cart.map(i=>{const p=P.find(x=>x.id===i.id);return `<div class="item"><div class="mini">${bottle(p.c,34,"c"+i.k)}</div>
  <div><h4>${p.n}</h4><small>${i.ml} ml · ${fmt(price(p,i.ml))}</small><br><span class="qty"><button data-d="-1" data-k="${i.k}">−</button>${i.q}<button data-d="1" data-k="${i.k}">+</button></span></div>
  <div><b>${fmt(price(p,i.ml)*i.q)}</b><button class="rm" data-rm="${i.k}">Remove</button></div></div>`}).join("");
 const t=total(),left=FREE_SHIPPING_OVER-t;
 foot.innerHTML=`<div class="note-free">${left>0?`Add ${fmt(left)} more for free shipping`:"🎉 You qualify for free shipping"}</div><div class="tot"><span>Subtotal</span><b>${fmt(t)}</b></div><button class="btn" id="go" style="border:0">Checkout</button>`;
 $("go").onclick=()=>{step="checkout";renderCart()};
}
$("dBody").onclick=e=>{
 const d=e.target.dataset;
 if(d.d){const it=cart.find(i=>i.k===d.k);it.q+=+d.d;if(it.q<1)cart=cart.filter(i=>i.k!==d.k)}
 else if(d.rm){cart=cart.filter(i=>i.k!==d.rm)}else return;
 saveCart();updateCount();renderCart();
};

function placeOrder(d){
 const lines=cart.map(i=>{const p=P.find(x=>x.id===i.id);return `• ${i.q} × ${p.n} (${i.ml} ml) — ${fmt(price(p,i.ml)*i.q)}`});
 const msg=`NEW ORDER — Genaro, Tomás T Gian\n\n${lines.join("\n")}\n\nTotal: ${fmt(total())}${total()>=FREE_SHIPPING_OVER?" (free shipping)":""}\n\nCustomer: ${d.name}\nEmail: ${d.email}\nPhone: ${d.phone}\nAddress: ${d.addr}, ${d.city}, ${d.zip}, ${d.country}\nNotes: ${d.notes||"-"}`;
 const url=d.via==="mail"
  ?`mailto:${STORE_EMAIL}?subject=${encodeURIComponent("New order — "+d.name)}&body=${encodeURIComponent(msg)}`
  :`https://wa.me/${WHATSAPP_NUMBER}?text=${encodeURIComponent(msg)}`;
 window.open(url,"_blank");
 cart=[];saveCart();updateCount();step="done";renderCart();
}

function toast(m){const t=$("toast");t.textContent=m;t.classList.add("on");clearTimeout(toast.t);toast.t=setTimeout(()=>t.classList.remove("on"),1800)}

$("waLink").href="https://wa.me/"+WHATSAPP_NUMBER;
$("mailLink").href="mailto:"+STORE_EMAIL;
render();updateCount();
</script>
</body>
</html>