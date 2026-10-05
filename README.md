<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio — main.cpp</title>
    
    <!-- Connect design -->
    <link rel="stylesheet" href="style.css">
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
            <span class="cmt">//   School:  Catanduanes State University</span><br>
            <span class="cmt">// ==========================================</span>
        </div>

        <!-- ===== ABOUT ME ===== -->
        <div class="code-block">
            <h2>📌 About Me</h2>
            
            <span class="kw">string</span> <span class="fn">about_me</span>() {<br>
            &nbsp;&nbsp;return <span class="str">"I am a Computer Science student who is interested in learning more about technology and programming. Coding can be challenging for me, especially when I encounter problems that I do not understand right away. However, I do not want to give up.

I always try my best to practice, learn from my mistakes, and understand each lesson step by step. I know that learning to code takes time, patience, and continuous practice. My goal is to improve my skills and become more confident in programming as I continue my studies. 🚀"</span>;<br>
            }
        </div>

        <!-- ===== SKILLS ===== -->
        <div class="code-block">
            <h2>🛠️ My Skills</h2>
            
            <span class="kw">void</span> <span class="fn">skills</span>() {<br>
            &nbsp;&nbsp;<span class="fn">cout</span> <<span class="str"> "C++"</span> <<span class="str"> " | "</span><br>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<<span class="str"> "C"</span> <<span class="str"> " | "</span><br>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<<span class="str"> "HTML/CSS"</span> <<span class="str"> " | "</span><br>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<<span class="str"> "JavaScript"</span> <<span class="str"> " | "</span><br>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<<span class="str"> "Problem Solving"</span> <<span class="str"> endl</span>;<br>
            }
        </div>

        <!-- ===== PROJECTS ===== -->
        <div class="code-block">
            <h2>My Project <h2>
            
            Student Portfolio Website
            
        
            A personal portfolio website created using
            HTML and CSS.
                                                                 
            
            &nbsp;&nbsp;<span class="cm>C++ Programming Activities
            &nbsp;&nbsp;<span class="fn">cout</span> <<span class="str"> "Different C++ programming activities completed during my studies.
            
            &nbsp;&nbsp;<span class="cmt">//Data Structure Activities
            &nbsp;&nbsp;<span class="fn">cout</span> <<span class +"str"> "Activities involving arrays,stack,queues and linked list 
            
            &nbsp;&nbsp;<span class="kw">return</span> <span class="accent">0</span>;<br>
            }
        </div>

        <!-- ===== CONTACT ===== -->
        <div class="code-block">
            <h2>📬 Contact</h2>
            
            <span class="kw">string</span> <span class="fn">email</span> = <span class="str">"magnoleamae653@gmail.com"</span>;<br>
            <span class="kw">string</span> <span class="fn">github</span> = <span class="str">"github.com/markreyes-dev"</span>;<br>
            <span class="kw">string</span> <span class="fn">Facebook</span> = <span class= "st">"Lea Mae P. Magno"</span>;
        </div>

        <!-- ===== FOOTER ===== -->
        <div class="footer">
            <span class="cmt">// Built with 💻 & passion — © 2026 Mark Anthony Reyes</span><br>
            <span class="cmt">// 
        </div>
            /* ===== GLOBAL STYLES — BACKGROUND & FONT ===== */
* {
margin: 0;
padding: 0;
box-sizing: border-box;
font-family: 'Consolas', 'Monaco', monospace;
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
