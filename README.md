# Huginn

**Huginn by Svartalfheim** — a free, single-file, local-first CRM for founder-led
B2B prospecting and cold calling in Norway. One HTML file. No account, no
server, nothing leaves your machine except company lookups against
data.brreg.no.

Named after Odin's raven Huginn ("thought"), who flies out over the world
each morning and comes back to report. The mark is the rune Ansuz (ᚨ), the
rune of speech.

## Bruk / Use

1. Open `huginn.html` in **Chrome or Edge** (Brave works after enabling
   `brave://flags/#file-system-access-api`; Safari and Firefox run in
   browser-storage mode only).
2. Innstillinger → **Velg mappe**: pick a folder on your machine, ideally one
   that is synced or backed up. Huginn writes `huginn-data.json` (source of
   truth), `huginn.xlsx` (the same data as a spreadsheet) and `pitch.json`
   (your call script) there on every change.
3. Press **N** for a new lead. Type a company name or org.nr and Huginn fills
   the rest from Brønnøysundregistrene, including daglig leder and styreleder.
4. **I dag** is your call list. **Ring nå** shows the script with the lead's
   name and your reason spliced in, and one-click outcomes that log the call
   and set the next action.

Norwegian and English UI. Export to xlsx, CSV, JSON, and HubSpot-shaped CSVs.

## What it is not

Not multi-user, not cloud, not a pipeline for thousands of leads. It is the
tool you use before you need a real CRM, and it exports cleanly into one when
you do.

## GDPR

Built in, not bolted on: contact type (named person vs generic address), an
email-consent checkbox with a where/when note, a legitimate-interest note per
lead, a blocker for article 9 categories in notes, a 12-month deletion list,
and a per-lead export for access requests. Cold email to a named person in
Norway needs consent (markedsføringsloven §15); Huginn will tell you so.

## Development

Everything is in `huginn.html`: CSS, a small i18n layer, the xlsx writer and
reader, the Brreg client, and the views. No build step, no dependencies.
Bump `APP.version` when you change behaviour.

## Licence

MIT. See `LICENSE`.

Svartalfheim Solutions AS · [svartalfheim.no](https://svartalfheim.no) ·
hello@svartalfheim.no
