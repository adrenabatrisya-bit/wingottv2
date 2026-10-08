<!DOCTYPE html>
<html lang="ms">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Wingo Trend Tracker</title>
<style>
  *{box-sizing:border-box;}
  body{margin:0;background:#f7f7f9;}
  #app{font-family:system-ui,-apple-system,"Segoe UI",sans-serif;max-width:760px;margin:0 auto;padding:14px;color:#1a1a1a;}
  header{display:flex;justify-content:space-between;align-items:center;gap:10px;flex-wrap:wrap;margin-bottom:12px;}
  .brand{display:flex;align-items:center;gap:10px;}
  .logo{font-size:30px;} h1{margin:0;font-size:19px;} .tag{font-size:12px;color:#999;}
  .hbtns{display:flex;gap:6px;flex-wrap:wrap;}
  .modes{display:flex;gap:8px;margin-bottom:12px;}
  .mode{flex:1;background:#fff;color:#666;border:2px solid #ececec;padding:12px;border-radius:12px;font-weight:700;font-size:14px;cursor:pointer;}
  .mode.active{background:#e74c3c;color:#fff;border-color:#e74c3c;}
  .card,.inputCard,.pred,.stat{background:#fff;border:1px solid #ececec;border-radius:14px;padding:14px;box-shadow:0 1px 3px rgba(0,0,0,.04);}
  .inputCard,.grid,.pred,.card{margin-bottom:12px;}
  .sub{font-size:13px;color:#888;margin-bottom:10px;}
  .inputRow{display:flex;gap:8px;flex-wrap:wrap;}
  input{flex:1;min-width:110px;padding:12px;border:2px solid #ececec;border-radius:10px;font-size:16px;outline:none;}
  input:focus{border-color:#e74c3c;}
  button{background:#e74c3c;color:#fff;border:none;padding:11px 16px;border-radius:10px;font-size:14px;font-weight:600;cursor:pointer;transition:.15s;}
  button:hover{background:#c0392b;}
  button.ghost{background:#f2f2f4;color:#555;} button.ghost:hover{background:#e6e6e9;}
  button.danger{background:#f2f2f4;color:#c0392b;} button.danger:hover{background:#fde8e6;}
  .quick{display:flex;gap:6px;flex-wrap:wrap;margin-top:10px;}
  .qb{width:40px;height:40px;border-radius:10px;border:2px solid #ececec;background:#fff;font-weight:700;font-size:16px;cursor:pointer;padding:0;}
  .qb:hover{border-color:#e74c3c;background:#fff5f3;} .qb.b{color:#27ae60;} .qb.s{color:#e74c3c;}
  .grid{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;}
  .stat{text-align:center;padding:12px 6px;}
  .lbl{font-size:11px;color:#999;text-transform:uppercase;letter-spacing:.5px;margin-bottom:5px;}
  .val{font-size:22px;font-weight:700;} .val.green{color:#27ae60;} .val.red{color:#e74c3c;}
  .pred{background:linear-gradient(135deg,#fff8f0,#fff);border:2px solid #e74c3c;}
  .patName{font-size:20px;font-weight:800;margin:2px 0 4px;}
  .patDesc{font-size:13px;color:#777;line-height:1.5;margin-bottom:10px;}
  .confWrap{height:9px;background:#f0f0f0;border-radius:6px;overflow:hidden;margin-bottom:4px;}
  .confBar{height:100%;width:0;border-radius:6px;transition:.3s;background:#e74c3c;}
  .confTxt{font-size:12px;color:#999;margin-bottom:8px;}
  .predVal{font-size:34px;font-weight:800;letter-spacing:2px;margin:6px 0 4px;}
  .numBox{display:flex;gap:20px;margin-top:12px;padding-top:12px;border-top:1px dashed #e5e5e5;}
  .nbCol{flex:1;} .nbLbl{font-size:12px;color:#888;margin-bottom:7px;font-weight:600;}
  .nbChips{display:flex;flex-wrap:wrap;gap:7px;}
  .nc{width:38px;height:38px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-weight:700;font-size:16px;}
  .nc.sug{background:#27ae60;color:#fff;} .nc.avoid{background:#f2f2f4;color:#999;border:2px solid #e2e2e2;}
  .history{display:flex;flex-wrap:wrap;gap:6px;margin-top:8px;max-height:260px;overflow-y:auto;}
  .chip{width:40px;height:40px;border-radius:11px;display:flex;align-items:center;justify-content:center;font-weight:700;font-size:17px;color:#fff;}
  .chip.b{background:#27ae60;} .chip.s{background:#e74c3c;} .chip.first{outline:3px solid #f39c12;outline-offset:2px;}
  .freq{display:flex;gap:5px;margin-top:10px;align-items:flex-end;height:90px;}
  .fbar{flex:1;display:flex;flex-direction:column;justify-content:flex-end;align-items:center;gap:3px;}
  .fbar .bar{width:100%;border-radius:5px 5px 0 0;background:#e74c3c;min-height:3px;}
  .fbar .n{font-size:11px;color:#999;} .fbar .c{font-size:11px;font-weight:700;color:#555;}
  .empty{color:#bbb;font-size:13px;padding:8px 0;}
  footer{text-align:center;font-size:12px;color:#aaa;padding:10px;}
  @media(max-width:520px){.grid{grid-template-columns:repeat(2,1fr);}}
</style>
</head>
<body>
<div id="app">
  <header>
    <div class="brand"><span class="logo">🎯</span>
      <div><h1>Wingo Trend Tracker</h1><div class="tag">Pattern AI • Naga • Silang • Double Jump</div></div>
    </div>
    <div class="hbtns">
      <button class="ghost" id="exportBtn">⬇ Export</button>
      <button class="ghost" id="importBtn">⬆ Import</button>
      <button class="ghost danger" id="resetBtn">Reset</button>
    </div>
  </header>

  <div class="modes">
    <button class="mode active" data-mode="s30">⏱️ Win Go 30s</button>
    <button class="mode" data-mode="m1">⏱️ Win Go 1 Min</button>
  </div>

  <section class="inputCard">
    <div class="sub">Taip nombor result (0–9) → Enter. Paling baru di atas.</div>
    <div class="inputRow">
      <input id="numInput" type="number" min="0" max="9" placeholder="Nombor 0–9" autofocus />
      <button id="addBtn">Tambah</button>
      <button id="undoBtn" class="ghost">↶ Undo</button>
    </div>
    <div class="quick" id="quickRow"></div>
  </section>

  <section class="grid">
    <div class="stat"><div class="lbl">Total</div><div class="val" id="total">0</div></div>
    <div class="stat"><div class="lbl">Big</div><div class="val green" id="bigC">0</div></div>
    <div class="stat"><div class="lbl">Small</div><div class="val red" id="smallC">0</div></div>
    <div class="stat"><div class="lbl">Streak</div><div class="val" id="streak">—</div></div>
  </section>

  <section class="grid">
    <div class="stat"><div class="lbl">🔥 Panas</div><div class="val" id="hot">—</div></div>
    <div class="stat"><div class="lbl">❄️ Sejuk</div><div class="val" id="cold">—</div></div>
    <div class="stat"><div class="lbl">Imbangan</div><div class="val" id="balance">—</div></div>
    <div class="stat"><div class="lbl">Corak</div><div class="val" id="patShort">—</div></div>
  </section>

  <section class="pred">
    <div class="lbl">🧬 Corak Dikesan</div>
    <div class="patName" id="patName">—</div>
    <div class="patDesc" id="patDesc">Tambah sekurang-kurangnya 5 result.</div>
    <div class="confWrap"><div class="confBar" id="confBar"></div></div>
    <div class="confTxt" id="confTxt"></div>
    <div class="predVal" id="predVal">—</div>
    <div id="numBox" class="numBox" style="display:none;">
      <div class="nbCol"><div class="nbLbl">✅ Disyorkan</div><div class="nbChips" id="sugNums"></div></div>
      <div class="nbCol"><div class="nbLbl">⚠️ Elak</div><div class="nbChips" id="avoidNums"></div></div>
    </div>
  </section>

  <section class="card"><div class="lbl">Sejarah (baru → lama)</div><div id="history" class="history"></div></section>
  <section class="card"><div class="lbl">📊 Kekerapan Nombor</div><div id="freq" class="freq"></div></section>
  <footer>⚠️ Bukan jaminan. Alat disiplin & rujukan sahaja.</footer>
</div>
<input type="file" id="fileIn" accept=".json" style="display:none">

<script>
const KEY='wingo_app_v4';
let store=JSON.parse(localStorage.getItem(KEY)||'{"s30":[],"m1":[]}');
if(!store.s30)store.s30=[]; if(!store.m1)store.m1=[];
let mode='s30';
const save=()=>localStorage.setItem(KEY,JSON.stringify(store));
const get=()=>store[mode];
const type=n=>n>=5?'B':'S';
const opp=x=>x==='B'?'S':'B';
const $=id=>document.getElementById(id);

document.querySelectorAll('.mode').forEach(b=>b.onclick=()=>{
  mode=b.dataset.mode;
  document.querySelectorAll('.mode').forEach(x=>x.classList.toggle('active',x===b));
  render();
});

function detect(seq){
  const n=seq.length;
  if(n<3) return {name:'📊 Awal', next:seq[n-1]||'B', conf:50, desc:'Data belum cukup.'};
  const runs=[]; let c=seq[0],l=1;
  for(let i=1;i<n;i++){ if(seq[i]===c)l++; else{runs.push(l);c=seq[i];l=1;} }
  runs.push(l);
  const last=seq[n-1], o=opp(last);
  const lastLen=runs[runs.length-1];
  const prevLen=runs.length>=2?runs[runs.length-2]:0;
  const prev2=runs.length>=3?runs[runs.length-3]:0;

  if(lastLen>=5) return {name:'🐉 Naga Panjang ('+lastLen+')', next:last, conf:80, desc:'Streak sangat panjang — ikut arah sehingga pecah.'};
  if(lastLen===4) return {name:'🐉 Naga ('+lastLen+')', next:last, conf:70, desc:'Streak panjang — biasanya sambung.'};
  if(lastLen===3) return {name:'🐉 Streak 3', next:o, conf:60, desc:'Streak 3 — kerap pecah selepas ni.'};

  let alt=1; for(let i=n-1;i>=1 && seq[i]!==seq[i-1];i--) alt++;
  if(alt>=5) return {name:'✂️ Silang (Single Jump)', next:o, conf:74, desc:'Berselang-seli lama — lawan arah terakhir.'};
  if(alt>=3) return {name:'✂️ Silang', next:o, conf:63, desc:'Corak selang-seli dikesan.'};

  if(lastLen===2 && prevLen===2) return {name:'🔁 Double Jump (2-2)', next:o, conf:70, desc:'Pasangan lengkap — tukar arah.'};
  if(lastLen===1 && prevLen===2 && prev2===2) return {name:'🔁 Double Jump (2-2)', next:last, conf:68, desc:'Lengkapkan pasangan yang baru mula.'};

  if(lastLen===3 && prevLen===3) return {name:'🔂 Triple Jump (3-3)', next:o, conf:66, desc:'Corak 3-3 — tukar selepas blok.'};
  if(lastLen<=1 && prevLen===3 && prev2===3) return {name:'🔂 Triple Jump (3-3)', next:last, conf:64, desc:'Sambung blok 3.'};

  if(runs.length>=4 && prev2===1 && prevLen===2 && lastLen===1) return {name:'↔️ Jump 1-2', next:last, conf:60, desc:'Corak 1-2 berulang.'};
  if(runs.length>=4 && prev2===2 && prevLen===1 && lastLen===2) return {name:'↔️ Jump 2-1', next:o, conf:60, desc:'Corak 2-1 berulang.'};

  if(lastLen===2) return {name:'📊 Double', next:o, conf:56, desc:'Double tanpa corak jelas — cadangan lawan.'};
  return {name:'📊 Neutral', next:o, conf:50, desc:'Tiada corak kuat. Ikut gerak hati / money management.'};
}

function render(){
  const data=get(), t=data.length;
  $('total').textContent=t;
  const b=data.filter(n=>type(n)==='B').length, s=t-b;
  $('bigC').textContent=b;
  $('smallC').textContent=s;

  let st='—';
  if(t>0){const x=type(data[0]);let c=1;for(let i=1;i<t;i++){if(type(data[i])===x)c++;else break;}st=(x==='B'?'Big':'Small')+' x'+c;}
  $('streak').textContent=st;

  const cnt=Array(10).fill(0); data.forEach(n=>cnt[n]++);
  const hot=[...cnt.keys()].sort((a,b)=>cnt[b]-cnt[a]).slice(0,3).filter(n=>cnt[n]>0);
  const cold=[...cnt.keys()].sort((a,b)=>cnt[a]-cnt[b]).slice(0,3);
  $('hot').textContent=hot.length?hot.join(' '):'—';
  $('cold').textContent=cold.join(' ');
  $('balance').textContent=b===s?'SEIMBANG':(b>s?'Big +'+(b-s):'Small +'+(s-b));

  const h=$('history');h.innerHTML='';
  if(t===0){h.innerHTML='<div class="empty">Belum ada result. Tambah nombor di atas.</div>';}
  else data.slice(0,60).forEach((n,i)=>{const d=document.createElement('div');d.className='chip '+(type(n)==='B'?'b':'s')+(i===0?' first':'');d.textContent=n;h.appendChild(d);});

  const fr=$('freq');fr.innerHTML='';
  const mx=Math.max(1,...cnt);
  cnt.forEach((c,n)=>{const w=document.createElement('div');w.className='fbar';
    w.innerHTML='<div class="c">'+c+'</div><div class="bar" style="height:'+(c/mx*60)+'px;background:'+(type(n)==='B'?'#27ae60':'#e74c3c')+'"></div><div class="n">'+n+'</div>';
    fr.appendChild(w);});

  const pv=$('predVal'),pn=$('patName'),pd=$('patDesc');
  const cb=$('confBar'),ct=$('confTxt'),nb=$('numBox'),ps=$('patShort');
  const sg=$('sugNums'),av=$('avoidNums');

  if(t<5){pn.textContent='—';pd.textContent='Tambah sekurang-kurangnya 5 result untuk analisis corak.';ps.textContent='—';pv.textContent='—';pv.style.color='#999';cb.style.width='0';ct.textContent='';nb.style.display='none';return;}

  const seq=data.slice(0,14).map(type).reverse();
  const d=detect(seq);
  pn.textContent=d.name; pd.textContent=d.desc;
  ps.textContent=d.name.split(' ')[0];
  cb.style.width=d.conf+'%';
  cb.style.background=d.conf>=70?'#27ae60':(d.conf>=60?'#f39c12':'#e74c3c');
  ct.textContent='Keyakinan: '+d.conf+'%';

  pv.textContent=d.next==='B'?'BIG':'SMALL';
  pv.style.color=d.next==='B'?'#27ae60':'#e74c3c';

  const pool=d.next==='B'?[5,6,7,8,9]:[0,1,2,3,4], oPool=d.next==='B'?[0,1,2,3,4]:[5,6,7,8,9];
  nb.style.display='flex';sg.innerHTML='';av.innerHTML='';
  [...pool].sort((a,b)=>cnt[b]-cnt[a]).slice(0,3).forEach(n=>{const e=document.createElement('div');e.className='nc sug';e.textContent=n;sg.appendChild(e);});
  [...oPool].sort((a,b)=>cnt[a]-cnt[b]).slice(0,3).forEach(n=>{const e=document.createElement('div');e.className='nc avoid';e.textContent=n;av.appendChild(e);});
}

const qi=$('quickRow');
for(let n=0;n<=9;n++){const bt=document.createElement('button');bt.className='qb '+(type(n)==='B'?'b':'s');bt.textContent=n;bt.onclick=()=>add(n);qi.appendChild(bt);}

function add(v){get().unshift(v);save();render();}
$('addBtn').onclick=()=>{const v=parseInt($('numInput').value);if(isNaN(v)||v<0||v>9)return;add(v);$('numInput').value='';$('numInput').focus();};
$('numInput').addEventListener('keydown',e=>{if(e.key==='Enter')$('addBtn').click();});
$('undoBtn').onclick=()=>{get().shift();save();render();};
$('resetBtn').onclick=()=>{if(confirm('Reset data mod ini?')){store[mode]=[];save();render();}};
$('exportBtn').onclick=()=>{const blob=new Blob([JSON.stringify(store)],{type:'application/json'});const a=document.createElement('a');a.href=URL.createObjectURL(blob);a.download='wingo-history.json';a.click();};
$('importBtn').onclick=()=>$('fileIn').click();
$('fileIn').onchange=e=>{const f=e.target.files[0];if(!f)return;const r=new FileReader();r.onload=()=>{try{const j=JSON.parse(r.result);if(j&&typeof j==='object'){if(j.s30||j.m1){store=j;}else if(Array.isArray(j)){store[mode]=j;}save();render();}}catch(x){alert('Fail tak sah');}};r.readAsText(f);};
render();
</script>
</body>
</html>