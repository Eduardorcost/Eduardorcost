- 👋 Hi, I’m @Eduardo Rodrigues Costa;
- 👀 I’m interested in: Programming, technologies and Linux;
- 🌱 I’m currently learning: Linux ,Programming Languages,C,Java,Python,C++,C#,JavaScript and Ruby;
- 💞️ I’m looking :a job opportunity and new knowledge and challenges in technology as well as a personal project;
- 📫 How to reach me my e-mail: eduardorcost@gmail.com or th page.

<div>
  <a href="https://github.com/eduardorcost">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=eduardorcost&show_icons=true&theme=dracula&include_all_commits=true&count_private=true"/>
  <img height="150em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=eduardorcost&layout=compact&langs_count=16&theme=dark"/>
  <img height="150em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=eduardorcost&layout=compact&langs_count=7&theme=dark"/>
</div>
<div style="display: inline_block"><br>
  <img align="center" alt="Rafa-Js" height="10" width="10" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  
  
  name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
