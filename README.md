<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=44&duration=1400&pause=0&color=A371F7&center=true&vCenter=true&repeat=false&width=820&height=80&lines=Pramod+Dixit" alt="Pramod Dixit" />
</p>

<p align="center">
  <img align="top" src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=1200&pause=300&color=2DA44E&vCenter=true&repeat=false&width=820&height=28&lines=;%E2%9D%AF+cat+focus.txt" alt="❯ cat focus.txt" /><br>
  <img align="top" src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=1200&pause=300&color=388BFD&vCenter=true&repeat=false&width=820&height=28&lines=;;backend+engineering+%C2%B7+data+science+%C2%B7+machine+learning+%C2%B7+low-level+programming" alt="backend engineering · data science · machine learning · low-level programming" /><br>
  <img align="top" src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=1200&pause=300&color=2DA44E&vCenter=true&repeat=false&width=820&height=28&lines=;;;%E2%9D%AF+cat+mindset.txt" alt="❯ cat mindset.txt" /><br>
  <img align="top" src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=1200&pause=300&color=DB6D28&vCenter=true&repeat=false&width=820&height=28&lines=;;;;building+software%2C+and+understanding+the+machine+underneath+it" alt="building software, and understanding the machine underneath it" /><br>
  <img align="top" src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=1200&pause=300&color=2DA44E&vCenter=true&repeat=false&width=820&height=28&lines=;;;;;%E2%9D%AF+ls+.%2Fnow" alt="❯ ls ./now" /><br>
  <img align="top" src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=1200&pause=300&color=DB61A2&vCenter=true&repeat=false&width=820&height=28&lines=;;;;;;relay%2F%C2%A0%C2%A0%C2%A0%C2%A0ml-from-scratch%2F%C2%A0%C2%A0%C2%A0%C2%A0os-internals%2F" alt="relay/  ml-from-scratch/  os-internals/" />
</p>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/People/Technologist.png" width="34" /> About me

<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Travel%20and%20places/Rocket.png" width="22" /> &nbsp;Currently building **Relay**, a webhook delivery service<br>
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Laptop.png" width="22" /> &nbsp;I work mostly on **backend, data science and low-level programming**: REST APIs, backend services, background jobs, data analysis, ML models and systems-level code<br>
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Smilies/Robot.png" width="22" /> &nbsp;Going deeper into **machine learning**, from the math behind a model to how it learns<br>
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Gear.png" width="22" /> &nbsp;Spent a lot of time on **low-level programming**: memory layout, stack vs heap, pointers and system calls<br>
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Desktop%20Computer.png" width="22" /> &nbsp;Studying **operating systems and computer architecture** to understand what really happens beneath my code<br>
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Activities/Puzzle%20Piece.png" width="22" /> &nbsp;I enjoy solving **algorithmic problems**, especially dynamic programming, graphs and recursion<br>
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Hand%20gestures/Brain.png" width="22" /> &nbsp;I like learning things from **first principles**, and I keep asking "why?" until I hit the hardware<br>
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Smilies/Speech%20Balloon.png" width="22" /> &nbsp;Ask me about backend, data science and ML, or systems internals: memory management, operating systems and computer architecture<br>
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Briefcase.png" width="22" /> &nbsp;Open to opportunities in **backend, data science and ML**

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Travel%20and%20places/Building%20Construction.png" width="34" /> Currently building: Relay

A webhook delivery service. It accepts events, delivers them to subscriber endpoints in background workers, and retries failed deliveries instead of dropping them.

```mermaid
flowchart LR
    P[Producer] -->|POST event| A[FastAPI]
    A -->|store| M[(MongoDB)]
    A -->|enqueue delivery| R[(Redis)]
    R --> W[Celery worker]
    W -->|HTTP POST| S[Subscriber endpoint]
    W -. retry on failure .-> R

    classDef ext fill:#ff9e64,stroke:#ff9e64,color:#1a1b27
    classDef api fill:#7aa2f7,stroke:#7aa2f7,color:#1a1b27
    classDef store fill:#9ece6a,stroke:#9ece6a,color:#1a1b27
    classDef queue fill:#bb9af7,stroke:#bb9af7,color:#1a1b27
    classDef worker fill:#7dcfff,stroke:#7dcfff,color:#1a1b27
    class P,S ext
    class A api
    class M store
    class R queue
    class W worker
```

<p>
  <img src="https://img.shields.io/badge/Python-1a1b27?style=flat-square&logo=python&logoColor=7aa2f7" alt="Python" />
  <img src="https://img.shields.io/badge/FastAPI-1a1b27?style=flat-square&logo=fastapi&logoColor=009688" alt="FastAPI" />
  <img src="https://img.shields.io/badge/MongoDB-1a1b27?style=flat-square&logo=mongodb&logoColor=47A248" alt="MongoDB" />
  <img src="https://img.shields.io/badge/Celery-1a1b27?style=flat-square&logo=celery&logoColor=9ece6a" alt="Celery" />
  <img src="https://img.shields.io/badge/Redis-1a1b27?style=flat-square&logo=redis&logoColor=DC382D" alt="Redis" />
  <img src="https://img.shields.io/badge/status-in_progress-e0af68?style=flat-square" alt="Status: in progress" />
