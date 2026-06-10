<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>공부 시간 배분</title>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@400;700;900&family=Space+Mono:wght@700&display=swap" rel="stylesheet" />
  <style>
    /* ─── CSS 변수 ─── */
    :root {
      --bg: #f4f0e8;
      --card: #ffffff;
      --green-1: #1e4d3b;
      --green-2: #3a7d5e;
      --green-3: #6aab84;
      --green-4: #97c9a8;
      --green-5: #c2dfc9;
      --green-6: #dff0e2;
      --accent-red: #d93030;
      --accent-blue: #1a8fd1;
      --text: #1a1a1a;
      --muted: #888;
      --shadow: 0 4px 24px rgba(30,77,59,0.10);
    }

    /* ─── 기본 초기화 ─── */
    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Noto Sans KR', sans-serif;
      background: var(--bg);
      min-height: 100vh;
      color: var(--text);
      padding: 32px 16px 60px;
    }

    /* ─── 제목 ─── */
    h1 {
      text-align: center;
      font-size: 2.2rem;
      font-weight: 900;
      letter-spacing: -1px;
      color: var(--green-1);
      margin-bottom: 4px;
    }
    .subtitle {
      text-align: center;
      color: var(--muted);
      font-size: 0.92rem;
      margin-bottom: 36px;
    }

    /* ─── 레이아웃 ─── */
    .main-grid {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      gap: 24px;
      max-width: 1060px;
      margin: 0 auto;
      align-items: start;
    }

    /* ─── 카드 공통 ─── */
    .card {
      background: var(--card);
      border-radius: 20px;
      padding: 28px 24px;
      box-shadow: var(--shadow);
    }

    /* ─── 왼쪽: 시간 입력 ─── */
    .input-section { display: flex; flex-direction: column; gap: 24px; }

    .clock-block { display: flex; flex-direction: column; gap: 12px; }
    .clock-block label {
      font-weight: 700;
      font-size: 1rem;
      color: var(--accent-red);
    }
    .clock-block label span { color: var(--accent-blue); }

    .clock-wrap {
      display: flex;
      align-items: center;
      gap: 14px;
    }

    /* SVG 아날로그 시계 */
    .clock-svg { flex-shrink: 0; }
    .clock-svg circle { fill: none; stroke: var(--text); stroke-width: 4; }
    .hand { stroke: var(--text); stroke-width: 3; stroke-linecap: round; transition: transform 0.3s; transform-origin: 50px 50px; }
    .hand-min { stroke: var(--accent-red); stroke-width: 2.5; }

    .time-inputs { display: flex; align-items: center; gap: 6px; }
    .time-inputs input {
      width: 58px;
      padding: 8px 6px;
      border: 2px solid #d0d0d0;
      border-radius: 10px;
      font-size: 1.3rem;
      font-family: 'Space Mono', monospace;
      font-weight: 700;
      text-align: center;
      color: var(--text);
      outline: none;
      transition: border-color 0.2s;
      background: #fafafa;
    }
    .time-inputs input:focus { border-color: var(--green-2); background: #fff; }
    .time-inputs span { font-size: 1.4rem; font-weight: 900; color: var(--muted); }

    /* ─── 과목 입력 영역 ─── */
    .subjects-section { display: flex; flex-direction: column; gap: 10px; }
    .subjects-section h3 { font-size: 0.95rem; font-weight: 700; color: var(--green-1); margin-bottom: 4px; }

    .subject-row {
      display: flex;
      gap: 8px;
      align-items: center;
      animation: fadeIn 0.25s ease;
    }
    @keyframes fadeIn { from { opacity: 0; transform: translateY(-4px); } to { opacity: 1; transform: translateY(0); } }

    .subject-row input[type="text"] {
      flex: 1;
      padding: 7px 10px;
      border: 2px solid #d0d0d0;
      border-radius: 9px;
      font-size: 0.9rem;
      font-family: 'Noto Sans KR', sans-serif;
      outline: none;
      transition: border-color 0.2s;
    }
    .subject-row input[type="text"]:focus { border-color: var(--green-3); }

    .subject-row input[type="number"] {
      width: 64px;
      padding: 7px 6px;
      border: 2px solid #d0d0d0;
      border-radius: 9px;
      font-size: 0.9rem;
      font-family: 'Space Mono', monospace;
      text-align: center;
      outline: none;
      transition: border-color 0.2s;
    }
    .subject-row input[type="number"]:focus { border-color: var(--green-3); }

    .color-dot {
      width: 18px; height: 18px;
      border-radius: 50%;
      flex-shrink: 0;
    }

    /* ─── 버튼 ─── */
    .btn-remove {
      background: none; border: none; cursor: pointer;
      color: #ccc; font-size: 1.1rem; line-height: 1;
      transition: color 0.15s;
    }
    .btn-remove:hover { color: var(--accent-red); }

    .btn-add {
      display: flex; align-items: center; gap: 6px;
      background: none; border: 2px dashed #ccc;
      border-radius: 9px; padding: 7px 12px;
      font-size: 0.88rem; color: var(--muted);
      cursor: pointer; transition: all 0.2s;
      font-family: 'Noto Sans KR', sans-serif;
    }
    .btn-add:hover { border-color: var(--green-3); color: var(--green-2); }

    .btn-calc {
      width: 100%;
      background: var(--green-1);
      color: #fff;
      border: none;
      border-radius: 12px;
      padding: 13px;
      font-size: 1rem;
      font-weight: 700;
      font-family: 'Noto Sans KR', sans-serif;
      cursor: pointer;
      margin-top: 4px;
      transition: background 0.2s, transform 0.1s;
    }
    .btn-calc:hover { background: var(--green-2); }
    .btn-calc:active { transform: scale(0.98); }

    /* ─── 가운데: 파이차트 ─── */
    .chart-section {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 18px;
    }
    .chart-title {
      font-size: 1.6rem;
      font-weight: 900;
      color: var(--accent-red);
      letter-spacing: -0.5px;
      text-align: center;
    }

    canvas#pieChart {
      max-width: 240px;
      max-height: 240px;
      filter: drop-shadow(0 6px 18px rgba(30,77,59,0.18));
    }

    .total-time {
      text-align: center;
      font-size: 0.9rem;
      color: var(--muted);
    }
    .total-time strong {
      display: block;
      font-size: 1.5rem;
      font-family: 'Space Mono', monospace;
      color: var(--green-1);
    }

    /* ─── 오른쪽: 결과 ─── */
    .result-section { display: flex; flex-direction: column; gap: 20px; }

    .result-box {
      border-radius: 14px;
      padding: 18px 20px;
      display: flex;
      flex-direction: column;
      gap: 6px;
    }
    .result-box.most { background: linear-gradient(135deg, #1e4d3b11, #3a7d5e22); border: 2px solid var(--green-3); }
    .result-box.least { background: linear-gradient(135deg, #d9303011, #ff666622); border: 2px solid #f09090; }

    .result-box .label {
      font-size: 0.82rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 1px;
    }
    .result-box.most .label { color: var(--accent-blue); }
    .result-box.least .label { color: var(--accent-red); }

    .result-box .subject-name {
      font-size: 1.3rem;
      font-weight: 900;
      color: var(--text);
    }
    .result-box .subject-time {
      font-size: 0.9rem;
      color: var(--muted);
      font-family: 'Space Mono', monospace;
    }

    /* ─── 범례 ─── */
    .legend { display: flex; flex-direction: column; gap: 8px; }
    .legend-item {
      display: flex;
      align-items: center;
      gap: 10px;
      font-size: 0.88rem;
    }
    .legend-dot {
      width: 13px; height: 13px;
      border-radius: 3px;
      flex-shrink: 0;
    }
    .legend-bar-wrap { flex: 1; background: #eee; border-radius: 99px; height: 6px; overflow: hidden; }
    .legend-bar { height: 100%; border-radius: 99px; transition: width 0.6s cubic-bezier(.4,0,.2,1); }
    .legend-pct { font-family: 'Space Mono', monospace; font-size: 0.8rem; color: var(--muted); min-width: 36px; text-align: right; }

    /* ─── 안내 문구 ─── */
    .placeholder {
      text-align: center;
      color: #bbb;
      font-size: 0.88rem;
      padding: 24px 0;
    }

    /* ─── 반응형 ─── */
    @media (max-width: 800px) {
      .main-grid { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>

<h1>📚 시간 배분</h1>
<p class="subtitle">공부 시작·종료 시간과 과목별 비율을 입력하세요</p>

<div class="main-grid">

  <!-- 왼쪽: 입력 -->
  <div class="card input-section">

    <div class="clock-block">
      <label><span>공부 시작 시간</span> <span style="color:var(--accent-red)">(입력)</span></label>
      <div class="clock-wrap">
        <svg class="clock-svg" id="clockStart" width="70" height="70" viewBox="0 0 100 100">
          <circle cx="50" cy="50" r="46"/>
          <line id="startHour" class="hand" x1="50" y1="50" x2="50" y2="24"/>
          <line id="startMin" class="hand hand-min" x1="50" y1="50" x2="50" y2="16"/>
          <circle cx="50" cy="50" r="3" fill="var(--text)"/>
        </svg>
        <div class="time-inputs">
          <input type="number" id="startH" min="0" max="23" value="09" placeholder="HH" />
          <span>:</span>
          <input type="number" id="startM" min="0" max="59" value="00" placeholder="MM" />
        </div>
      </div>
    </div>

    <div class="clock-block">
      <label style="color:var(--accent-red)">공부 종료 시간 <span style="color:var(--accent-red)">(입력)</span></label>
      <div class="clock-wrap">
        <svg class="clock-svg" id="clockEnd" width="70" height="70" viewBox="0 0 100 100">
          <circle cx="50" cy="50" r="46"/>
          <line id="endHour" class="hand" x1="50" y1="50" x2="50" y2="24"/>
          <line id="endMin" class="hand hand-min" x1="50" y1="50" x2="50" y2="16"/>
          <circle cx="50" cy="50" r="3" fill="var(--text)"/>
        </svg>
        <div class="time-inputs">
          <input type="number" id="endH" min="0" max="23" value="18" placeholder="HH" />
          <span>:</span>
          <input type="number" id="endM" min="0" max="59" value="00" placeholder="MM" />
        </div>
      </div>
    </div>

    <!-- 과목 입력 -->
    <div class="subjects-section">
      <h3>📖 과목별 비율 (분 단위)</h3>
      <div id="subjectList"></div>
      <button class="btn-add" onclick="addSubject()">+ 과목 추가</button>
    </div>

    <button class="btn-calc" onclick="calculate()">계산하기 →</button>
  </div>

  <!-- 가운데: 파이차트 -->
  <div class="card chart-section">
    <div class="chart-title">시간 배분</div>
    <canvas id="pieChart" width="240" height="240"></canvas>
    <div class="total-time">
      총 공부 시간
      <strong id="totalDisplay">— 시간 — 분</strong>
    </div>
  </div>

  <!-- 오른쪽: 결과 -->
  <div class="card result-section">
    <div class="result-box most">
      <div class="label">🏆 가장 많이 한 과목</div>
      <div class="subject-name" id="mostSubject">—</div>
      <div class="subject-time" id="mostTime"></div>
    </div>
    <div class="result-box least">
      <div class="label">📉 가장 덜 한 과목</div>
      <div class="subject-name" id="leastSubject">—</div>
      <div class="subject-time" id="leastTime"></div>
    </div>
    <div class="legend" id="legend">
      <div class="placeholder">계산하기를 누르면<br>결과가 표시됩니다</div>
    </div>
  </div>

</div>

<script>
  const PALETTE = [
    '#1e4d3b','#3a7d5e','#6aab84','#97c9a8',
    '#c2dfc9','#dff0e2','#a8c5a0','#5d9970',
    '#2e6b4f','#84b898'
  ];

  let subjects = [
    { name: '수학', minutes: 120 },
    { name: '영어', minutes: 90 },
    { name: '국어', minutes: 60 },
    { name: '과학', minutes: 45 },
    { name: '사회', minutes: 45 },
  ];

  function renderSubjects() {
    const list = document.getElementById('subjectList');
    list.innerHTML = '';
    subjects.forEach((s, i) => {
      const row = document.createElement('div');
      row.className = 'subject-row';
      row.innerHTML = `
        <div class="color-dot" style="background:${PALETTE[i % PALETTE.length]}"></div>
        <input type="text" value="${s.name}" placeholder="과목명"
          oninput="subjects[${i}].name=this.value" />
        <input type="number" value="${s.minutes}" min="1" placeholder="분"
          oninput="subjects[${i}].minutes=+this.value" />
        <button class="btn-remove" onclick="removeSubject(${i})">✕</button>
      `;
      list.appendChild(row);
    });
  }

  function addSubject() {
    subjects.push({ name: '', minutes: 30 });
    renderSubjects();
  }

  function removeSubject(i) {
    subjects.splice(i, 1);
    renderSubjects();
  }

  function updateClock(prefix, h, m) {
    const hAngle = (h % 12) * 30 + m * 0.5 - 90;
    const mAngle = m * 6 - 90;
    const toXY = (angle, r) => ({
      x: 50 + r * Math.cos(angle * Math.PI / 180),
      y: 50 + r * Math.sin(angle * Math.PI / 180)
    });
    const hEnd = toXY(hAngle, 28);
    const mEnd = toXY(mAngle, 36);
    document.getElementById(prefix + 'Hour').setAttribute('x2', hEnd.x);
    document.getElementById(prefix + 'Hour').setAttribute('y2', hEnd.y);
    document.getElementById(prefix + 'Min').setAttribute('x2', mEnd.x);
    document.getElementById(prefix + 'Min').setAttribute('y2', mEnd.y);
  }

  ['startH','startM','endH','endM'].forEach(id => {
    document.getElementById(id).addEventListener('input', syncClocks);
  });

  function syncClocks() {
    updateClock('start',
      +document.getElementById('startH').value,
      +document.getElementById('startM').value);
    updateClock('end',
      +document.getElementById('endH').value,
      +document.getElementById('endM').value);
  }
  syncClocks();

  function drawPie(data) {
    const canvas = document.getElementById('pieChart');
    const ctx = canvas.getContext('2d');
    const W = canvas.width, H = canvas.height;
    const cx = W / 2, cy = H / 2, r = Math.min(W, H) / 2 - 8;
    ctx.clearRect(0, 0, W, H);

    const total = data.reduce((s, d) => s + d.value, 0);
    let startAngle = -Math.PI / 2;

    data.forEach((d, i) => {
      const slice = (d.value / total) * 2 * Math.PI;
      ctx.beginPath();
      ctx.moveTo(cx, cy);
      ctx.arc(cx, cy, r, startAngle, startAngle + slice);
      ctx.closePath();
      ctx.fillStyle = PALETTE[i % PALETTE.length];
      ctx.fill();
      ctx.strokeStyle = '#fff';
      ctx.lineWidth = 2;
      ctx.stroke();
      startAngle += slice;
    });

    ctx.beginPath();
    ctx.arc(cx, cy, r * 0.38, 0, 2 * Math.PI);
    ctx.fillStyle = '#fff';
    ctx.fill();
  }

  function calculate() {
    const sH = +document.getElementById('startH').value;
    const sM = +document.getElementById('startM').value;
    const eH = +document.getElementById('endH').value;
    const eM = +document.getElementById('endM').value;

    let totalMin = (eH * 60 + eM) - (sH * 60 + sM);
    if (totalMin <= 0) { alert('종료 시간이 시작 시간보다 늦어야 합니다!'); return; }

    const valid = subjects.filter(s => s.minutes > 0 && s.name.trim());
    if (!valid.length) { alert('과목을 하나 이상 입력하세요!'); return; }

    const rawTotal = valid.reduce((s, d) => s + d.minutes, 0);
    const scaled = valid.map(s => ({
      name: s.name,
      value: Math.round((s.minutes / rawTotal) * totalMin)
    }));

    const h = Math.floor(totalMin / 60), m = totalMin % 60;
    document.getElementById('totalDisplay').textContent = `${h}시간 ${m}분`;

    drawPie(scaled);

    const sorted = [...scaled].sort((a, b) => b.value - a.value);
    const most = sorted[0], least = sorted[sorted.length - 1];

    document.getElementById('mostSubject').textContent = most.name;
    document.getElementById('mostTime').textContent =
      `${Math.floor(most.value/60)}시간 ${most.value%60}분`;
    document.getElementById('leastSubject').textContent = least.name;
    document.getElementById('leastTime').textContent =
      `${Math.floor(least.value/60)}시간 ${least.value%60}분`;

    const legend = document.getElementById('legend');
    legend.innerHTML = '';
    scaled.forEach((d, i) => {
      const pct = Math.round(d.value / totalMin * 100);
      const item = document.createElement('div');
      item.className = 'legend-item';
      item.innerHTML = `
        <div class="legend-dot" style="background:${PALETTE[i%PALETTE.length]}"></div>
        <span style="min-width:64px;font-weight:600">${d.name}</span>
        <div class="legend-bar-wrap">
          <div class="legend-bar" style="width:0%;background:${PALETTE[i%PALETTE.length]}"
            data-pct="${pct}"></div>
        </div>
        <span class="legend-pct">${pct}%</span>
      `;
      legend.appendChild(item);
    });

    requestAnimationFrame(() => {
      document.querySelectorAll('.legend-bar').forEach(bar => {
        bar.style.width = bar.dataset.pct + '%';
      });
    });
  }

  renderSubjects();
</script>
</body>
</html>
