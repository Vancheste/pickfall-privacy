# Pickfall — Privacy Policy

The privacy policy of the game Pickfall, published at <https://vancheste.github.io/pickfall-privacy/>.

Политика конфиденциальности игры Pickfall.

## Mail / Почта

`mail.json` is the list of letters the game shows in its mailbox; the game downloads it from
<https://vancheste.github.io/pickfall-privacy/mail.json>. To send a letter to every player, add
it to the list and push. `mail.example.json` shows a letter of news and a letter with a gift.

- `id`: a name of its own, never used again (the game remembers a gift taken by it).
- `date`: shown on the letter, `YYYY-MM-DD`. `until` (optional): the letter is gone after that day.
- `title`, `text`: a string, or one per language: `{"en": "...", "ru": "..."}`.
- `gift` (optional): `coins`, `gems`, `chests`, `ore` (`{"copper": 20}`; copper, iron, gold, crystal).

The file must stay valid JSON: a broken file shows the players no new letters.
