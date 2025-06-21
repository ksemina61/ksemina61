![Snake animation](https://raw.githubusercontent.com/ksemina61/snk/output/github-contribution-grid-snake.svg)

name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"  # Обновлять ежедневно
  workflow_dispatch:     # Можно запустить вручную

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: ksemina61  # Ваш никнейм
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-snake-dark.svg?palette=github-dark
