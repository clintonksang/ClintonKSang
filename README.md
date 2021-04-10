### Hi there 👋 I`m Clinton

name: Update README with my latest coding stats

on:
  schedule:
    - cron: '30 5 * * *'

jobs:
  update-Readme:
    name: Automatically update my README  
    runs-on: ubuntu-latest
    steps:
      - uses: tariksahni/coding-stats-wakatime@v1.0.0
        with:
          WAKATIME_API_KEY: ${{ 52585fc7-90eb-4cc7-a7f0-ef3ab9373c21 }}
          SHOW_MONTHLY: true
          GITHUB_TOKEN: ${{ github.token }}
          GITHUB_ACTION: ${{ github.action }}
