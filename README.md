<h1 align="center">
  <br>
  <a href="https://www.tapmad.com/"><img src="https://d34080pnh6e62j.cloudfront.net/images/VideoOnDemandThumb/1648210285NewTapmadLogo-01@2x.png" alt="🔥 Tapmad Live 🔥" width="200"></a>
  <br>
  🔥 Tapmad Live Events Updater 🔥
  <br>
</h1>

<h2 align="center">A Script to trigger GitHub Actions automatically to update Tapmad Live Sports Matches & M3U Playlist</h2>

<p align="center">
  <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Made_With-Python_3.10%2B-blue" alt="Python">
  </a>
  <a href="#">
      <img src="https://img.shields.io/badge/Brand-CodeCrafter-green.svg" alt="CodeCrafter">
  </a>
  <a href="https://www.tapmad.com/">
    <img src="https://img.shields.io/badge/App-Tapmad_Sports-purple" alt="Tapmad">
  </a>
  <a href="#"><img src="https://img.shields.io/badge/Made%20in-Bangladesh_🇧🇩-green?colorA=%23ff0000&colorB=%23017e40&style=flat-square" alt="Bangladesh"></a>
</p>

# 📒 Introduction 
* This repository provides an automated way to extract **Tapmad** Live and Upcoming Sports Premium match links (like PSL, EPL, UFC, etc.) and generate a working M3U playlist. 

# 💥 Key Features
* All Live Match Links and Playlists are Updated Automatically via GitHub Actions.
* Extracts high-quality `.m3u8` links without token expiration issues.
* Bypasses Geo-restrictions using a custom PHP Proxy system.
* Generates data in both **JSON** and **M3U** format.
* Categorized streams (Live Match, Upcoming Sports Premium).
* Easily integrable into any IPTV player or Restreaming App.

## 🕹️ How To Use (For Developers)

* 👉 **[Auto Updated Matches JSON File](https://raw.githubusercontent.com/hasanhabibmottakin/tapmad-events/main/main.json)**
* 👉 **[Auto Updated M3U Playlist](https://raw.githubusercontent.com/hasanhabibmottakin/tapmad-events/main/live.m3u)**

**Example Usage in Python:**
```python
import requests

# Get the updated JSON data
link = "[https://raw.githubusercontent.com/hasanhabibmottakin/tapmad-events/main/main.json](https://raw.githubusercontent.com/hasanhabibmottakin/tapmad-events/main/main.json)"
matches = requests.get(link).json()

for match in matches:
    print(f"✓ Category: {match['category']}")
    print(f"✓ Match Title: {match['title']}")
    print(f"✓ Stream URL: {match['url']}\n")
