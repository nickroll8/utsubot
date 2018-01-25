# Installing

## Webserver

Preferrably apache2 with php7 and https certificate ( https://www.letsencrypt.org )

## Config

Copy config.php.example and edit (values explained further)

## Log files

Create dir /var/log/tg-bots/ and set it writeable by webserver
edit config.php and set `CONFIG_LOGFILE`

## Bot token

Start chat with https://t.me/BotFather and create bot token.
Enable Inline mode, Allow Groups, Group Privacy off

Use https://www.miniwebtool.com/sha512-hash-generator/ and set `CONFIG_HASH` to hashed value of your token (make sure it is lowecase)

## Database

Create database named for your bot ID (first part of your TG bot token)
Set database password to second part of your TG bot token
Only allow localhost access
Import `utsubot.sql` as default DB structure

## Webhooks

Use https://your-hostname/bot-dir/setup.php

## Google maps API

Get maps API key, and set as `TZ_API_KEY` in your config.

Activate it for both Geocoding and Time Zone API

https://developers.google.com/maps/documentation/timezone/get-api-key
https://developers.google.com/maps/documentation/geocoding/start#get-a-key
