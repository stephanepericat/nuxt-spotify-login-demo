# nuxt-spotify-login-demo

A demo showing how to authenticate against the [Spotify API](https://developer.spotify.com/) in a [Nuxt.js](https://nuxtjs.org/) application.

## Installation

```bash
yarn install --immutable
```

## Setup

Create a `.env` file at the root of the project, and add the following properties:

```
SPOTIFY_CALLBACK_URL=http://localhost:3000/callback
SPOTIFY_CLIENT_ID=YOUR_SPOTIFY_CLIENT_ID
SPOTIFY_LOGIN_URL=https://accounts.spotify.com/authorize
SPOTIFY_TOKEN_URL=https://accounts.spotify.com/api/token
SPOTIFY_USER_URL=https://api.spotify.com/v1/me
```

Replace `YOUR_SPOTIFY_CLIENT_ID` with the ID you can get from the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications).

## Run

```bash
yarn dev
```
