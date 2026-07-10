# Field Guide: Solving a Duplicate Payment

An interactive walkthrough of Antithesis's deterministic simulation testing platform.

## What this is

A single self contained HTML file that teaches deterministic simulation testing the way I actually learned it: one concept at a time, framed as investigating a real bug rather than reading documentation. Every chapter states the idea plainly first, then applies it to a running example, a payment service that occasionally charges a customer twice, clearly labeled as one illustrative case, not a real customer or a real incident.

## Why I built it

Antithesis's own engineering blog notes that the real obstacle for customers isn't understanding the platform, it's translating their own system into a property: "this sounds great, but what properties should my system have?" That's the actual bottleneck a Solutions Engineer works against. This guide is a prototype of the kind of resource I'd want to hand a customer's engineering team on day one of onboarding, built to close that exact gap rather than restate the marketing copy.

## What's inside

1. **The Bug** — why the hardest bugs are the ones nobody imagined testing for
2. **Package Your System** — why Antithesis needs the whole system as containers, not one service in isolation
3. **The Determinator** — Antithesis's own name for its deterministic hypervisor, and why controlling timing is the whole trick
4. **Same Seed, Same Bug** — a live demo where the replay result genuinely depends on the seed you type in
5. **Fault Injection** — an interactive panel showing what each fault actually breaks and why
6. **Properties, the Laws of the System** — includes the method for deriving properties from any system, not just the example, with working examples across payments, blockchain, and database verticals
7. **The Pipeline** — the real five step workflow, animated end to end
8. **Triage Report** — the case closed out using the platform's real reporting fields

## How to view it

Open `field-guide.html` in any browser. No install, no server, no internet connection required after the fonts load. All interactions (seed replay, fault injection, property tabs, pipeline animation, recording demo) are fully functional.

## A note on accuracy

Product terminology (the Determinator, Triage Report, Copy Moment, Always and Sometimes properties) is pulled directly from Antithesis's own documentation and engineering blog, not invented for this guide. The duplicate payment case is a constructed teaching example.

---
Built by Siwoo (Reese) Yoon
