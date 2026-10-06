<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio — main.cpp</title>
 
    <style>
        /* ===== GLOBAL STYLES — BACKGROUND & FONT ===== */
        * {
          margin: 0;
          padding: 0;
          box-sizing: border-box;
          font-family: 'Consolas', 'Monaco', 'Courier New', monospace;
        }
 
        :root {
          --panel: rgba(15, 23, 42, 0.85);
          --border: #3730a3;
          --text: #e2e8f0;
          --keyword: #c084fc;   /* #include, string, void, return */
          --string: #86efac;    /* "text" */
          --function: #7dd3fc;  /* function names */
          --comment: #94a3b8;   /* // comments */
          --accent: #fbbf24;    /* numbers, headings */
        }
 
        body {
          /* 🎨 CHANGE BACKGROUND HERE — pick ONE option below: */
 
          /* Option 1: Dark Blue-Purple Gradient (RECOMMENDED) */
          background: linear-gradient(135deg, #0f172a 0%, #1e1b4b 50%, #312e81 100%);
 
          /* Option 2: Simple Solid Dark Color */
          /* background: #0f172a; */
 
          /* Option 3: Teal-Green Gradient */
          /* background: linear-gradient(135deg, #064e3b 0%, #0f766e 100%); */
 
          /* Option 4: Red-Orange Gradient */
          /* background: linear-gradient(135deg, #7f1d1d 0%, #c2410c 100%); */
 
          background-attachment: fixed;
          color: var(--text);
          line-height: 1.7;
          min-height: 100vh;
          padding: 24px 16px;
        }
 
        /* ===== LAYOUT ===== */
        .container {
          max-width: 820px;
          margin: 0 auto;
        }
 
        .code-header,
        .code-block,
        .footer {
          background: var(--panel);
          border: 1px solid var(--border);
          border-radius: 10px;
          padding: 20px 24px;
          margin-bottom: 20px;
          overflow-x: auto;
        }
 
        .code-block h2 {
          color: var(--accent);
          font-size: 1.1rem;
          margin-bottom: 12px;
        }
 
        /* ===== FILE TABS ===== */
        .file-tab {
          display: flex;
          flex-wrap: wrap;
          gap: 4px;
          margin: -20px -24px 16px;
          padding: 8px 12px 0;
          background: rgba(0, 0, 0, 0.35);
          border-radius: 10px 10px 0 0;
        }
 
        .tab {
          padding: 6px 14px;
          font-size: 0.85rem;
          color: var(--comment);
          border-radius: 6px 6px 0 0;
        }
 
        .tab.active {
          color: var(--text);
          background: var(--panel);
          border-bottom: 2px solid var(--accent);
        }
 
        /* ===== SYNTAX COLORS ===== */
        .kw     { color: var(--keyword); }
        .str    { color: var(--string); }
        .fn     { color: var(--function); }
        .cmt    { color: var(--comment); }
        .accent { color: var(--accent); }
 
        /* ===== CODE LINES ===== */
        .ln { white-space: pre-wrap; }
        .i1 { padding-left: 2ch; }
        .i2 { padding-left: 4ch; }
        .i3 { padding-left: 6ch; }
 
        .footer {
          text-align: center;
          font-size: 0.85rem;
        }
 
        a { color: var(--function); }
 
        /* ===== SMALL SCREENS ===== */
        @media (max-width: 600px) {
          .code-header,
          .code-block,
          .footer {
            padding: 16px;
          }
          .file-tab {
            margin: -16px -16px 12px;
          }
        }
    </style>
</head>
<body>
    <div class="container">
 
        <!-- ===== HEADER — Like C++ Header ===== -->
        <div class="code-header">
            <div class="file-tab">
                <span class="tab active">main.cpp</span>
                <span class="tab">skills.h</span>
                <span class="tab">projects.hpp</span>
            </div>
 
            <span class="kw">#include</span> <span class="str">&lt;iostream&gt;</span><br>
            <span class="kw">#include</span> <span class="str">&lt;string&gt;</span><br>
            <span class="kw">using namespace</span> <span class="fn">std</span>;<br><br>
 
            <span class="cmt">// ==========================================</span><br>
            <span class="cmt">//   STUDENT PORTFOLIO — Version 1.0</span><br>
            <span class="cmt">//   Name: Lea Mae P. Magno</span><br>
            <span class="cmt">//   Role: Computer Science Student 💻</span><br>
            <span class="cmt">//   School: Catanduanes State University</span><br>
            <span class="cmt">// ==========================================</span>
        </div>
 
        <!-- ===== ABOUT ME ===== -->
        <div class="code-block">
            <h2>📌 About Me</h2>
 
            <div class="ln"><span class="kw">string</span> <span class="fn">about_me</span>() {</div>
            <div class="ln i1"><span class="kw">return</span> <span class="str">"I am a Computer Science student who is interested in learning more about technology and programming. Coding can be challenging for me, especially when I encounter problems that I do not understand right away. However, I do not want to give up.<br><br>I always try my best to practice, learn from my mistakes, and understand each lesson step by step. I know that learning to code takes time, patience, and continuous practice. My goal is to improve my skills and become more confident in programming as I continue my studies. 🚀"</span>;</div>
            <div class="ln">}</div>
        </div>
 
        <!-- ===== SKILLS ===== -->
        <div class="code-block">
            <h2>🛠️ My Skills</h2>
 
            <div class="ln"><span class="kw">void</span> <span class="fn">skills</span>() {</div>
            <div class="ln i1"><span class="fn">cout</span> &lt;&lt; <span class="str">"C++"</span> &lt;&lt; <span class="str">" | "</span></div>
            <div class="ln i3">&lt;&lt; <span class="str">"C"</span> &lt;&lt; <span class="str">" | "</span></div>
            <div class="ln i3">&lt;&lt; <span class="str">"HTML/CSS"</span> &lt;&lt; <span class="str">" | "</span></div>
            <div class="ln i3">&lt;&lt; <span class="str">"JavaScript"</span> &lt;&lt; <span class="str">" | "</span></div>
            <div class="ln i3">&lt;&lt; <span class="str">"Problem Solving"</span> &lt;&lt; <span class="fn">endl</span>;</div>
            <div class="ln">}</div>
        </div>
 
        <!-- ===== PROJECTS ===== -->
        <div class="code-block">
            <h2>💼 My Projects</h2>
 
            <div class="ln"><span class="kw">void</span> <span class="fn">projects</span>() {</div>
 
            <div class="ln i1"><span class="cmt">// Student Portfolio Website</span></div>
            <div class="ln i1"><span class="fn">cout</span> &lt;&lt; <span class="str">"A personal portfolio website created using HTML and CSS."</span>;</div>
            <br>
 
            <div class="ln i1"><span class="cmt">// C++ Programming Activities</span></div>
            <div class="ln i1"><span class="fn">cout</span> &lt;&lt; <span class="str">"Different C++ programming activities completed during my studies."</span>;</div>
            <br>
 
            <div class="ln i1"><span class="cmt">// Data Structure Activities</span></div>
            <div class="ln i1"><span class="fn">cout</span> &lt;&lt; <span class="str">"Activities involving arrays, stacks, queues, and linked lists."</span>;</div>
            <br>
 
            <div class="ln i1"><span class="kw">return</span> <span class="accent">0</span>;</div>
            <div class="ln">}</div>
        </div>
 
        <!-- ===== CONTACT ===== -->
        <div class="code-block">
            <h2>📬 Contact</h2>
 
            <div class="ln"><span class="kw">string</span> <span class="fn">email</span> = <span class="str">"magnoleamae653@gmail.com"</span>;</div>
            <div class="ln"><span class="kw">string</span> <span class="fn">github</span> = <span class="str">"github.com/markreyes-dev"</span>;</div>
            <div class="ln"><span class="kw">string</span> <span class="fn">facebook</span> = <span class="str">"Lea Mae P. Magno"</span>;</div>
        </div>
 
        <!-- ===== FOOTER ===== -->
        <div class="footer">
            <span class="cmt">// Built with 💻 &amp; passion — © 2026 Lea Mae P. Magno</span>
        </div>
 
    </div>
</body>
</html>
