# How to add a new piece

Everything happens on github.com in your browser. There's nothing to install. Each piece is one file in the **`_pieces`** folder.

## The steps

1. Go to **github.com/barrybarneswriting/barrybarneswriting.github.io**. Make sure you're signed in.
2. Click the **`_pieces`** folder.
3. Near the top right, click **Add file**, then **Create new file**.
4. In the box at the top, type a file name for the piece. Use lowercase, put hyphens instead of spaces, and end it with `.md`. For example: `the-long-goodbye.md`. The file name becomes the piece's web address (`…/pieces/the-long-goodbye/`), so choose it carefully.
5. In the big text area, paste this template, then fill it in:

   ```
   ---
   title: "The Title of Your Piece"
   date: 2026-11-20
   section: fiction
   subtitle: "An optional italic line under the title. Delete this line if you don't want one."
   ---

   Your first paragraph goes here.

   Your second paragraph goes here. Leave one blank line between paragraphs.
   ```

   - **title:** keep the quotation marks around it.
   - **date:** must be written as year-month-day, like `2026-11-20`. Pieces are sorted by this date, newest first.
   - **section:** write either `fiction` or `essays`, all lowercase. Nothing else will work.
   - **subtitle:** optional. If you include it, it also becomes the short excerpt on the listing pages. If you leave it out, the excerpt is the first few lines of the piece.
   - The two `---` lines have to stay exactly as they are.

6. Paste your piece below the second `---`.
7. Click the green **Commit changes…** button. In the box that pops up, leave the defaults and click **Commit changes** again.
8. Wait one to two minutes, then reload your site. The new piece will be on the home page and on its section page. If you want to watch the progress, click the **Actions** tab at the top of the repository. A green check means the site is live.

## Formatting cheat sheet

| What you want | What to type |
|---|---|
| A new paragraph | Leave one blank line between paragraphs |
| *Italics* | Put an asterisk on each side: `*like this*` |
| A section break | A line containing only `* * *`, with a blank line above and below |

The site handles curly quotes and apostrophes. You can paste text from Word, Google Docs, or Substack without changing anything.

**One quirk.** A paragraph that *starts* with a number and a period (like `1999. That was the year…`) or with `#`, `-`, `>`, or `+` can be read as a heading or a list. To prevent that, type a backslash before the character: `1999\. That was the year…`

## Fixing or deleting a piece

- **To fix a typo:** open the piece's file in `_pieces`, click the pencil icon (✏️), make the change, then click **Commit changes**.
- **To remove a piece:** open its file, click the **⋯** menu at the top right, choose **Delete file**, then commit. Deleted files can be restored from the repository's history, but doing that is fiddly, so be sure before you delete.

## Other easy changes

- **The one-line description on the home page:** open `_config.yml`, click the pencil, and edit the text in quotes after `description:`.
- **Your Substack link:** same file, the `substack_url:` line.
- **The About page:** open `about.md`, click the pencil, and write your text below the second `---`.
