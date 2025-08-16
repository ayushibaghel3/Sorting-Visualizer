<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>README • Sorting Visualizer</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --bg: linear-gradient(135deg, #1e1e2f 0%, #2a2a72 50%, #6b2a87 100%);
      --card: rgba(255, 255, 255, 0.06);
      --border: rgba(255, 255, 255, 0.12);
      --text: #f7f7fb;
      --muted: #cfd2ff;
      --accent: #ff7ad9;
      --chip: rgba(255, 255, 255, 0.12);
      --code: #0f1226;
    }
    * { box-sizing: border-box; }
    html, body { height: 100%; }
    body {
      margin: 0;
      font-family: "Poppins", system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif;
      color: var(--text);
      background: var(--bg);
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
    }
    .wrap {
      max-width: 980px;
      margin: 40px auto;
      padding: 0 20px 60px;
    }
    header {
      text-align: center;
      margin-bottom: 28px;
    }
    h1 {
      font-size: clamp(2.2rem, 4.6vw, 3.6rem);
      margin: 0 0 8px;
      font-weight: 700;
      letter-spacing: 0.5px;
    }
    .tagline {
      font-size: clamp(1rem, 2vw, 1.125rem);
      opacity: 0.9;
      margin: 0 auto 8px;
      max-width: 780px;
    }
    .chiprow { display: flex; gap: 8px; justify-content: center; flex-wrap: wrap; }
    .chip {
      font-size: 0.85rem;
      padding: 6px 10px;
      border-radius: 999px;
      background: var(--chip);
      border: 1px solid var(--border);
    }
    section {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 22px 22px;
      margin: 16px 0;
      box-shadow: 0 6px 24px rgba(0,0,0,0.18);
    }
    h2 {
      font-size: clamp(1.35rem, 2.6vw, 1.75rem);
      margin: 0 0 14px;
      font-weight: 700;
    }
    h3 {
      font-size: 1.05rem;
      margin: 18px 0 10px;
    }
    p { line-height: 1.7; margin: 10px 0; color: var(--muted); }
    ul { margin: 10px 0 0 0; padding-left: 18px; }
    li { margin: 6px 0; color: var(--muted); }
    .kbd, code, pre { font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace; }

    /* Code block */
    pre {
      background: var(--code);
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 14px 16px;
      overflow: auto;
      line-height: 1.6;
      margin: 12px 0 0 0;
      color: #e7e9ff;
    }
    code { background: rgba(255,255,255,0.08); padding: 2px 6px; border-radius: 6px; }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 10px;
    }
    .muted { color: var(--muted); }
    .accent { color: var(--accent); font-weight: 600; }
    .footer { text-align: center; opacity: 0.9; margin-top: 22px; }
    .hr { height: 1px; background: var(--border); margin: 24px 0; border: 0; }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>🔥 Sorting Visualizer</h1>
      <p class="tagline">An interactive <b>Sorting Visualizer</b> built using <b>HTML</b>, <b>CSS</b>, and <b>JavaScript</b>. Currently supports <b>Bubble Sort</b> with smooth animations and a modern UI design.</p>
      <div class="chiprow">
        <span class="chip">HTML5</span>
        <span class="chip">CSS3</span>
        <span class="chip">JavaScript (ES6)</span>
      </div>
    </header>

    <section>
      <h2>✨ Features</h2>
      <ul>
        <li>🎲 <b>Dynamic Array Generation</b> – Generates a new random array with bars every time.</li>
        <li>🔄 <b>Bubble Sort Visualization</b> – Step-by-step sorting with animations.</li>
        <li>🎨 <b>Modern UI</b> – Gradient background, animated flaming title, responsive layout.</li>
        <li>⚡ <b>Smooth Animations</b> – Bars highlight during comparison and change colors once sorted.</li>
      </ul>
    </section>

    <section>
      <h2>🛠️ Tech Stack</h2>
      <div class="grid">
        <div><b>HTML5</b> – Structure</div>
        <div><b>CSS3</b> – Design &amp; Animations</div>
        <div><b>JavaScript (ES6)</b> – Sorting logic &amp; Interactivity</div>
      </div>
    </section>

    <section>
      <h2>🚀 Getting Started</h2>
      <p>Open <code>index.html</code> in your browser. For GitHub users:</p>
      <pre><code># Clone the repository
 git clone https://github.com/your-username/sorting-visualizer.git

# Navigate to project folder
 cd sorting-visualizer

# Open index.html in your browser</code></pre>
    </section>

    <section>
      <h2>🧮 Bubble Sort Algorithm</h2>
      <p>Bubble Sort works by repeatedly swapping adjacent elements if they are in the wrong order. The largest element “bubbles up” to the end of the array in each pass.</p>
      <h3>🔑 Pseudocode</h3>
      <pre><code>for i = 0 to n-1
    for j = 0 to n-i-1
        if arr[j] &gt; arr[j+1]
            swap(arr[j], arr[j+1])</code></pre>
      <h3>📊 Complexity</h3>
      <ul>
        <li><b>Best Case:</b> O(n) (already sorted)</li>
        <li><b>Average Case:</b> O(n²)</li>
        <li><b>Worst Case:</b> O(n²)</li>
        <li><b>Space:</b> O(1)</li>
      </ul>
    </section>

    <section>
      <h2>📸 Screenshots</h2>
      <p class="muted">Add a screenshot file to your repo and reference it:</p>
      <pre><code>![App Screenshot](./screenshot.png)</code></pre>
    </section>

    <section>
      <h2>🔮 Future Scope</h2>
      <ul>
        <li>Add more algorithms: Merge Sort, Quick Sort, Insertion Sort, Heap Sort</li>
        <li>Speed control for animations</li>
        <li>Color indicators (comparing, swapping, sorted)</li>
        <li>Sound effects during swaps</li>
      </ul>
    </section>

    <section>
      <h2>🙏 Acknowledgement</h2>
      <p>This project was inspired by a YouTube tutorial and customized to enhance my learning of HTML, CSS, and JavaScript.</p>
    </section>

    <hr class="hr"/>
    <p class="footer">👩‍💻 Developed with ❤️ by <b>Ayu</b></p>
  </div>
</body>
</html>



    
