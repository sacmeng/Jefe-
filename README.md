# Jefe: Voice Estimate Maker

**Walk the job, talk it through, and send a finished estimate.**

Jefe is an iPhone app for people in the trades. You record yourself walking a job site, and Jefe turns what you said into a clean estimate, invoice, work order or report.

[**Download on the App Store →**](https://apps.apple.com/us/app/jefe-voice-estimate-maker/id6761315709)

<!-- TODO: add 3-4 screenshots to a /screenshots folder in this repo, then keep or rename the files below. -->
<p>
  <img src="screenshots/01-record-walk.png" alt="Recording a site walk" width="200">
  <img src="screenshots/02-line-items.png" alt="Line items pulled from the walk" width="200">
  <img src="screenshots/03-estimate.png" alt="Finished estimate" width="200">
</p>

> This repo is a public overview of the product. The app's source code lives in a private repository in the [damsac](https://github.com/damsac) organization.

---

## The problem

<!-- TODO: this section is my framing, not from your resume. Replace it with what you actually heard from contractors. -->
Contractors size up a job by walking it: looking at the space, measuring, and talking with the client. Then they go home and write it all up. That write-up happens at night, from memory, and it is slow. Estimates go out late, details get missed, and jobs are lost to whoever quoted first.

## What Jefe does

1. **Record the walk.** Talk through the job the way you already do while you walk it.
2. **Get organized notes.** Jefe pulls out the line items and quantities and groups them into notes.
3. **Fix what's missing.** Anything without a price or quantity is flagged for you to fill in. Jefe doesn't guess.
4. **Send the document.** Turn the notes into an estimate, invoice, work order or report with your business details on it.
5. **Keep it with the job.** Each walk is filed under its job, along with your photos.

Built for landscaping, plumbing, electrical, HVAC, home inspection and similar trades.

## My role

**Co-founder & Product Lead** (January 2026 – present)

I own the product: what we build, how it looks and works, how it's priced, and how we get it in front of contractors.

- Took Jefe from beta to a production App Store release, shipping **100+ builds in 5 weeks**. Launched on the App Store in **October 2026**.
- Led UI/UX design, translating how people in the trades actually work into features that make sense to them.
- Designed pricing and built subscription billing, usage limits and a free tier to turn the beta into a paid product.
- Run go-to-market through paid ads, the App Store and contractor groups, and track App Store views through paid conversion weekly to decide where to spend on ads.

## Product decisions

<!-- TODO: check each "why" below and rewrite it in your own words if the real reason was different. -->

**Audio never leaves the phone.**
Speech-to-text runs on the device, so the recording itself stays on the phone. An LLM then turns the transcript into line items.
*Why:* contractors are recording inside clients' homes and businesses. Keeping the audio on the phone makes that an easy yes.

**Flag it, don't guess it.**
When a price or quantity is missing or unclear, Jefe marks it instead of filling in a plausible number.
*Why:* a wrong number on an estimate costs a contractor money or credibility. A visible blank costs them five seconds.

**Talk first, type later.**
The core input is a voice recording made while walking the site, not a form.
*Why:* that's how the work already happens. People in the trades rarely want to type on a phone at a job site.

**A free tier before the paywall.**
New users get their first walks free before subscribing monthly or yearly.
*Why:* contractors need to see one real estimate come out of their own walk before they'll pay for it.

## Making it reliable in the field

Job sites are hard on a phone app. Recent releases focused on what breaks in the real world:

- Recordings survive interruptions from phone calls.
- Recording recovers from Bluetooth or headset disconnects and microphone drops.
- The app reconnects to the server when a walk starts on a weak connection.
- Error messages say clearly when a document failed or an edit wasn't saved.

## Tech at a glance

- iPhone app (iOS 17 or later)
- On-device speech-to-text
- An LLM that turns transcripts into structured line items and flags uncertain ones
- Subscription billing with usage metering and a free tier

<!-- TODO: add the main frameworks and services you use (for example SwiftUI, your backend, your LLM provider, StoreKit), only if you're comfortable sharing them. -->

## Team

- **Isaac Wallace-Menge**, Co-founder & Product Lead · [LinkedIn](https://www.linkedin.com/in/isaac-wallace-menge/) · [GitHub](https://github.com/sacmeng)
- <!-- TODO: co-founder name, role and link --> Co-founder

## Links

- [Jefe on the App Store](https://apps.apple.com/us/app/jefe-voice-estimate-maker/id6761315709)
- <!-- TODO: your personal site link once it's live -->
