<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Insulin Log</title>
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@500;600&display=swap" rel="stylesheet" />
<style>
  :root{
    --paper:#F4F6F8;
    --card:#FFFFFF;
    --ink:#16202B;
    --ink-soft:#5A6B7B;
    --line:#DDE3E9;
    --accent:#0E7C7B;
    --accent-dark:#0A5E5D;
    --rapid:#E8833A;
    --long:#2E74C4;
    --other:#7A8694;
    --danger:#C0392B;
    --radius:14px;
    --shadow:0 1px 2px rgba(22,32,43,.05), 0 8px 24px rgba(22,32,43,.06);
  }
  *{box-sizing:border-box;}
  html,body{margin:0;}
  body{
    background:var(--paper);
    color:var(--ink);
    font-family:"Inter",system-ui,sans-serif;
    line-height:1.5;
    -webkit-font-smoothing:antialiased;
    padding:0 16px 64px;
  }
  .wrap{max-width:680px;margin:0 auto;}

  /* Header */
  header{
    display:flex;align-items:baseline;justify-content:space-between;
    gap:12px;padding:28px 0 20px;flex-wrap:wrap;
  }
  .brand{display:flex;align-items:center;gap:12px;}
  .vial{
    width:26px;height:26px;flex:none;
    border:2px solid var(--ink);border-radius:5px 5px 7px 7px;
    position:relative;background:
      linear-gradient(to top, var(--accent) 0 42%, transparent 42%);
  }
  .vial::before{content:"";position:absolute;top:-6px;left:5px;right:5px;height:5px;background:var(--ink);border-radius:2px;}
  h1{
    font-family:"Space Grotesk",sans-serif;
    font-weight:600;font-size:1.4rem;letter-spacing:-.01em;margin:0;
  }
  .status{
    font-family:"IBM Plex Mono",monospace;font-size:.72rem;
    color:var(--ink-soft);display:flex;align-items:center;gap:7px;
  }
  .dot{width:8px;height:8px;border-radius:50%;background:var(--other);}
  .dot.on{background:var(--accent);}

  /* Banner */
  .banner{
    background:#FFF6E9;border:1px solid #F2D7A6;color:#7A5418;
    border-radius:var(--radius);padding:14px 16px;margin-bottom:20px;
    font-size:.9rem;display:none;
  }
  .banner code{font-family:"IBM Plex Mono",monospace;background:#0000000d;padding:1px 5px;border-radius:4px;}

  /* Summary */
  .summary{
    display:flex;gap:10px;margin-bottom:20px;flex-wrap:wrap;
  }
  .stat{
    flex:1;min-width:120px;background:var(--card);border:1px solid var(--line);
    border-radius:var(--radius);padding:14px 16px;
  }
  .stat .k{font-size:.72rem;text-transform:uppercase;letter-spacing:.06em;color:var(--ink-soft);}
  .stat .v{font-family:"IBM Plex Mono",monospace;font-weight:600;font-size:1.5rem;margin-top:2px;}
  .stat .v small{font-size:.8rem;color:var(--ink-soft);font-weight:500;}

  /* Card / form */
  .card{
    background:var(--card);border:1px solid var(--line);
    border-radius:var(--radius);box-shadow:var(--shadow);
    padding:20px;margin-bottom:24px;
  }
  .card h2{
    font-family:"Space Grotesk",sans-serif;font-size:.8rem;font-weight:600;
    text-transform:uppercase;letter-spacing:.08em;color:var(--ink-soft);
    margin:0 0 16px;
  }
  .grid{display:grid;grid-template-columns:1fr 1fr;gap:14px;}
  .field{display:flex;flex-direction:column;gap:6px;}
  .field.full{grid-column:1 / -1;}
  label{font-size:.78rem;font-weight:500;color:var(--ink-soft);}
  input,select{
    font-family:inherit;font-size:.95rem;color:var(--ink);
    background:var(--paper);border:1px solid var(--line);border-radius:9px;
    padding:10px 12px;width:100%;
  }
  input:focus,select:focus{outline:2px solid var(--accent);outline-offset:1px;border-color:var(--accent);}
  .units-input{font-family:"IBM Plex Mono",monospace;font-weight:600;}

  .seg{display:flex;gap:6px;}
  .seg button{
    flex:1;font-family:inherit;font-size:.82rem;font-weight:500;cursor:pointer;
    padding:9px 6px;border-radius:9px;border:1px solid var(--line);
    background:var(--paper);color:var(--ink-soft);
  }
  .seg button[aria-pressed="true"]{color:#fff;border-color:transparent;}
  .seg button.rapid[aria-pressed="true"]{background:var(--rapid);}
  .seg button.long[aria-pressed="true"]{background:var(--long);}
  .seg button.other[aria-pressed="true"]{background:var(--other);}

  .btn{
    font-family:"Space Grotesk",sans-serif;font-weight:600;font-size:.95rem;
    color:#fff;background:var(--accent);border:none;border-radius:10px;
    padding:13px 18px;cursor:pointer;width:100%;margin-top:4px;
    transition:background .15s ease;
  }
  .btn:hover{background:var(--accent-dark);}
  .btn:focus-visible{outline:2px solid var(--ink);outline-offset:2px;}
  .btn:disabled{opacity:.5;cursor:not-allowed;}

  /* Log */
  .daygroup{margin-bottom:22px;}
  .dayhead{
    font-family:"Space Grotesk",sans-serif;font-size:.76rem;font-weight:600;
    text-transform:uppercase;letter-spacing:.07em;color:var(--ink-soft);
    padding:0 4px 8px;display:flex;justify-content:space-between;
  }
  .entry{
    background:var(--card);border:1px solid var(--line);border-left:4px solid var(--other);
    border-radius:12px;padding:14px 16px;margin-bottom:8px;
    display:flex;align-items:center;gap:14px;
  }
  .entry.rapid{border-left-color:var(--rapid);}
  .entry.long{border-left-color:var(--long);}
  .readout{
    font-family:"IBM Plex Mono",monospace;font-weight:600;
    font-size:1.55rem;line-height:1;letter-spacing:-.02em;
    font-variant-numeric:tabular-nums;min-width:62px;text-align:right;
  }
  .readout small{font-size:.65rem;color:var(--ink-soft);margin-left:2px;}
  .meta{flex:1;min-width:0;}
  .meta .top{display:flex;align-items:center;gap:8px;flex-wrap:wrap;}
  .chip{
    font-size:.68rem;font-weight:600;padding:2px 8px;border-radius:999px;
    text-transform:uppercase;letter-spacing:.04em;color:#fff;background:var(--other);
  }
  .chip.rapid{background:var(--rapid);}
  .chip.long{background:var(--long);}
  .name{font-weight:600;font-size:.95rem;}
  .time{font-family:"IBM Plex Mono",monospace;font-size:.74rem;color:var(--ink-soft);}
  .sub{font-size:.82rem;color:var(--ink-soft);margin-top:3px;}
  .del{
    flex:none;border:none;background:none;cursor:pointer;color:var(--ink-soft);
    font-size:1.1rem;padding:6px;border-radius:8px;line-height:1;
  }
  .del:hover{color:var(--danger);background:#C0392B12;}

  .empty{
    text-align:center;color:var(--ink-soft);padding:40px 16px;font-size:.92rem;
  }
  footer{text-align:center;color:var(--ink-soft);font-size:.74rem;padding:8px 0;}

  @media (max-width:520px){
    .grid{grid-template-columns:1fr;}
    .readout{font-size:1.35rem;min-width:54px;}
  }
  @media (prefers-reduced-motion:reduce){*{transition:none!important;}}
</style>
</head>
<body>
<div class="wrap">

  <header>
    <div class="brand">
      <div class="vial" aria-hidden="true"></div>
      <h1>Insulin Log</h1>
    </div>
    <div class="status"><span class="dot" id="dot"></span><span id="statusText">connecting…</span></div>
  </header>

  <div class="banner" id="banner">
    Firebase not set up. Paste your project config into <code>firebaseConfig</code> in this file's script.
  </div>

  <div class="summary">
    <div class="stat"><div class="k">Today · total</div><div class="v" id="sumUnits">0<small> U</small></div></div>
    <div class="stat"><div class="k">Today · doses</div><div class="v" id="sumDoses">0</div></div>
  </div>

  <div class="card">
    <h2>Log a dose</h2>
    <div class="grid">
      <div class="field full">
        <label>Category</label>
        <div class="seg" id="seg">
          <button type="button" class="rapid" data-cat="rapid" aria-pressed="true">Rapid-acting</button>
          <button type="button" class="long" data-cat="long" aria-pressed="false">Long-acting</button>
          <button type="button" class="other" data-cat="other" aria-pressed="false">Other</button>
        </div>
      </div>
      <div class="field">
        <label for="units">Units (U)</label>
        <input class="units-input" id="units" type="number" step="0.5" min="0" inputmode="decimal" placeholder="0" />
      </div>
      <div class="field">
        <label for="when">Time</label>
        <input id="when" type="datetime-local" />
      </div>
      <div class="field">
        <label for="name">Insulin name <span style="font-weight:400">(optional)</span></label>
        <input id="name" type="text" placeholder="e.g. Humalog" autocomplete="off" />
      </div>
      <div class="field">
        <label for="glucose">Glucose <span style="font-weight:400">(optional)</span></label>
        <input id="glucose" type="number" step="0.1" min="0" inputmode="decimal" placeholder="reading" />
      </div>
      <div class="field full">
        <label for="note">Note <span style="font-weight:400">(optional)</span></label>
        <input id="note" type="text" placeholder="before lunch, correction…" autocomplete="off" />
      </div>
    </div>
    <button class="btn" id="save" disabled>Log dose</button>
  </div>

  <div id="log"><div class="empty">No doses logged yet.</div></div>

  <footer>Personal record only. Not medical advice.</footer>
</div>

<script type="module">
  import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-app.js";
  import { getAuth, signInAnonymously, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-auth.js";
  import {
    getFirestore, collection, addDoc, deleteDoc, doc,
    query, orderBy, onSnapshot, serverTimestamp, Timestamp
  } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-firestore.js";

  // ===== 1. PASTE YOUR FIREBASE CONFIG HERE =====
  const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_PROJECT.firebaseapp.com",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_PROJECT.appspot.com",
    messagingSenderId: "YOUR_SENDER_ID",
    appId: "YOUR_APP_ID"
  };
  // ==============================================

  const $ = (id) => document.getElementById(id);
  const dot = $("dot"), statusText = $("statusText");

  if (firebaseConfig.apiKey === "YOUR_API_KEY") {
    $("banner").style.display = "block";
    statusText.textContent = "no config";
  }

  let db, uid = null;
  let selectedCat = "rapid";

  // Category selector
  $("seg").addEventListener("click", (e) => {
    const b = e.target.closest("button[data-cat]");
    if (!b) return;
    selectedCat = b.dataset.cat;
    [...$("seg").children].forEach(x => x.setAttribute("aria-pressed", x === b));
  });

  // Default time = now (local)
  function nowLocal(){
    const d = new Date(); d.setMinutes(d.getMinutes() - d.getTimezoneOffset());
    return d.toISOString().slice(0,16);
  }
  $("when").value = nowLocal();

  // Init Firebase
  try {
    const app = initializeApp(firebaseConfig);
    db = getFirestore(app);
    const auth = getAuth(app);
    onAuthStateChanged(auth, (user) => {
      if (user) { uid = user.uid; ready(); }
    });
    signInAnonymously(auth).catch(err => {
      statusText.textContent = "auth error";
      console.error(err);
    });
  } catch (err) {
    console.error("Firebase init failed:", err);
  }

  function ready(){
    dot.classList.add("on");
    statusText.textContent = "synced · " + uid.slice(0,6);
    $("save").disabled = false;
    watch();
  }

  // Save dose
  $("save").addEventListener("click", async () => {
    const units = parseFloat($("units").value);
    if (!units || units <= 0) { $("units").focus(); return; }
    const whenVal = $("when").value;
    const taken = whenVal ? new Date(whenVal) : new Date();
    const glucose = $("glucose").value ? parseFloat($("glucose").value) : null;

    $("save").disabled = true;
    try {
      await addDoc(collection(db, "users", uid, "doses"), {
        category: selectedCat,
        name: $("name").value.trim() || null,
        units,
        glucose,
        note: $("note").value.trim() || null,
        taken: Timestamp.fromDate(taken),
        created: serverTimestamp()
      });
      $("units").value = ""; $("name").value = "";
      $("glucose").value = ""; $("note").value = "";
      $("when").value = nowLocal();
    } catch (err) {
      console.error(err);
      alert("Could not save. Check Firestore rules and connection.");
    } finally {
      $("save").disabled = false;
    }
  });

  // Live read
  function watch(){
    const q = query(collection(db, "users", uid, "doses"), orderBy("taken", "desc"));
    onSnapshot(q, (snap) => {
      const rows = [];
      snap.forEach(d => rows.push({ id: d.id, ...d.data() }));
      render(rows);
    }, (err) => {
      console.error(err);
      statusText.textContent = "read error";
    });
  }

  const CAT_LABEL = { rapid: "Rapid", long: "Long", other: "Other" };
  const fmtNum = (n) => Number.isInteger(n) ? n : n.toFixed(1);

  function render(rows){
    const log = $("log");

    // Today summary
    const today = new Date(); today.setHours(0,0,0,0);
    let tUnits = 0, tDoses = 0;
    rows.forEach(r => {
      const t = r.taken?.toDate?.();
      if (t && t >= today) { tUnits += r.units || 0; tDoses++; }
    });
    $("sumUnits").innerHTML = fmtNum(tUnits) + "<small> U</small>";
    $("sumDoses").textContent = tDoses;

    if (!rows.length) {
      log.innerHTML = '<div class="empty">No doses logged yet.</div>';
      return;
    }

    // Group by day
    const groups = {};
    rows.forEach(r => {
      const t = r.taken?.toDate?.() || new Date();
      const key = t.toDateString();
      (groups[key] = groups[key] || []).push({ r, t });
    });

    log.innerHTML = "";
    for (const key in groups) {
      const items = groups[key];
      const dayUnits = items.reduce((s, x) => s + (x.r.units || 0), 0);
      const g = document.createElement("div");
      g.className = "daygroup";
      const head = document.createElement("div");
      head.className = "dayhead";
      head.innerHTML = `<span>${dayLabel(items[0].t)}</span><span>${fmtNum(dayUnits)} U</span>`;
      g.appendChild(head);

      items.forEach(({ r, t }) => {
        const cat = r.category || "other";
        const el = document.createElement("div");
        el.className = "entry " + cat;
        el.innerHTML = `
          <div class="readout">${fmtNum(r.units)}<small>U</small></div>
          <div class="meta">
            <div class="top">
              <span class="chip ${cat}">${CAT_LABEL[cat] || "Other"}</span>
              ${r.name ? `<span class="name">${esc(r.name)}</span>` : ""}
              <span class="time">${timeLabel(t)}</span>
            </div>
            ${(r.glucose != null || r.note) ? `<div class="sub">${
              r.glucose != null ? `Glucose ${fmtNum(r.glucose)}` : ""
            }${r.glucose != null && r.note ? " · " : ""}${r.note ? esc(r.note) : ""}</div>` : ""}
          </div>
          <button class="del" title="Delete" aria-label="Delete dose">✕</button>`;
        el.querySelector(".del").addEventListener("click", async () => {
          if (!confirm("Delete this entry?")) return;
          try { await deleteDoc(doc(db, "users", uid, "doses", r.id)); }
          catch (e) { console.error(e); }
        });
        g.appendChild(el);
      });
      log.appendChild(g);
    }
  }

  function dayLabel(d){
    const today = new Date(); today.setHours(0,0,0,0);
    const that = new Date(d); that.setHours(0,0,0,0);
    const diff = Math.round((today - that) / 86400000);
    if (diff === 0) return "Today";
    if (diff === 1) return "Yesterday";
    return d.toLocaleDateString(undefined, { weekday:"short", month:"short", day:"numeric" });
  }
  function timeLabel(d){
    return d.toLocaleTimeString(undefined, { hour:"numeric", minute:"2-digit" });
  }
  function esc(s){
    return String(s).replace(/[&<>"']/g, c => ({ "&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;" }[c]));
  }
</script>
</body>
</html>
