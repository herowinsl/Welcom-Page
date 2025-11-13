<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Profile</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #0d1117;
            font-family: 'Courier New', monospace;
            min-height: 100vh;
            padding: 40px 20px;
            color: #c9d1d9;
        }

        .terminal {
            max-width: 900px;
            margin: 0 auto;
            background: #161b22;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 0 50px rgba(56, 189, 248, 0.2);
            border: 1px solid #30363d;
        }

        .terminal-header {
            background: #21262d;
            padding: 12px 20px;
            display: flex;
            align-items: center;
            gap: 8px;
            border-bottom: 1px solid #30363d;
        }

        .terminal-btn {
            width: 12px;
            height: 12px;
            border-radius: 50%;
        }

        .btn-close { background: #ff5f56; }
        .btn-minimize { background: #ffbd2e; }
        .btn-maximize { background: #27c93f; }

        .terminal-title {
            margin-left: 15px;
            color: #8b949e;
            font-size: 0.9em;
        }

        .terminal-body {
            padding: 30px;
            line-height: 1.8;
        }

        .prompt {
            color: #58a6ff;
            margin-right: 10px;
        }

        .command {
            color: #7ee787;
        }

        .output {
            margin: 10px 0 20px 0;
            padding-left: 20px;
        }

        .ascii-art {
            color: #58a6ff;
            font-size: 0.8em;
            line-height: 1.2;
            margin: 20px 0;
            white-space: pre;
            font-family: monospace;
        }

        .section-title {
            color: #f0883e;
            font-weight: bold;
            margin: 25px 0 15px 0;
            font-size: 1.1em;
        }

        .highlight {
            color: #58a6ff;
            font-weight: bold;
        }

        .tech-item {
            display: inline-block;
            color: #7ee787;
            margin: 5px 15px 5px 0;
            position: relative;
            padding-left: 15px;
        }

        .tech-item::before {
            content: '▹';
            position: absolute;
            left: 0;
            color: #f0883e;
        }

        .link-line {
            margin: 10px 0;
            transition: all 0.3s ease;
        }

        .link-line:hover {
            transform: translateX(10px);
            color: #58a6ff;
        }

        .link-icon {
            color: #f0883e;
            margin-right: 10px;
        }

        .link {
            color: #58a6ff;
            text-decoration: none;
            border-bottom: 1px dashed #58a6ff;
            transition: all 0.3s ease;
        }

        .link:hover {
            color: #7ee787;
            border-bottom-color: #7ee787;
        }

        .blink {
            animation: blink 1s infinite;
        }

        @keyframes blink {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0; }
        }

        .status-bar {
            background: #21262d;
            padding: 15px 30px;
            border-top: 1px solid #30363d;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 15px;
        }

        .status-item {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.9em;
        }

        .status-dot {
            width: 8px;
            height: 8px;
            border-radius: 50%;
            background: #7ee787;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.5; }
        }

        .divider {
            color: #30363d;
            margin: 20px 0;
        }

        @media (max-width: 768px) {
            .terminal-body {
                padding: 20px;
            }
            
            .ascii-art {
                font-size: 0.6em;
            }

            .status-bar {
                flex-direction: column;
                align-items: flex-start;
            }
        }
    </style>
</head>
<body>
    <div class="terminal">
        <div class="terminal-header">
            <div class="terminal-btn btn-close"></div>
            <div class="terminal-btn btn-minimize"></div>
            <div class="terminal-btn btn-maximize"></div>
            <div class="terminal-title">elias@github: ~/profile</div>
        </div>

        <div class="terminal-body">
            <div class="ascii-art">
 _____ _ _             
| ____| (_) __ _ ___  
|  _| | | |/ _` / __| 
| |___| | | (_| \__ \ 
|_____|_|_|\__,_|___/ 
                      </div>

            <div>
                <span class="prompt">elias@dev:~$</span>
                <span class="command">cat about.txt</span>
            </div>
            <div class="output">
                <p>Full Stack Developer | Student @ <span class="highlight">CMC-BMK</span></p>
                <p>Status: <span class="highlight">Year 2/2</span> - Building & Learning</p>
                <p>Location: Morocco 🇲🇦</p>
                <p>Philosophy: <em>"Code is poetry, bugs are just plot twists"</em></p>
            </div>

            <div class="divider">────────────────────────────────────────</div>

            <div>
                <span class="prompt">elias@dev:~$</span>
                <span class="command">ls skills/</span>
            </div>
            <div class="output">
                <div class="section-title">&gt; Frontend Development</div>
                <span class="tech-item">HTML5</span>
                <span class="tech-item">CSS3</span>
                <span class="tech-item">JavaScript</span>
                <span class="tech-item">React.js</span>
                <span class="tech-item">Tailwind CSS</span>

                <div class="section-title">&gt; Backend Development</div>
                <span class="tech-item">Node.js</span>
                <span class="tech-item">Express.js</span>
                <span class="tech-item">Python</span>
                <span class="tech-item">PHP</span>

                <div class="section-title">&gt; Database & Tools</div>
                <span class="tech-item">MongoDB</span>
                <span class="tech-item">MySQL</span>
                <span class="tech-item">Git</span>
                <span class="tech-item">GitHub</span>
                <span class="tech-item">VS Code</span>
            </div>

            <div class="divider">────────────────────────────────────────</div>

            <div>
                <span class="prompt">elias@dev:~$</span>
                <span class="command">cat stats.json</span>
            </div>
            <div class="output">
                <p>{</p>
                <p>  <span class="highlight">"experience"</span>: "2+ years",</p>
                <p>  <span class="highlight">"current_focus"</span>: "Full Stack Development",</p>
                <p>  <span class="highlight">"learning"</span>: "Always something new",</p>
                <p>  <span class="highlight">"coffee_consumed"</span>: "∞ cups",</p>
                <p>  <span class="highlight">"bugs_fixed"</span>: "Too many to count"</p>
                <p>}</p>
            </div>

            <div class="divider">────────────────────────────────────────</div>

            <div>
                <span class="prompt">elias@dev:~$</span>
                <span class="command">echo $SOCIAL_LINKS</span>
            </div>
            <div class="output">
                <div class="link-line">
                    <span class="link-icon">📸</span>
                    Instagram: <a href="https://instagram.com/elias__slh" target="_blank" class="link">@elias__slh</a>
                </div>
                <div class="link-line">
                    <span class="link-icon">💼</span>
                    GitHub: <a href="https://github.com/herowinsl" target="_blank" class="link">@herowinsl</a>
                </div>
                <div class="link-line">
                    <span class="link-icon">📧</span>
                    Email: <a href="mailto:iliassalhi1949@gmail.com" class="link">iliassalhi1949@gmail.com</a>
                </div>
            </div>

            <div style="margin-top: 30px;">
                <span class="prompt">elias@dev:~$</span>
                <span class="blink">▊</span>
            </div>
        </div>

        <div class="status-bar">
            <div class="status-item">
                <span class="status-dot"></span>
                <span>Online & Coding</span>
            </div>
            <div class="status-item">
                <span>📍 CMC-BMK</span>
            </div>
            <div class="status-item">
                <span>🚀 Open to Collaborate</span>
            </div>
        </div>
    </div>
</body>
</html>
