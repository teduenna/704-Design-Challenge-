<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Web Basics Lab</title>
<style>
  :root {
    --ink: #1a1a1a;
    --muted: #5a5a5a;
    --line: #e2e2e2;
    --accent: #2f5d50;
    --bg: #fbfaf8;
  }
  * { box-sizing: border-box; }
  body {
    margin: 0;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
    color: var(--ink);
    background: var(--bg);
    line-height: 1.5;
  }
  .wrap {
    max-width: 760px;
    margin: 0 auto;
    padding: 64px 24px 96px;
  }
  header {
    margin-bottom: 48px;
    padding-bottom: 32px;
    border-bottom: 1px solid var(--line);
  }
  h1 {
    font-family: 'Newsreader', Georgia, serif;
    font-weight: 500;
    font-size: clamp(32px, 5vw, 46px);
    line-height: 1.1;
    letter-spacing: -0.015em;
    margin: 0 0 12px;
  }
  header p {
    color: var(--muted);
    font-size: 17px;
    margin: 0;
    max-width: 56ch;
  }
  ol {
    list-style: none;
    margin: 0;
    padding: 0;
    counter-reset: module;
  }
  li {
    counter-increment: module;
    border-bottom: 1px solid var(--line);
  }
  li:first-child { border-top: 1px solid var(--line); }
  a.module {
    display: flex;
    align-items: baseline;
    gap: 18px;
    padding: 20px 4px;
    text-decoration: none;
    color: var(--ink);
    transition: background 0.15s ease;
  }
  a.module:hover { background: #f1efe9; }
  a.module::before {
    content: counter(module, decimal-leading-zero);
    font-family: 'Newsreader', Georgia, serif;
    font-weight: 500;
    font-size: 15px;
    color: var(--accent);
    flex-shrink: 0;
    min-width: 24px;
  }
  a.module .title {
    font-size: 18px;
    font-weight: 500;
  }
  .glossary {
    margin-top: 40px;
    padding-top: 8px;
  }
  .glossary a.module::before {
    content: "—";
    font-family: inherit;
  }
  footer {
    margin-top: 56px;
    color: var(--muted);
    font-size: 14px;
  }
</style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Web Basics Lab</h1>
      <p>A self-paced introduction to HTML and CSS, built for graduate Instructional Design students.</p>
    </header>

    <ol>
      <li><a class="module" href="01-anatomy.html"><span class="title">Anatomy of a tag</span></a></li>
      <li><a class="module" href="02-page-structure.html"><span class="title">The shape of every page</span></a></li>
      <li><a class="module" href="03-everyday-tags.html"><span class="title">The tags you'll use daily</span></a></li>
      <li><a class="module" href="04-how-css-works.html"><span class="title">How CSS works</span></a></li>
      <li><a class="module" href="05-box-model.html"><span class="title">The box model</span></a></li>
      <li><a class="module" href="06-semantics-and-ia.html"><span class="title">Semantics &amp; information architecture</span></a></li>
      <li><a class="module" href="07-layout.html"><span class="title">Arranging things: flex &amp; grid</span></a></li>
      <li><a class="module" href="08-knowledge-check.html"><span class="title">Knowledge check</span></a></li>
      <li><a class="module" href="09-build-the-page.html"><span class="title">Build the page, step by step</span></a></li>
    </ol>

    <ol class="glossary">
      <li><a class="module" href="Glossary-Handout.html"><span class="title">Glossary of Web Terms</span></a></li>
    </ol>

    <footer>
      EDIT 704 &middot; Web Basics Lab
    </footer>
  </div>
</body>
</html>
