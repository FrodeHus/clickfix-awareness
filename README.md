# ClickFix Awareness Training

A browser-based security awareness exercise that teaches people to recognise and stop **ClickFix** phishing attacks. Built for Sopra Steria client training.

**Live page:** https://frodehus.github.io/clickfix-awareness/

## What is ClickFix?

ClickFix is a social-engineering technique where a fake web page (often a "verify you're human" check or a "document won't open" error) convinces you to copy a hidden instruction and paste it into the Windows **Run** box yourself. Because you run the command, no download warning appears and the usual browser protections are bypassed. The result is malware, data theft or ransomware.

## What this page does

The page walks a learner through four stages, in order:

1. **The walkthrough.** The attack from both sides at once. On the left, a fake "verify you're human" page that presents the ClickFix steps (Win+R, Ctrl+V, Enter). On the right, a synced six-step explainer in plain language showing how the trick moves from fake page to full compromise. A **"Play attack step-by-step"** button runs the whole sequence.
2. **Same trick, four masks.** All four lure variants side by side (fake CAPTCHA, fake document, FileFix, external shared file). The cover stories differ completely; the final ask is identical. The point is that people should learn to spot the *ask*, rather than memorise one page.
3. **Quick check.** Three "would you do it?" situations with instant feedback. Two of them are perfectly safe, so nobody leaves thinking the answer is always no.
4. **The lesson.** Red flags, and what to do if it happens to you.

A single takeaway banner sits at the top of the page, and a **FACILITATOR** dropdown in the walkthrough lets a trainer demo any of the four variants in full during a live session.

## Safety

This is a **harmless simulation for education only**. Nothing on the page runs any command or contacts any server:

- The "copied" command is a clearly labelled placeholder that does nothing.
- There are no network calls, downloads, or real clipboard payloads.
- A prominent banner marks the page as a training simulation throughout.

## Files

- `index.html` is the complete, self-contained training page. All HTML, CSS and JavaScript live in one file, with no build step or dependencies.

## Running it

Open `index.html` in any modern browser, locally, from a shared drive, or hosted. It is already deployed via **GitHub Pages** from the `main` branch at the link above.

To host elsewhere, just serve the single file; no server-side code is required.

## Using it in a session

For a sanctioned phishing exercise, keep the page behind access control (intranet / SharePoint / link-with-password) rather than a fully public URL, and always brief participants afterwards so the exercise teaches rather than blames. No one should be penalised for falling for it, or for reporting it.

---

*Sopra Steria Security Awareness Training.*
