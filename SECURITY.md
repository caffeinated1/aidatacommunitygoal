# Security

## Reporting

Report a vulnerability privately through GitHub's **Report a vulnerability**
button on the Security tab, or by opening an issue if the problem is not
sensitive. Please do not post working exploits in a public issue.

Expect an acknowledgement within a week.

## What is in scope

The published site is static and stores assessment data only in the reader's own
browser. In scope:

- Anything that causes contributed content — an overlay note, an evidence
  headline, a source title — to execute as script in a reader's browser. All
  content is escaped on render; a bypass is a real finding.
- Anything that would send a reader's assessment off their machine. It is meant
  to stay in `localStorage` and go nowhere.
- Anything in `build.py` that would execute contributed data rather than
  validate it.

## What is not

- Content disputes — a wrong figure or a legal statement that does not hold is a
  correction, not a vulnerability. See [CONTRIBUTING.md](CONTRIBUTING.md).
- Denial of service against GitHub Pages, which is not ours to fix.
