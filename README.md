$ mkdir -p /home/user/profile/assets && cat > /home/user/profile/assets/header.svg <<'EOF'
<svg xmlns="http://www.w3.org/2000/svg" width="1000" height="260" viewBox="0 0 1000 260">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0" stop-color="#050816"/>
      <stop offset="1" stop-color="#0b1b3a"/>
    </linearGradient>
    <linearGradient id="g" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0" stop-color="#1e90ff"/>
      <stop offset="1" stop-color="#a855f7"/>
    </linearGradient>
    <filter id="glow"><feGaussianBlur stdDeviation="4" result="b"/><feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
  </defs>
  <rect width="1000" height="260" fill="url(#bg)"/>

  <!-- estrelas piscando -->
  <g fill="#fff">
    <circle cx="80" cy="40" r="1.5"><animate attributeName="opacity" values="0.1;1;0.1" dur="3s" repeatCount="indefinite"/></circle>
    <circle cx="210" cy="210" r="1.2"><animate attributeName="opacity" values="1;0.1;1" dur="2.4s" repeatCount="indefinite"/></circle>
    <circle cx="420" cy="30" r="1.4"><animate attributeName="opacity" values="0.1;1;0.1" dur="3.6s" repeatCount="indefinite"/></circle>
    <circle cx="620" cy="225" r="1.6"><animate attributeName="opacity" values="1;0.2;1" dur="2.8s" repeatCount="indefinite"/></circle>
    <circle cx="760" cy="45" r="1.2"><animate attributeName="opacity" values="0.2;1;0.2" dur="3.2s" repeatCount="indefinite"/></circle>
    <circle cx="940" cy="190" r="1.5"><animate attributeName="opacity" values="1;0.1;1" dur="2.6s" repeatCount="indefinite"/></circle>
  </g>

  <!-- planeta + órbita girando -->
  <g transform="translate(830 130)">
    <circle r="46" fill="url(#g)" opacity="0.25" filter="url(#glow)">
      <animate attributeName="r" values="44;50;44" dur="4s" repeatCount="indefinite"/>
    </circle>
    <text x="0" y="22" text-anchor="middle" font-family="Arial Black, Arial, sans-serif" font-size="64" font-weight="900" fill="#fff">R</text>
    <g>
      <ellipse rx="95" ry="30" fill="none" stroke="url(#g)" stroke-width="5" stroke-linecap="round" stroke-dasharray="260 340" filter="url(#glow)" transform="rotate(-25)"/>
      <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="8s" repeatCount="indefinite"/>
    </g>
    <circle r="6" fill="#1e90ff" filter="url(#glow)">
      <animateMotion dur="6s" repeatCount="indefinite" path="M-95,0 a95,30 0 1,0 190,0 a95,30 0 1,0 -190,0"/>
    </circle>
  </g>

  <!-- textos -->
  <text x="60" y="95" font-family="Segoe UI, Arial, sans-serif" font-size="22" fill="#7aa8ff" letter-spacing="6">
    <animate attributeName="opacity" values="0;1" dur="1.2s" fill="freeze"/>
    OLÁ, EU SOU O DIOGO
  </text>
  <text x="60" y="150" font-family="Segoe UI, Arial, sans-serif" font-size="52" font-weight="800" fill="url(#g)">
    <animate attributeName="opacity" values="0;1" dur="1.6s" begin="0.4s" fill="freeze"/>
    Ramuski Inovation Group
  </text>
  <rect x="60" y="165" height="4" rx="2" fill="url(#g)" width="0">
    <animate attributeName="width" values="0;520" dur="1.5s" begin="1s" fill="freeze"/>
  </rect>
  <text x="60" y="205" font-family="Segoe UI, Arial, sans-serif" font-size="20" fill="#cbd5e1">
    <animate attributeName="opacity" values="0;1" dur="1.4s" begin="1.6s" fill="freeze"/>
    Desenvolvedor Full Stack · Sites sob medida · Engenharia de Software
  </text>
</svg>
EOF
cat > /home/user/profile/README.md <<'EOF'
<div align="center">

<img src="https://raw.githubusercontent.com/Diogo1006br/Diogo1006br/main/assets/header.svg" alt="Ramuski Inovation Group" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=7AA8FF&center=true&vCenter=true&width=700&lines=Fundador+da+Ramuski+Inovation+Group+🚀;Engenharia+de+Software+na+Católica+🎓;Back-end+%2B+Front-end+💻;Seu+site+do+zero+ao+deploy+⚡" alt="Typing SVG" />

<br/>

<img src="https://komarev.com/ghpvc/?username=Diogo1006br&label=Visitas&color=1e90ff&style=for-the-badge" />
<img src="https://img.shields.io/badge/Ramuski-Inovation%20Group-a855f7?style=for-the-badge" />
<img src="https://img.shields.io/badge/Aberto%20a%20projetos-22c55e?style=for-the-badge" />

</div>

---

## 🚀 Ramuski Inovation Group

Sou o **Diogo**, estudante de Engenharia de Software na Católica e fundador da **Ramuski Inovation Group**.
Criamos **sites, sistemas e soluções digitais sob medida**, com foco em desempenho, design e resultado.

- 💻 Desenvolvimento back-end e front-end
- 🌐 Sites institucionais, landing pages e sistemas web
- 🎮 Nas horas vagas, jogos online (sou bem competitivo)
- 📩 **Quer um site? Faça um orçamento comigo!**

## 🛠️ Stack

<div align="center">
<img src="https://skillicons.dev/icons?i=js,ts,html,css,python,nodejs,react,git,github,mysql,postgres,figma&perline=12" />
</div>

---

## 📊 Estatísticas

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=Diogo1006br&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github&include_all_commits=true&count_private=true" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Diogo1006br&layout=donut&theme=tokyonight&hide_border=true&langs_count=8" />

<br/>

<img src="https://streak-stats.demolab.com/?user=Diogo1006br&theme=tokyonight&hide_border=true" height="170" />

<br/>

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Diogo1006br&theme=tokyonight" height="170" />
<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Diogo1006br&theme=tokyonight" height="170" />

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Diogo1006br&theme=tokyo-night&hide_border=true&area=true&custom_title=Atividade%20nos%20%C3%BAltimos%2031%20dias" width="100%" />

</div>

## 🐍 Contribuições

<img src="https://raw.githubusercontent.com/Diogo1006br/Diogo1006br/output/github-snake-dark.svg" width="100%"/>

## 📫 Contato

<div align="center">
<a href="https://linkedin.com/in/SEU-USUARIO"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:dramuski@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://wa.me/55SEUNUMERO"><img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/></a>
</div>
EOF
cat > /home/user/profile/snake.yml <<'EOF'
name: Generate Snake
on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:
permissions:
  contents: write
jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-snake-dark.svg?palette=github-dark
      - uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
EOF
python3 -c "import xml.dom.minidom as m;m.parse('/home/user/profile/assets/header.svg');print('svg ok')"; ls -R /home/user/profile

svg ok
/home/user/profile:
README.md
assets
snake.yml

/home/user/profile/assets:
header.svg