</p>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Ladder.png" width="34" /> How I learn: from apps to hardware

I learn by going down the stack. I start at the top by building something real, like a backend, an API or an ML model. Then I follow my code down one layer at a time, asking what runs it, who manages it and what finally executes it, until I understand what the machine is actually doing.

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=16&duration=900&pause=150&color=2F81F7&multiline=true&repeat=false&width=560&height=180&lines=;%C2%A0%C2%A0apps%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0web%C2%A0backends%C2%A0%C2%B7%C2%A0APIs%C2%A0%C2%B7%C2%A0data%C2%A0%C2%B7%C2%A0ML%C2%A0models;%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%E2%86%93%C2%A0%C2%A0what%C2%A0runs%C2%A0it%3F;%C2%A0%C2%A0runtime%C2%A0%C2%A0%C2%A0%C2%A0languages%C2%A0%C2%B7%C2%A0memory%C2%A0%C2%B7%C2%A0compilers;%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%E2%86%93%C2%A0%C2%A0who%C2%A0manages%C2%A0it%3F;%C2%A0%C2%A0OS%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0processes%C2%A0%C2%B7%C2%A0threads%C2%A0%C2%B7%C2%A0syscalls;%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%C2%A0%E2%86%93%C2%A0%C2%A0what%C2%A0executes%C2%A0it%3F;%C2%A0%C2%A0hardware%C2%A0%C2%A0%C2%A0assembly%C2%A0%C2%B7%C2%A0registers%C2%A0%C2%B7%C2%A0CPU" alt="apps → runtime → OS → hardware" />
</p>

<p align="center"><sub>⬆️ building software &nbsp;·&nbsp; understanding computers ⬇️</sub></p>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Toolbox.png" width="34" /> Tech stack

<p align="center"><b>Languages</b></p>
<p align="center"><img src="https://skillicons.dev/icons?i=c,cpp,java,py,js,ts" alt="C, C++, Java, Python, JavaScript, TypeScript" /></p>
<p align="center">
  <img src="https://img.shields.io/badge/ARM_Assembly-1a1b27?style=for-the-badge&logo=arm&logoColor=7dcfff" alt="ARM Assembly" />
  <img src="https://img.shields.io/badge/x86_Assembly-1a1b27?style=for-the-badge" alt="x86 Assembly" />
</p>

<p align="center"><b>Backend & databases</b></p>
<p align="center"><img src="https://skillicons.dev/icons?i=nodejs,express,django,mysql,mongodb,redis" alt="Node.js, Express, Django, MySQL, MongoDB, Redis" /></p>

<p align="center"><b>Data science & ML</b></p>
<p align="center">
  <img src="https://img.shields.io/badge/NumPy-1a1b27?style=for-the-badge&logo=numpy&logoColor=4DABCF" alt="NumPy" />
  <img src="https://img.shields.io/badge/pandas-1a1b27?style=for-the-badge&logo=pandas&logoColor=bb9af7" alt="pandas" />
  <img src="https://img.shields.io/badge/Matplotlib-1a1b27?style=for-the-badge" alt="Matplotlib" />
  <img src="https://img.shields.io/badge/Seaborn-1a1b27?style=for-the-badge" alt="Seaborn" />
  <img src="https://img.shields.io/badge/scikit--learn-1a1b27?style=for-the-badge&logo=scikitlearn&logoColor=F7931E" alt="scikit-learn" />
</p>

<p align="center"><b>Tools</b></p>
<p align="center"><img src="https://skillicons.dev/icons?i=linux,ubuntu,git,github,vim,vscode" alt="Linux, Ubuntu, Git, GitHub, Vim, VS Code" /></p>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Bar%20Chart.png" width="34" /> GitHub stats

<p align="center">
  <img height="170" src="https://github-stats-extended.vercel.app/api?username=PramodDixit2003&show_icons=true&hide_rank=true&theme=tokyonight&hide_border=true&border_radius=10" alt="GitHub stats" />
  <img height="170" src="https://github-stats-extended.vercel.app/api/top-langs/?username=PramodDixit2003&layout=compact&langs_count=6&hide=css,html,scss&theme=tokyonight&hide_border=true&border_radius=10" alt="Top languages" />
</p>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Envelope%20with%20Arrow.png" width="34" /> Reach me

<p>
  <a href="mailto:pramoddixit098@gmail.com"><img src="https://img.shields.io/badge/Gmail-1a1b27?style=for-the-badge&logo=gmail&logoColor=EA4335" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/pramod-dixit-2b36b91bb/"><img src="https://img.shields.io/badge/LinkedIn-1a1b27?style=for-the-badge&logo=linkedin&logoColor=7aa2f7" alt="LinkedIn" /></a>
  <a href="https://leetcode.com/u/pramoddixit608/"><img src="https://img.shields.io/badge/LeetCode-1a1b27?style=for-the-badge&logo=leetcode&logoColor=FFA116" alt="LeetCode" /></a>
</p>
