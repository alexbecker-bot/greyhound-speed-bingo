# Greyhound Speed Bingo

Party bingo played like a Jackbox game: one screen on the TV, everyone else plays on their phone.

- **TV / big screen:** https://alexbecker-bot.github.io/greyhound-speed-bingo/tv.html — tap "Open a room" to get a 4-letter code.
- **Phones:** https://alexbecker-bot.github.io/greyhound-speed-bingo/ — enter the code and your name (or scan the QR code on the TV).

No accounts needed. Phones can also "Practice on my own" without a TV.

## Self-contained

Everything the game needs is in this repository: the page, the fonts (`vendor/`), the
libraries (`vendor/`) and the recorded caller voices (`audio/`). The only outside service is
the message relay that carries moves between phones and the TV (free public MQTT brokers,
with automatic fallback between three of them), because a static site cannot relay messages
between devices by itself.

## Credits

- Caller voices recorded with [Kokoro-82M](https://huggingface.co/hexgrad/Kokoro-82M) (Apache 2.0): "Heart" (af_heart) and "Barkley" (am_michael, pitched down).
- [MQTT.js](https://github.com/mqttjs/MQTT.js) (MIT) and [QRCode.js](https://github.com/davidshimjs/qrcodejs) (MIT).
- Fonts: [Luckiest Guy](https://fonts.google.com/specimen/Luckiest+Guy) and [Nunito](https://fonts.google.com/specimen/Nunito) (SIL Open Font License).
