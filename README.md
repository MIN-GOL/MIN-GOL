![](https://github-readme-stats.vercel.app/api?username=MIN-GOL&theme=dark)
name: WakaTime Readme

on:
  push:
    branches:
      - master
  schedule:
    - cron: '0 19 * * *'

jobs:
  update-readme:
    runs-on: ubuntu-latest
    steps:
      - uses: athul/waka-readme@master
        with:
          WAKATIME_API_KEY: ${{ secrets.43b95836-db12-41fb-8aed-5aa59d0c354c }}
