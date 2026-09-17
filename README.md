# 🐛 Wanna Crack GSoC 3.0 - Bug Hunt

Welcome! This is a small, real-world portfolio website built with plain **HTML + CSS + JavaScript**
across **two pages**: the main portfolio (`index.html`) and a **Blog** page (`blog.html`).

We've planted **20 bugs** in this codebase. Your job is to find them, fix them, and explain each
fix - exactly the kind of work you'll do when contributing to an open-source project during GSoC.

## 🎯 What to do
1. Get the site running locally and click through **both** pages.
2. Hunt down the bugs. Each one shows up as a visible glitch, a broken interaction, a console
   error, or an issue a tool (Lighthouse / the HTML or CSS validator) will flag.
3. Fix each bug **without breaking anything else**.
4. Submit your fixes (PR / patch / diff) with a one-line note per bug: *file, what was wrong, how you fixed it.*

## 🧮 Bug distribution (so you know when you're done)
- **Total bugs: 20**
- By file type: **HTML -> 7**, **CSS -> 6**, **JavaScript -> 7**
- By page: several live on the new **blog.html** page and its script **blog.js** - don't forget to test it.
- By difficulty: **Easy -> 5**, **Medium -> 9**, **Hard -> 6**

## How to run
No build step. Serve the folder (so relative paths behave):

    # Python 3
    python3 -m http.server 8000
    # then open http://localhost:8000

or use the VS Code **Live Server** extension. Opening the files directly also mostly works.

## General hints (no spoilers)
- **Open the DevTools Console.** If a whole chunk of a page's interactivity is dead, there's
  probably a JavaScript error stopping everything after it - fix crashes first.
- **Test at mobile width** and full desktop width. Some features/bugs only appear at one size.
- **Interact with everything, on both pages:** every nav link, the hamburger menu, the
  back-to-top button, the contact form, the blog **filter buttons**, **Read more**, and the
  **newsletter** box.
- **Type into the forms.** A field that looks fine at rest can still be broken.
- **Watch the visuals:** broken images, wrong colours, elements that should move but don't, and
  layouts that don't line up (especially grids on wide screens).
- **Use tooling:** run **Lighthouse** (accessibility) and paste the files into the W3C **HTML
  validator** and **CSS validator** - a couple of bugs are only obvious there.
- **Read carefully:** a single wrong character - in a property name, a class, an id, an
  attribute, a selector, a URL, or a regular expression - is one of the most common real bugs.
- Some JavaScript bugs are about *how the language works* (variable scope, `this`, regex). If a
  handler "kind of works but does the wrong thing," look there.

## Scoring suggestion
- Points per bug for correct identification + a working fix.
- Bonus for a clean fix (introduces no new bug) and a clear explanation of the root cause.

Good luck - go crack it!
