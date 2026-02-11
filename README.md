# Valentine

![demo](https://github.com/SrlLiu/Valentine/blob/main/demo/demo.gif)

## Run locally

1. From the project root, start a static server:
   ```bash
   python3 -m http.server 8000
   ```
2. Open [http://localhost:8000](http://localhost:8000) in your browser.
3. Navigate to:
   - Top prompt: click `Yes`/`No` on the Valentine question.
   - Click `Yes` to open the Valentine card with the title `Happy Valentine Day`, rose gif, and character-by-character “這段時間，跟妳一起相處的時光，我一直都很珍惜。” text.

## Manual verification checklist

- Boundaries:
  - Confirm the Valentine card keeps a 5:7 frame without overflowing on desktop and mobile widths.
  - Confirm the `Happy Valentine Day` title remains centered and does not overflow the card frame.
  - Confirm the rose GIF stays visually contained within the card during subtle floating motion.
  - Confirm text reveals one character at a time from empty to `這段時間，跟妳一起相處的時光，我一直都很珍惜。`.
  - Confirm after full message appears, it briefly holds, resets to empty, and repeats.
  - While hovering `No`, confirm it stays inside the prompt area and does not leave the card.
