<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<meta name="theme-color" content="#faf8f2">
<title>Cari Kata — Buku Tulis</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Patrick+Hand&family=Caveat:wght@600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --paper:#fbf9f3;
    --paper-deep:#f3efe4;
    --line:#b9c6de;
    --margin-red:#e2574b;
    --pencil:#3b3b3f;
    --pencil-soft:#6b6b70;
    --sun:#f6c945;
    --sun-soft:#fdeeb8;
    --found:#e9f4e4;
    --cell: 34px;
  }
  *{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent}
  html,body{height:100%}
  body{
    font-family:'Patrick Hand','Segoe Print','Comic Sans MS',cursive;
    background:var(--paper-deep);
    color:var(--pencil);
    display:flex;flex-direction:column;align-items:center;
    min-height:100dvh;
    padding:12px 10px 28px;
    background-image:radial-gradient(circle at 20% 10%, #fffdf6 0, transparent 55%);
    user-select:none;-webkit-user-select:none;
  }

  /* ---------- Header ---------- */
  header{width:100%;max-width:520px;text-align:center;margin-bottom:8px}
  h1{
    font-family:'Caveat',cursive;font-weight:700;
    font-size:clamp(34px,9vw,44px);line-height:1;
    letter-spacing:.5px;
  }
  h1 .under{position:relative;display:inline-block}
  h1 .under::after{
    content:"";position:absolute;left:-4px;right:-6px;bottom:2px;height:9px;
    background:var(--sun);opacity:.55;border-radius:6px;transform:rotate(-1.2deg);z-index:-1;
  }
  .sub{font-size:16px;color:var(--pencil-soft);margin-top:2px}

  /* ---------- Toolbar ---------- */
  .bar{
    width:100%;max-width:520px;display:flex;gap:8px;align-items:center;justify-content:center;
    flex-wrap:wrap;margin:6px 0 12px;
  }
  .chip{
    font-family:inherit;font-size:16px;color:var(--pencil);
    background:var(--paper);border:2px solid var(--pencil);
    border-radius:14px 16px 15px 13px/15px 13px 16px 14px; /* wobbly hand-drawn */
    padding:5px 14px;cursor:pointer;line-height:1.2;
    box-shadow:2px 2px 0 rgba(59,59,63,.18);
    transition:transform .08s;
  }
  .chip:active{transform:translate(1px,1px);box-shadow:0 0 0 rgba(0,0,0,0)}
  .chip.on{background:var(--sun);border-color:var(--pencil)}
  .chip.action{background:var(--margin-red);color:#fff;border-color:#b23c33}
  .timer{font-size:18px;min-width:64px;text-align:center;color:var(--pencil-soft)}

  /* ---------- Grid card ---------- */
  .board-wrap{
    position:relative;background:var(--paper);
    border:1.5px solid #d8d2c0;border-radius:6px;
    box-shadow:0 6px 18px rgba(90,80,50,.14), 0 1.5px 0 #e3ddca inset;
    padding:10px;
  }
  .grid{
    position:relative;display:grid;touch-action:none;
    grid-template-columns:repeat(var(--n),var(--cell));
    grid-template-rows:repeat(var(--n),var(--cell));
  }
  .cell{
    width:var(--cell);height:var(--cell);
    display:flex;align-items:center;justify-content:center;
    font-size:calc(var(--cell)*.58);
    border:1px solid #d9d4c4;
    color:var(--pencil);
    position:relative;z-index:2;
    border-radius:2px;
  }
  .cell.sel{background:var(--sun-soft)}
  .cell.done{color:var(--pencil)}
  svg.rings{
    position:absolute;inset:10px;z-index:3;pointer-events:none;
    width:calc(100% - 20px);height:calc(100% - 20px);
  }
  .ring{
    fill:none;stroke:var(--pencil);stroke-width:5;stroke-linecap:round;
    opacity:.85;
    stroke-dasharray:2000;stroke-dashoffset:2000;
    animation:draw .5s ease-out forwards;
  }
  @keyframes draw{to{stroke-dashoffset:0}}

  /* ---------- Word list: notebook page ---------- */
  .page{
    width:100%;max-width:520px;margin-top:16px;
    background:
      linear-gradient(90deg, transparent 44px, var(--margin-red) 44px, var(--margin-red) 46px, transparent 46px),
      repeating-linear-gradient(var(--paper), var(--paper) 35px, var(--line) 35px, var(--line) 36.5px);
    border:1.5px solid #d8d2c0;border-radius:6px;
    box-shadow:0 6px 18px rgba(90,80,50,.12);
    padding:10px 14px 16px 0;
  }
  .page h2{
    font-family:'Caveat',cursive;font-size:26px;font-weight:600;
    padding-left:58px;height:36px;display:flex;align-items:flex-end;
  }
  .words{list-style:none;columns:2;column-gap:0;padding-top:1px}
  @media (max-width:380px){ .words{columns:1} }
  .words li{
    height:36px;display:flex;align-items:center;gap:9px;
    padding-left:14px;break-inside:avoid;
    font-size:19px;letter-spacing:1.5px;
  }
  .box{
    width:21px;height:15px;flex:none;
    border:2px solid var(--margin-red);
    border-radius:6px 7px 6px 7px/7px 6px 7px 6px;
    position:relative;background:transparent;
  }
  li.hit .box::after{
    content:"✓";position:absolute;left:2px;top:-11px;
    font-size:22px;color:var(--pencil);
    font-family:'Caveat',cursive;font-weight:700;
  }
  li.hit .w{
    color:var(--pencil-soft);
    text-decoration:line-through;
    text-decoration-thickness:2px;
    text-decoration-color:rgba(59,59,63,.6);
  }

  /* ---------- Win overlay ---------- */
  .win{
    position:fixed;inset:0;background:rgba(40,35,20,.45);
    display:none;align-items:center;justify-content:center;z-index:50;padding:20px;
  }
  .win.show{display:flex}
  .win-card{
    background:var(--paper);border:2px solid var(--pencil);
    border-radius:18px 22px 20px 16px/20px 16px 22px 18px;
    box-shadow:4px 4px 0 rgba(59,59,63,.25);
    padding:26px 28px;text-align:center;max-width:320px;width:100%;
    animation:pop .35s cubic-bezier(.2,1.5,.4,1);
  }
  @keyframes pop{from{transform:scale(.7);opacity:0}}
  .win-card .big{font-family:'Caveat',cursive;font-size:42px;font-weight:700;line-height:1.1}
  .win-card p{font-size:18px;color:var(--pencil-soft);margin:8px 0 16px}
  .stars{font-size:30px;letter-spacing:4px;margin-bottom:4px}
</style>
</head>
<body>

<header>
  <h1><span class="under">Cari Kata</span> ✏️</h1>
  <div class="sub">Geser hurufnya, lingkari katanya!</div>
</header>

<div class="bar">
  <button class="chip on" data-lv="0">Mudah</button>
  <button class="chip" data-lv="1">Sedang</button>
  <button class="chip" data-lv="2">Sulit</button>
  <button class="chip action" id="btnNew">Acak Ulang 🔄</button>
  <div class="timer" id="timer">0:00</div>
</div>

<div class="board-wrap">
  <div class="grid" id="grid"></div>
  <svg class="rings" id="rings"></svg>
</div>

<div class="page">
  <h2 id="pageTitle">Temukan kata-kata ini:</h2>
  <ul class="words" id="wordList"></ul>
</div>

<div class="win" id="win">
  <div class="win-card">
    <div class="stars" id="stars">⭐⭐⭐</div>
    <div class="big">Hebat! 🎉</div>
    <p id="winText">Semua kata ketemu!</p>
    <button class="chip action" id="btnAgain">Main Lagi</button>
  </div>
</div>

<script>
(function(){
  // ====== Bank kata (dari buku tulis) ======
  const BANK = [
    // — dari buku tulis (asli) —
    "BUKU","PENSIL","PULPEN","PENGGARIS","BACA",
    "KOMPOR","SAUS","KECAP","GULA","TERIGU","MINYAK",
    "NASI","IKAN","AYAM","SEPATU","SENDAL",
    "ZUBAIR","SHAFIYYAH","UMI","ABI","KAKAK","ADIK","AYAH","IBU","CINTA",
    // — hewan —
    "KUCING","ANJING","KELINCI","BURUNG","GAJAH","HARIMAU","MONYET",
    "KUDA","SAPI","KAMBING","BEBEK","SEMUT","ULAR","SINGA","JERAPAH","BUAYA",
    // — buah —
    "APEL","JERUK","MANGGA","PISANG","ANGGUR","SEMANGKA","PEPAYA",
    "DURIAN","RAMBUTAN","NANAS","SALAK","JAMBU","MELON","STROBERI",
    // — sayur & makanan —
    "WORTEL","BAYAM","TOMAT","KENTANG","BAWANG","CABAI","TAHU","TEMPE",
    "TELUR","ROTI","SUSU","MADU","GARAM","SAMBAL","BAKSO","SOTO","SATE",
    // — warna —
    "MERAH","BIRU","HIJAU","KUNING","UNGU","PUTIH","HITAM","COKLAT","JINGGA",
    // — tubuh —
    "MATA","HIDUNG","TELINGA","MULUT","TANGAN","KAKI","RAMBUT","GIGI","JARI",
    // — alam —
    "MATAHARI","BULAN","BINTANG","LANGIT","HUJAN","AWAN","GUNUNG",
    "PANTAI","LAUT","SUNGAI","POHON","BUNGA","DAUN","ANGIN","PELANGI",
    // — sekolah —
    "SEKOLAH","GURU","MURID","KELAS","TAS","MEJA","KURSI",
    "KERTAS","KRAYON","SPIDOL","PENGHAPUS",
    // — rumah —
    "RUMAH","PINTU","JENDELA","KASUR","BANTAL","LEMARI","LAMPU","SAPU","MASJID",
    // — kendaraan & mainan —
    "MOBIL","MOTOR","SEPEDA","KERETA","PESAWAT","KAPAL","BECAK","DELMAN",
    "BOLA","LAYANGAN","BONEKA","ROBOT"
  ];
  const ALPHA = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

  // level: [ukuran grid, jumlah kata, arah]
  const LEVELS = [
    { n:10, count:6,  dirs:[[1,0],[0,1]] },                                   // mudah: → ↓
    { n:12, count:9,  dirs:[[1,0],[0,1],[1,1]] },                             // sedang: + diagonal
    { n:14, count:12, dirs:[[1,0],[0,1],[1,1],[-1,0],[0,-1],[-1,-1],[1,-1],[-1,1]] } // sulit: + terbalik
  ];

  let level = 0, N = 10, grid = [], placed = [], found = new Set();
  let startCell = null, selCells = [], timerId = null, seconds = 0, running = false;

  const $grid = document.getElementById('grid');
  const $rings = document.getElementById('rings');
  const $list  = document.getElementById('wordList');
  const $timer = document.getElementById('timer');
  const $win   = document.getElementById('win');

  // ====== Util ======
  const rnd = m => Math.floor(Math.random()*m);
  const shuffle = a => { for(let i=a.length-1;i>0;i--){const j=rnd(i+1);[a[i],a[j]]=[a[j],a[i]];} return a; };
  const fmt = s => Math.floor(s/60) + ":" + String(s%60).padStart(2,'0');

  // ====== Susun grid ======
  function build(){
    const cfg = LEVELS[level];
    N = cfg.n;
    // pilih kata yang muat di grid
    const pool = shuffle(BANK.filter(w => w.length <= N).slice());
    const words = pool.slice(0, cfg.count);

    for(let attempt=0; attempt<40; attempt++){
      grid = Array.from({length:N}, () => Array(N).fill(null));
      placed = [];
      let ok = true;
      for(const w of words.slice().sort((a,b)=>b.length-a.length)){
        if(!placeWord(w, cfg.dirs)){ ok = false; break; }
      }
      if(ok) break;
    }
    // isi sisa dengan huruf acak
    for(let r=0;r<N;r++) for(let c=0;c<N;c++) if(!grid[r][c]) grid[r][c]=ALPHA[rnd(26)];

    found = new Set();
    render(words);
    resetTimer();
  }

  function placeWord(w, dirs){
    for(let t=0;t<250;t++){
      const [dc,dr] = dirs[rnd(dirs.length)];
      const L = w.length;
      const rMin = dr<0 ? L-1 : 0, rMax = dr>0 ? N-L : N-1;
      const cMin = dc<0 ? L-1 : 0, cMax = dc>0 ? N-L : N-1;
      if(rMax<rMin || cMax<cMin) continue;
      const r0 = rMin + rnd(rMax-rMin+1), c0 = cMin + rnd(cMax-cMin+1);
      let fits = true;
      for(let i=0;i<L;i++){
        const ch = grid[r0+dr*i][c0+dc*i];
        if(ch && ch !== w[i]){ fits=false; break; }
      }
      if(!fits) continue;
      for(let i=0;i<L;i++) grid[r0+dr*i][c0+dc*i] = w[i];
      placed.push({ w, r0, c0, dr, dc });
      return true;
    }
    return false;
  }

  // ====== Render ======
  function render(words){
    // ukuran sel responsif
    const avail = Math.min(window.innerWidth - 44, 520);
    const cell = Math.max(24, Math.min(40, Math.floor(avail / N)));
    document.documentElement.style.setProperty('--cell', cell + 'px');
    document.documentElement.style.setProperty('--n', N);

    $grid.innerHTML = '';
    for(let r=0;r<N;r++) for(let c=0;c<N;c++){
      const d = document.createElement('div');
      d.className = 'cell';
      d.textContent = grid[r][c];
      d.dataset.r = r; d.dataset.c = c;
      $grid.appendChild(d);
    }
    $rings.setAttribute('viewBox', `0 0 ${N*100} ${N*100}`);
    $rings.innerHTML = '';

    $list.innerHTML = '';
    for(const w of words){
      const li = document.createElement('li');
      li.dataset.w = w;
      li.innerHTML = `<span class="box"></span><span class="w">${w}</span>`;
      $list.appendChild(li);
    }
  }

  // ====== Seleksi (sentuh & mouse) ======
  function cellAt(x,y){
    const rect = $grid.getBoundingClientRect();
    const size = rect.width / N;
    const c = Math.floor((x-rect.left)/size), r = Math.floor((y-rect.top)/size);
    return (r>=0 && r<N && c>=0 && c<N) ? {r,c} : null;
  }

  function lineCells(a,b){
    let dr = b.r-a.r, dc = b.c-a.c;
    // patenkan ke arah lurus/diagonal terdekat
    if(dr!==0 && dc!==0 && Math.abs(dr)!==Math.abs(dc)){
      if(Math.abs(dr) > Math.abs(dc)) dc = 0; else dr = 0;
    }
    const L = Math.max(Math.abs(dr),Math.abs(dc));
    const sr = Math.sign(dr), sc = Math.sign(dc);
    const cells = [];
    for(let i=0;i<=L;i++){
      const r=a.r+sr*i, c=a.c+sc*i;
      if(r<0||r>=N||c<0||c>=N) break;
      cells.push({r,c});
    }
    return cells;
  }

  function paint(cells){
    $grid.querySelectorAll('.cell.sel').forEach(e=>e.classList.remove('sel'));
    for(const {r,c} of cells){
      $grid.children[r*N+c].classList.add('sel');
    }
  }

  $grid.addEventListener('pointerdown', e=>{
    const cl = cellAt(e.clientX,e.clientY);
    if(!cl) return;
    startTimer();
    startCell = cl; selCells = [cl]; paint(selCells);
    $grid.setPointerCapture(e.pointerId);
  });
  $grid.addEventListener('pointermove', e=>{
    if(!startCell) return;
    const cl = cellAt(e.clientX,e.clientY);
    if(!cl) return;
    selCells = lineCells(startCell, cl);
    paint(selCells);
  });
  $grid.addEventListener('pointerup', ()=>{
    if(!startCell) return;
    check(selCells);
    startCell = null; selCells = [];
    $grid.querySelectorAll('.cell.sel').forEach(e=>e.classList.remove('sel'));
  });

  // ====== Cek jawaban ======
  function check(cells){
    if(cells.length < 2) return;
    const s  = cells.map(({r,c})=>grid[r][c]).join('');
    const sr = s.split('').reverse().join('');
    const li = [...$list.children].find(li =>
      !li.classList.contains('hit') && (li.dataset.w===s || li.dataset.w===sr)
    );
    if(!li) return;
    li.classList.add('hit');
    found.add(li.dataset.w);
    drawRing(cells[0], cells[cells.length-1]);
    if(navigator.vibrate) navigator.vibrate(35);
    if(found.size === $list.children.length) winGame();
  }

  // lingkaran pensil ala kertas
  function drawRing(a,b){
    const x1=a.c*100+50, y1=a.r*100+50, x2=b.c*100+50, y2=b.r*100+50;
    const mx=(x1+x2)/2, my=(y1+y2)/2;
    const len=Math.hypot(x2-x1,y2-y1)+92;
    const ang=Math.atan2(y2-y1,x2-x1)*180/Math.PI;
    const wob=()=> (Math.random()*8-4).toFixed(1);
    const rect=document.createElementNS('http://www.w3.org/2000/svg','rect');
    rect.setAttribute('x', mx-len/2);
    rect.setAttribute('y', my-46);
    rect.setAttribute('width', len);
    rect.setAttribute('height', 92);
    rect.setAttribute('rx', 46);
    rect.setAttribute('class','ring');
    rect.setAttribute('transform',`rotate(${(ang+ +wob()/3).toFixed(2)} ${mx} ${my})`);
    $rings.appendChild(rect);
  }

  // ====== Timer & menang ======
  function startTimer(){
    if(running) return;
    running = true;
    timerId = setInterval(()=>{ seconds++; $timer.textContent = fmt(seconds); }, 1000);
  }
  function resetTimer(){
    clearInterval(timerId); running=false; seconds=0; $timer.textContent="0:00";
  }
  function winGame(){
    clearInterval(timerId); running=false;
    const t = seconds;
    const stars = t<60 ? "⭐⭐⭐" : t<150 ? "⭐⭐" : "⭐";
    document.getElementById('stars').textContent = stars;
    document.getElementById('winText').textContent =
      `Semua kata ketemu dalam ${fmt(t)}!`;
    setTimeout(()=>$win.classList.add('show'), 400);
  }

  // ====== Kontrol ======
  document.querySelectorAll('.chip[data-lv]').forEach(btn=>{
    btn.addEventListener('click', ()=>{
      document.querySelectorAll('.chip[data-lv]').forEach(b=>b.classList.remove('on'));
      btn.classList.add('on');
      level = +btn.dataset.lv;
      build();
    });
  });
  document.getElementById('btnNew').addEventListener('click', build);
  document.getElementById('btnAgain').addEventListener('click', ()=>{
    $win.classList.remove('show'); build();
  });
  window.addEventListener('resize', ()=>{ /* jaga ukuran sel */ 
    const avail = Math.min(window.innerWidth - 44, 520);
    const cell = Math.max(24, Math.min(40, Math.floor(avail / N)));
    document.documentElement.style.setProperty('--cell', cell + 'px');
  });

  build();
})();
</script>
</body>
</html>