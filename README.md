# Hi there 👋, I'm Nikayel

### 🚀 About Me
- 🔭 I’m currently working on **Ill talk about it later:)**
- 👯 I’m looking to collaborate on **innovative projects**
- 💬 Ask me about **Web Development**
- 📫 How to reach me: **[alikayeljamal@gmail.com / NikayelAli]**
- ⚡ Fun fact: *I love building, breaking, and fixing things.*

---

### 🛠️ Tech Stack
![Python](https://img.shields.io/badge/-Python-333?style=flat&logo=python)
![JavaScript](https://img.shields.io/badge/-JavaScript-333?style=flat&logo=javascript)
![React](https://img.shields.io/badge/-React-333?style=flat&logo=react)
![Node.js](https://img.shields.io/badge/-Node.js-333?style=flat&logo=node.js)
![Git](https://img.shields.io/badge/-Git-333?style=flat&logo=git)

---

---

---

⭐️ From nikayel(https://github.com/Nikayel)
name: Generate Snake


on:
schedule:
- cron: "0 0 * * *" # daily
workflow_dispatch:


jobs:
build:
runs-on: ubuntu-latest
steps:
- name: Generate snake.svg
uses: Platane/snk@v3
with:
github_user_name: YOUR_GITHUB_USERNAME
outputs: |
dist/snake.svg
- name: Upload to GitHub Pages
uses: crazy-max/ghaction-github-pages@v4
with:
target_branch: gh-pages
build_dir: dist
env:
GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
