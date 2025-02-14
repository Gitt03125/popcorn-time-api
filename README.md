# Popcorn Time API ![Version](https://img.shields.io/badge/Version-v0.0.2-orange?style=flat-square&url=https://github.com/DEADSEC-SECURITY/popcorn-time-api/blob/main/CHANGELOG.md) ![Python_Version](https://img.shields.io/badge/Python-3.7%2B-blue?style=flat-square) ![License](https://img.shields.io/badge/License-MIT-red?style=flat-square) ![Donate](https://img.shields.io/badge/Donate-Crypto-yellow?style=flat-square) [![CodeQL](https://github.com/DEADSEC-SECURITY/popcorn-time-api/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/DEADSEC-SECURITY/popcorn-time-api/actions/workflows/codeql-analysis.yml)

## 📝 CONTRIBUTIONS

Before doing any contribution read <a href="https://github.com/DEADSEC-SECURITY/popcorn-time-api/blob/main/CONTRIBUTING.md">CONTRIBUTING</a>.

## 📧 CONTACT

Email: amng835@gmail.com

General Discord: https://discord.gg/dFD5HHa

Developer Discord: https://discord.gg/rxNNHYN9EQ

## 📥 INSTALLING
<a href="https://pypi.org/project/popcorn-time">Latest PyPI stable release</a>
```bash
pip install popcorn-time
```

## ⚙ HOW TO USE
```python
from popcorntime import PopcornTime
popAPI = PopcornTime()
```

## 🤝 PARAMETERS
### CLASS PARAMETERS
- debug : bool, optional
  - Enable for debug mode (Default: False)
- min_peers : int, optional
  - Minimum number of peers to select torrent (Default: 0)
- min_seeds : int, optional
  - Minimum number of seeds to select torrent (Default: 0)
### FUNCTION PARAMETERS
- #### FUNCTION `set_logging_level`
  - level : int, required
    - Set the logging level
    - Accepted values:
      - 0: DEBUG
      - 1: INFO
      - 2: WARNING
      - 3: ERROR
      - 4: CRITICAL
      - 5: NOTSET
- #### FUNCTION `set_base_url`
  - url : str, required
    - Set the base url for the API
- #### FUNCTION `set_base_url`
  - url : str, required
    - Set the base url for the API
- #### FUNCTION `set_min_seeds`
  - value : int, required
    - Minimum number of seeds to select torrent
- #### FUNCTION `set_min_peers`
  - value : int, required
    - Minimum number of peers to select torrent
- #### FUNCTION `get_shows_page`
  - page : (int, str), required
  - Returns the shows page in json format
- #### FUNCTION `get_movies_page`
  - page : (int, str), required
  - Returns the movies page in json format
- #### FUNCTION `get_show`
  - show_id : (int, str), required
    - IMDB ID of the show
  - Returns the show data in json format
- #### FUNCTION `get_movie`
  - movie_id : (int, str), required
    - IMDB ID of the movie
  - Returns the movie data in json format
- #### FUNCTION `get_best_quality_torrent`
  - torrents : dict, required
    - The dictionary of torrents provided by the API (get_show or get_movie)
  - Returns the best quality torrent is json format
