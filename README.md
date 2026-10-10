# Ratna Rajput — Portfolio

Static site. Four pages, no build step, no framework to install.

```
index.html        Start page
who-i-am.html     Who I Am
what-i-do.html    What I Do (case studies)
hire-me.html      Hire Me
assets/           fonts, images, video, and the JS runtime
.nojekyll         tells GitHub Pages to serve files as-is
```

## Editing text

All copy lives as plain text inside the four HTML files. Open one in any
text editor, use Find (Ctrl/Cmd+F), change the words, save, refresh.

## Things still to fill in

Find-and-replace these placeholders:

| File | Find | Replace with |
|---|---|---|
| hire-me.html, what-i-do.html | `hello@example.com` | your real email |
| hire-me.html | `+91 00000 00000` | your phone |
| hire-me.html | `linkedin.com/in/username` | your LinkedIn |
| hire-me.html | `behance.net/username` | your Behance |
| hire-me.html | `20XX — 20XX` / `ADD YOUR DEGREE` / `Institute name, city` | your education |
| hire-me.html | `"resumeUrl":{"editor":"text","default":""` | put the résumé link inside the empty `""` |
| what-i-do.html | `"playStoreUrl":...,"default":""` | Play Store link |
| what-i-do.html | `"arjunNotionUrl":...,"default":""` | Notion case-study link |
| what-i-do.html | `"ndaNotionUrl":...,"default":""` | NDA case-study link |

Two Arjun videos (`arjunIntroVideo`, `arjunWalkthroughVideo`) are empty, which is
why those two boxes show a grey placeholder. Drop the mp4 files into `assets/`
and put `assets/your-file.mp4` inside the empty `""`.

One video still points at an outside host:
`https://ratnaportf-njrqcybn.manus.space/.../popup-desktop-demo_e70aff34.mp4`.
If that host ever goes away the Pop-up desktop video breaks. Download the file,
put it in `assets/`, and swap the URL for `assets/popup-desktop-demo.mp4`.

## Running it locally

Double-clicking `index.html` works, but video behaves better over a local
server. From this folder:

```
python3 -m http.server 8000
```

then open http://localhost:8000
