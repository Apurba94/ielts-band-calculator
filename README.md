# Band Score Calculator

Turn Listening and Reading raw scores into approximate bands, and work out your overall band with the official rounding rule.

Part of the [IELTS Study Suite](https://github.com/Apurba94/ielts-study-suite): 100 free study apps for IELTS. This one is for the IELTS Academic and General Training test. It works offline, as a Windows program or in the browser.

## Download and run

- **Windows:** download `Band Score Calculator.exe` from the [latest release](https://github.com/Apurba94/ielts-band-calculator/releases/latest) and open it. Nothing to install. It opens in its own window and saves your progress in your user folder.
- **Browser:** open it online in the suite's web edition at https://ielts-study-suite.vercel.app/apps/ielts-band-calculator/ . Progress stays in that browser.
- **From source:** `python launcher.py` (Python 3.10 or later, no packages needed).

## What it does

Turn Listening and Reading raw scores (out of 40) into approximate bands using the guide tables IELTS publishes, and work out an overall band from four skill bands. The overall band is the average rounded to the nearest half band, with averages ending in .25 rounded up to the next half band and .75 up to the next whole band. It also shows how many more correct answers reach the next band.

Sections: Overall, Raw scores, Progress, About.

## How to use it

1. In **Overall**, choose a band for each skill to see the average and the overall band.
2. In **Raw scores**, enter how many answers you got right to see the approximate band.
3. The raw-score tables are approximate: real tests convert slightly differently from version to version.

## Good to know

- All questions, passages, recordings and definitions were written for this suite. None are official IELTS questions. For official practice, use the materials on ielts.org and from the test partners.
- It follows IELTS as delivered on computer in 2026. Formats change, so check ielts.org before your test.
- Listening uses the voices installed on your computer, which sound less natural than real test recordings.
- Feedback on writing and speaking counts what a program can count honestly, such as length and linking words. It is not an IELTS band score. Band conversions for Listening and Reading are approximate.
- Not endorsed by or affiliated with the British Council, IDP or Cambridge University Press & Assessment. IELTS is a registered trademark of its owners.

## For developers

The app is plain HTML and JavaScript in `web/`, run by a small Python launcher that serves it on 127.0.0.1 only and needs a secret token for saving. Tests: `node --test "tests/*.test.js"` (29 tests) and `python -m unittest discover -s tests`. Build the .exe with `python build_exe.py`.

Built with AI assistance (Claude Code). MIT licence. By JANIN A APURBA.
