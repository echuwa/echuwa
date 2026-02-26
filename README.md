<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ECHUWA · dev & network engineer</title>
    <!-- Fonts & Icons (subtle, clean) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,600;14..32,700&family=Fira+Code:wght@400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #0a0c10;
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
            color: #e1e9f0;
            line-height: 1.5;
            display: flex;
            justify-content: center;
            padding: 2rem 1.2rem;
        }

        .profile-card {
            max-width: 1280px;
            width: 100%;
            background: rgba(10, 14, 23, 0.75);
            backdrop-filter: blur(2px);
            border-radius: 3rem 3rem 2rem 2rem;
            box-shadow: 0 25px 50px -8px rgba(0, 212, 255, 0.08), 0 0 0 1px rgba(0, 212, 255, 0.1) inset;
            overflow: hidden;
            padding: 2rem 2rem 1rem 2rem;
        }

        /* smooth gradient borders / headings */
        h2 {
            font-weight: 600;
            font-size: 2rem;
            letter-spacing: -0.02em;
            background: linear-gradient(130deg, #ffffff, #a0e9ff);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            display: inline-flex;
            align-items: center;
            gap: 0.6rem;
            border-bottom: 2px solid rgba(0, 212, 255, 0.25);
            padding-bottom: 0.4rem;
            margin: 2rem 0 1.5rem 0;
        }

        h2 i, h2 img {
            filter: drop-shadow(0 0 6px #00d4ff66);
        }

        /* table clean */
        table {
            width: 100%;
            border-collapse: collapse;
        }

        td {
            vertical-align: top;
            padding: 0.5rem;
        }

        /* badge style overhaul — clean glass */
        .info-badge {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            background: rgba(13, 20, 30, 0.8);
            border: 1px solid #2a3a4a;
            backdrop-filter: blur(4px);
            padding: 0.6rem 1.4rem;
            border-radius: 60px;
            font-size: 0.95rem;
            font-weight: 500;
            color: #ccddee;
            transition: 0.2s ease;
            box-shadow: 0 4px 12px rgba(0,0,0,0.5);
            margin: 0.3rem 0.3rem 0.3rem 0;
            width: fit-content;
        }

        .info-badge i, .info-badge .emoji {
            color: #00d4ff;
            font-size: 1.2rem;
            width: 1.6rem;
            text-align: center;
        }

        .info-badge:hover {
            border-color: #00d4ff;
            transform: translateY(-2px);
            background: rgba(0, 212, 255, 0.05);
        }

        /* stats / skill bars analog */
        .skill-bar-row {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin: 1rem 0;
        }
        .skill-tag {
            min-width: 120px;
            font-weight: 600;
            color: #b0d4ff;
        }
        .bar-bg {
            flex: 1;
            height: 10px;
            background: #1e2a36;
            border-radius: 20px;
            overflow: hidden;
        }
        .bar-fill {
            height: 100%;
            background: linear-gradient(90deg, #00d4ff, #4a9eff);
            border-radius: 20px;
            box-shadow: 0 0 8px #00d4ff;
        }

        /* network block terminal style */
        .net-box {
            background: #0b121b;
            border: 1px solid #2a4a5a;
            border-radius: 28px;
            padding: 1.8rem 1.5rem;
            font-family: 'Fira Code', monospace;
            box-shadow: 0 15px 30px -15px #00d4ff20, inset 0 1px 2px #ffffff0c;
        }

        .net-line {
            display: flex;
            border-bottom: 1px dashed #2e4b5c;
            padding: 0.8rem 0;
        }

        .net-cat {
            width: 160px;
            color: #00d4ff;
            font-weight: 600;
            letter-spacing: 0.3px;
        }

        .net-desc {
            color: #bfd9f0;
        }

        /* repo cards soft */
        .repo-pin {
            background: #111b24;
            border-radius: 2rem;
            border: 1px solid #253545;
            transition: all 0.2s;
        }
        .repo-pin:hover {
            border-color: #00d4ff;
            background: #14222e;
        }

        /* section separation */
        .section-divider {
            margin: 3rem 0 1.5rem;
            height: 2px;
            background: linear-gradient(90deg, transparent, #00d4ff40, #a0d4ff80, #00d4ff40, transparent);
        }

        /* footer wave text */
        .wave-footer {
            font-size: 1.2rem;
            font-weight: 400;
            text-shadow: 0 2px 5px #00d4ff30;
        }

        a {
            text-decoration: none;
            color: inherit;
        }
    </style>
</head>
<body>
<div class="profile-card">

    <!-- ========= HEADER ========= -->
    <div align="center">
        <!-- wave header (capsule render simulated with gradient & text) -->
        <div style="width:100%; background: linear-gradient(115deg, #0d1117 0%, #0a3d62 30%, #1a6b8a 70%, #00d4ff 100%); height: 200px; border-radius: 0 0 130px 130px / 0 0 60px 60px; display: flex; flex-direction: column; justify-content: center; align-items: center; box-shadow: 0 20px 35px -8px #00d4ff50; margin-bottom: 1.5rem;">
            <div style="font-size: 5.5rem; font-weight: 800; letter-spacing: 4px; color: white; text-shadow: 0 0 10px #00d4ff, 0 4px 15px #0a3d62; line-height: 1.2;">ECHUWA</div>
            <div style="font-size: 1.3rem; background: rgba(0,0,0,0.3); backdrop-filter: blur(4px); padding: 0.3rem 2rem; border-radius: 60px; color: #fff; font-weight: 500; border: 1px solid #ffffff40;">⚡ Full-Stack Developer | Network Engineer ⚡</div>
        </div>

        <!-- typing svg placeholder (SVG look with typed effect simulation) -->
        <a href="https://github.com/echuwa">
            <div style="background: #0f1a24; padding: 0.9rem 2rem; border-radius: 60px; border: 1px solid #00d4ff80; box-shadow: 0 0 20px #00d4ff30; font-family: 'Fira Code', monospace; font-size: 1.4rem; font-weight: 600; color: #b5f0ff; display: inline-block; margin: 0.5rem 0;">
                <span>🐘 PHP & Laravel Expert · ☕ Spring Boot · 💚 Vue.js · 🔌 Networks</span>
            </div>
        </a>
        <br/>

        <!-- badges row -->
        <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 0.7rem; margin: 1.5rem 0 0.8rem;">
            <span class="info-badge"><i class="fas fa-map-pin"></i> 🌍 Tanzania</span>
            <span class="info-badge"><i class="fas fa-briefcase"></i> 💼 Open to Work</span>
            <span class="info-badge"><i class="fas fa-bolt"></i> ⚡ Code & Networks</span>
            <span class="info-badge"><i class="fas fa-eye"></i> 👁️ Profile Views 1.4k</span>
            <span class="info-badge"><i class="fas fa-users"></i> 👥 Followers 187</span>
        </div>
    </div>

    <!-- divider subtle -->
    <div class="section-divider"></div>

    <!-- ========= WHO AM I ========= -->
    <div align="center">
        <h2><img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="32" alt="wave"> Who Am I?</h2>
    </div>

    <div style="display: flex; flex-wrap: wrap; gap: 2rem; justify-content: center;">
        <!-- left personal info -->
        <div style="flex: 1 1 300px;">
            <h3 style="color: #b0f0ff; margin-bottom: 1rem; font-weight: 500;"><i class="fas fa-user-astronaut" style="color:#00d4ff;"></i> Personal Info</h3>
            <div class="info-badge"><i class="fas fa-tag"></i> 👤 Emmanuel Chuwa</div>
            <div class="info-badge"><i class="fas fa-mask"></i> 🎭 Mr.chmod / echuwa</div>
            <div class="info-badge"><i class="fas fa-location-dot"></i> 🌍 Dar es Salaam, Tanzania</div>
            <div class="info-badge"><i class="fas fa-envelope"></i> 📧 emmanuelchuwa243@gmail.com</div>
            <div class="info-badge"><i class="fab fa-github"></i> 🐙 github.com/echuwa</div>
            <div class="info-badge"><i class="fas fa-code"></i> 💼 Full‑Stack Developer</div>
            <div class="info-badge"><i class="fas fa-network-wired"></i> 🔌 Network Engineer</div>
        </div>
        <!-- right currently -->
        <div style="flex: 1 1 300px;">
            <h3 style="color: #b0f0ff; margin-bottom: 1rem; font-weight: 500;"><i class="fas fa-rocket" style="color:#00d4ff;"></i> Currently</h3>
            <div class="info-badge"><i class="fas fa-fire"></i> 🔥 Laravel & Vue.js Projects</div>
            <div class="info-badge"><i class="fas fa-dharmachakra"></i> 📚 Docker 🐳</div>
            <div class="info-badge"><i class="fas fa-dharmachakra"></i> 📚 Kubernetes ☸️</div>
            <div class="info-badge"><i class="fas fa-cloud"></i> 📚 AWS Cloud ☁️</div>
            <div class="info-badge"><i class="fas fa-arrows-rotate"></i> 📚 DevOps 🔄</div>
            <div class="info-badge"><i class="fas fa-comment"></i> 💬 Ask me: PHP, Laravel, Networks</div>
        </div>
    </div>

    <div align="center" style="margin: 2rem 0 0.5rem; font-style: italic; background: #0e1a22; padding: 1.2rem; border-radius: 60px; border-left: 5px solid #00d4ff;">
        💡 *"Clean code today → Scalable systems tomorrow!"* — <strong>Emmanuel Chuwa</strong>
    </div>

    <div class="section-divider"></div>

    <!-- ========= TECH ARSENAL ========= -->
    <div align="center">
        <h2><i class="fas fa-tools"></i> Complete Tech Arsenal</h2>
    </div>

    <!-- backend details open (using skill bars) -->
    <details open style="margin-bottom: 2rem;">
        <summary style="font-size: 1.5rem; font-weight: 600; color: #d0edff; cursor: pointer; list-style: none;"><span>🔷 Backend Development</span></summary>
        <div style="margin-top: 1.2rem; display: flex; flex-wrap: wrap; gap: 2rem;">
            <div style="flex: 2; min-width: 280px;">
                <div class="skill-bar-row"><span class="skill-tag"><i class="fab fa-php" style="color:#777BB4;"></i> PHP</span> <div class="bar-bg"><div class="bar-fill" style="width:95%"></div></div><span style="margin-left:0.8rem;">95%</span></div>
                <div class="skill-bar-row"><span class="skill-tag"><i class="fab fa-laravel" style="color:#FF2D20;"></i> Laravel</span> <div class="bar-bg"><div class="bar-fill" style="width:93%"></div></div><span>93%</span></div>
                <div class="skill-bar-row"><span class="skill-tag"><i class="fas fa-leaf" style="color:#6DB33F;"></i> Spring Boot</span> <div class="bar-bg"><div class="bar-fill" style="width:78%"></div></div><span>78%</span></div>
                <div class="skill-bar-row"><span class="skill-tag"><i class="fab fa-java" style="color:#ED8B00;"></i> Java</span> <div class="bar-bg"><div class="bar-fill" style="width:75%"></div></div><span>75%</span></div>
            </div>
            <div style="flex:1; color:#b0c8e0; font-size:0.95rem; background: #0d1722; border-radius: 28px; padding: 1.2rem;">
                <p><span style="color:#00d4ff;">◉</span> Server-side scripting, OOP, MVC, Eloquent</p>
                <p><span style="color:#00d4ff;">◉</span> REST APIs, Microservices, JPA</p>
                <p><span style="color:#00d4ff;">◉</span> Collections, Streams, Security</p>
            </div>
        </div>
    </details>

    <details open style="margin-bottom: 2rem;">
        <summary style="font-size: 1.5rem; font-weight: 600; color: #d0edff;"><span>🔶 Frontend Development</span></summary>
        <div style="margin-top: 1.2rem; display: flex; flex-wrap: wrap; gap: 2rem;">
            <div style="flex:2; min-width:280px;">
                <div class="skill-bar-row"><span class="skill-tag"><i class="fab fa-js" style="color:#F7DF1E;"></i> JS</span> <div class="bar-bg"><div class="bar-fill" style="width:90%"></div></div><span>90%</span></div>
                <div class="skill-bar-row"><span class="skill-tag"><i class="fab fa-vuejs" style="color:#4FC08D;"></i> Vue.js</span> <div class="bar-bg"><div class="bar-fill" style="width:88%"></div></div><span>88%</span></div>
                <div class="skill-bar-row"><span class="skill-tag"><i class="fab fa-html5" style="color:#E34F26;"></i> HTML5</span> <div class="bar-bg"><div class="bar-fill" style="width:95%"></div></div><span>95%</span></div>
                <div class="skill-bar-row"><span class="skill-tag"><i class="fab fa-css3-alt" style="color:#1572B6;"></i> CSS3</span> <div class="bar-bg"><div class="bar-fill" style="width:90%"></div></div><span>90%</span></div>
            </div>
            <div style="flex:1; color:#b0c8e0; background:#0d1722; border-radius:28px; padding:1.2rem;">
                <p><span style="color:#00d4ff;">◉</span> ES6+, Composition API, Vuex, Router</p>
                <p><span style="color:#00d4ff;">◉</span> Semantic HTML, Flex/Grid, animations</p>
            </div>
        </div>
    </details>

    <details open style="margin-bottom: 2rem;">
        <summary style="font-size: 1.5rem; font-weight: 600;"><span>🗄️ Databases</span></summary>
        <div style="display: flex; flex-wrap: wrap; gap:2rem; margin-top:1rem;">
            <div style="flex:2;">
                <div class="skill-bar-row"><span class="skill-tag"><i class="fas fa-database" style="color:#4479A1;"></i> MySQL</span> <div class="bar-bg"><div class="bar-fill" style="width:92%"></div></div><span>92%</span></div>
                <div class="skill-bar-row"><span class="skill-tag"><i class="fas fa-leaf" style="color:#47A248;"></i> MongoDB</span> <div class="bar-bg"><div class="bar-fill" style="width:78%"></div></div><span>78%</span></div>
                <div class="skill-bar-row"><span class="skill-tag"><i class="fas fa-database" style="color:#336791;"></i> PgAdmin4/PSQL</span> <div class="bar-bg"><div class="bar-fill" style="width:75%"></div></div><span>75%</span></div>
            </div>
            <div style="flex:1; background:#0d1722; border-radius:28px; padding:1.2rem;">Stored procedures, aggregation, JSONB, indexing</div>
        </div>
    </details>

    <!-- Network engineering (beautiful box) -->
    <details open>
        <summary style="font-size: 1.5rem; font-weight: 600;"><span>🌐 Network Engineering</span></summary>
        <div class="net-box" style="margin-top: 1rem;">
            <div class="net-line"><span class="net-cat">OSI Layer 2</span><span class="net-desc">VLANs • STP • EtherChannel • MAC Tables</span></div>
            <div class="net-line"><span class="net-cat">OSI Layer 3</span><span class="net-desc">OSPF • EIGRP • RIP • Static • BGP</span></div>
            <div class="net-line"><span class="net-cat">Security</span><span class="net-desc">Firewalls • ACLs • VPN • IPSec • NAT</span></div>
            <div class="net-line"><span class="net-cat">Infrastructure</span><span class="net-desc">DNS • DHCP • NTP • Monitoring</span></div>
            <div class="net-line"><span class="net-cat">Wireless</span><span class="net-desc">WLAN • WPA2/3 • Access Points</span></div>
            <div class="net-line"><span class="net-cat">Tools</span><span class="net-desc">Cisco Packet Tracer • Wireshark • PuTTY</span></div>
        </div>
        <div align="center" style="margin: 1rem 0 0; display:flex; flex-wrap:wrap; gap:0.5rem; justify-content:center;">
            <span class="info-badge"><i class="fas fa-project-diagram"></i> VLAN Config</span>
            <span class="info-badge"><i class="fas fa-route"></i> Routing & Switching</span>
            <span class="info-badge"><i class="fas fa-shield-halved"></i> Firewall Setup</span>
            <span class="info-badge"><i class="fas fa-lock"></i> VPN Config</span>
        </div>
    </details>

    <!-- tools collapsed -->
    <details style="margin-top: 2rem;">
        <summary style="font-size:1.3rem; color:#b0f0ff;">⚙️ Tools & DevOps</summary>
        <div style="display: flex; gap: 1rem; flex-wrap: wrap; margin:1rem 0;">
            <span class="info-badge">Git</span><span class="info-badge">GitHub</span><span class="info-badge">VSCode</span><span class="info-badge">Postman</span>
            <span class="info-badge">Linux</span><span class="info-badge">Docker</span><span class="info-badge">K8s (learning)</span>
        </div>
    </details>

    <!-- GitHub stats -->
    <div class="section-divider"></div>
    <div align="center">
        <h2><i class="fas fa-chart-line"></i> GitHub Statistics</h2>
        <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 0.8rem;">
            <img height="160" src="https://github-readme-stats.vercel.app/api?username=echuwa&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=00d4ff&icon_color=00d4ff&text_color=8892b0" />
            <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=echuwa&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00d4ff&text_color=8892b0&langs_count=8" />
        </div>
        <div style="margin-top: 1rem;">
            <img src="https://github-readme-streak-stats.herokuapp.com/?user=echuwa&theme=tokyonight&hide_border=true&background=0d1117&stroke=00d4ff&ring=00d4ff&fire=ff6b35&currStreakLabel=00d4ff&sideLabels=8892b0&dates=8892b0" />
        </div>
    </div>

    <!-- featured projects -->
    <div class="section-divider"></div>
    <div align="center">
        <h2><i class="fas fa-code-branch"></i> Featured Projects</h2>
        <div style="display: flex; flex-wrap: wrap; gap: 1rem; justify-content: center;">
            <!-- simulated pinned repos -->
            <div class="repo-pin" style="padding: 1.2rem; width:280px;">
                <i class="fas fa-bookmark" style="color:#00d4ff;"></i> <strong style="font-size:1.2rem;">Hostel-Management-Syste-Updated-Code</strong>
                <p style="color:#9bb8da;">Updated hostel system with Laravel</p>
            </div>
            <div class="repo-pin" style="padding: 1.2rem; width:280px;">
                <i class="fas fa-bookmark" style="color:#00d4ff;"></i> <strong style="font-size:1.2rem;">Hostel</strong>
                <p style="color:#9bb8da;">Vue + Laravel dormitory app</p>
            </div>
            <div class="repo-pin" style="padding: 1.2rem; width:280px;">
                <i class="fas fa-bookmark" style="color:#00d4ff;"></i> <strong style="font-size:1.2rem;">Java_framework</strong>
                <p style="color:#9bb8da;">Custom spring-like experiment</p>
            </div>
            <div class="repo-pin" style="padding: 1.2rem; width:280px;">
                <i class="fas fa-bookmark" style="color:#00d4ff;"></i> <strong style="font-size:1.2rem;">ethay</strong>
                <p style="color:#9bb8da;">Network monitoring tool</p>
            </div>
        </div>
    </div>

    <!-- contribution graph placeholder (simulated) -->
    <div class="section-divider"></div>
    <div align="center">
        <h2><i class="fas fa-chart-area"></i> Contribution Graph</h2>
        <div style="width:100%; height:110px; background: linear-gradient(90deg, #0d1a24 0%, #00d4ff40 30%, #ff6b3540 70%, #0d1a24 100%); border-radius: 60px;"></div>
        <p style="color:#587e9c;"><i>github-readme-activity-graph (tokyo-night theme)</i></p>
    </div>

    <!-- trophies simplified -->
    <div align="center" style="margin: 2rem 0;">
        <h2><i class="fas fa-trophy"></i> Trophies</h2>
        <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 0.4rem;">
            <span class="info-badge">🏆 GitHub Star</span><span class="info-badge">🏆 Laravel Contributor</span><span class="info-badge">🏆 Network+</span><span class="info-badge">🏆 5x Hackathon</span>
        </div>
    </div>

    <!-- connect section -->
    <div class="section-divider"></div>
    <div align="center">
        <h2><i class="fas fa-handshake"></i> Let's Connect</h2>
        <div style="display: flex; flex-wrap: wrap; gap: 1rem; justify-content: center;">
            <a href="mailto:emmanuelchuwa243@gmail.com" class="info-badge"><i class="fas fa-envelope"></i> Gmail</a>
            <a href="https://github.com/echuwa" class="info-badge"><i class="fab fa-github"></i> GitHub/echuwa</a>
            <a href="#" class="info-badge"><i class="fab fa-linkedin"></i> LinkedIn (Emmanuel Chuwa)</a>
        </div>
    </div>

    <!-- snake animation placeholder (text graphic) -->
    <div align="center" style="margin: 2.5rem 0 1rem;">
        <picture>
            <img alt="github-snake" src="https://raw.githubusercontent.com/echuwa/echuwa/output/github-contribution-grid-snake-dark.svg" style="max-width:100%; border-radius: 30px; background:#0b141e; padding: 0.8rem;" />
        </picture>
        <p style="margin-top:0.5rem; color:#5c7f99;"><i>snake contribution animation</i></p>
    </div>

    <div align="center" style="margin: 1.5rem 0;">
        <i style="color:#b0e0ff;">⚡ "The best code is the code that solves real problems elegantly." — Emmanuel Chuwa</i>
    </div>

    <!-- footer wave gradient -->
    <div style="width:100%; height:120px; background: linear-gradient(90deg, #00d4ff, #1a6b8a, #0d1117); border-radius: 80px 80px 0 0; display: flex; align-items: center; justify-content: center; color: white; font-size: 1.7rem; font-weight: 400; text-shadow: 0 2px 6px black;">
        Thanks for visiting! 🚀
    </div>

</div> <!-- profile-card -->
</body>
</html>
