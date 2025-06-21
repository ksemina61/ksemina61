## Hi there 👋


![Snake animation](https://raw.githubusercontent.com/ksemina61/snk/output/github-contribution-grid-snake.svg)

name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *" 
  workflow_dispatch:  

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: ksemina61 
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-snake-dark.svg?palette=github-dark
<!--
**ksemina61/ksemina61** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
