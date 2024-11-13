# Retep Spotify

<br>
<div align="center">

![language](https://img.shields.io/github/languages/top/th3-riddler/Retep-Spotify?style=for-the-badge&logo=python&color=blue)
![GitHub](https://img.shields.io/badge/github-000000?style=for-the-badge&logo=github)
![OS](https://img.shields.io/badge/linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Spotify](https://img.shields.io/badge/Spotify-40a02b?style=for-the-badge&logo=spotify&logoColor=white)

</div>
<br>

Retep Spotify is a simple **Spotify Controller** that allows you to interact with your Spotify playback from the terminal and it's thought to make it easier to control with some keyboard shortcuts.

## Installation
In order to use Retep Spotify you need to install all the dependencies written in the `requirements.txt` file in a Python virtual environment. You can do this by running the following commands:
### Create the virtual environment and activate it
```bash
python -m venv .venv
source .venv/bin/activate
```
> make sure to replace `#!.venv/bin/python3` at the top of the `Retep` file with the path to your virtual environment's python executable.
### Install the dependencies
```bash
pip install -r requirements.txt
```
## Usage
To use Retep Spotify you have to create a [Spotify Developer App](https://developer.spotify.com/) and get the `Client ID` and `Client Secret` from the Spotify Developer Dashboard. Once you have them you can create a `.env` file in the root of the project and add the following lines:
```bash
SPOTIFY_CLIENT_ID=<your_client_id>
SPOTIFY_CLIENT_SECRET=<your_client_secret>
SPOTIFY_REDIRECT_URI=http://localhost:8888/callback
```
To use Retep Spotify you need to make `Retep` file executable if it's not already:
```bash
chmod +x Retep
```
And then you can run it with:
```bash
./Retep [option]
```
For more information about `option` type:
```bash
./Retep -h
```
or
```bash
./Retep --help
```
