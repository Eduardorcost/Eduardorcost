- 👋 Hi, I’m @Eduardo Rodrigues Costa;
- 👀 I’m interested in: Programming, technologies and Linux;
- 🌱 I’m currently learning: Linux ,Programming Languages,C,Java,Python,C++,C#,JavaScript and Ruby;
- 💞️ I’m looking :a job opportunity and new knowledge and challenges in technology as well as a personal project;
- 📫 How to reach me my e-mail: eduardorcost@gmail.com or th page.

 name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Summary Cards
      - uses: actions/checkout@v2
      - uses: vn7n24fzkq/github-profile-summary-cards@release
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
        with:
          USERNAME: ${{ github.repository_owner }}

      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
