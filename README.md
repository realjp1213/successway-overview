# successway-overview
Web app that matches Latin American students to US universities. Live with free and paid tiers. Overview only, code is private. Website: successway.app
# SuccessWay

A mobile-first web app that helps Latin American students find, compare and apply to US universities. Live at [successway.app](https://successway.app) with free and paid tiers since October 2026.

The code lives in three private repos (web app, database builder, matching engine). The matching logic is the core of the product, so it stays private. Happy to walk through it in an interview.

---

## The problem

Students in Latin America who want to study in the US face a confusing process: thousands of institutions, costs that are hard to compare, and advice that is either expensive or biased towards whoever pays the consultant. I ran a consultancy doing this by hand in Bogotá in 2017. SuccessWay is the software version of that service.

## What it does

- A questionnaire that captures what matters to each student (budget, grades, subject, location and more).
- A matching engine that scores each student against a verified database of 1,351 US institutions and returns suitable options.
- Comparison and application guidance in Spanish and English.
- Free, Premium and Premium+ tiers, with payments through Stripe. A consultancy tier for one-to-one help.
- A second channel selling to schools in Colombia.

## How it is built

- **Web app:** Next.js and TypeScript on Vercel
- **Database:** Supabase (PostgreSQL). The institution data is built by a separate pipeline from public sources (IPEDS and others) and verified before it goes in.
- **Matching engine:** Python
- **Payments:** Stripe

Built with AI coding agents (Claude Code). Over 200 releases so far, each tested on a preview site and signed off before going live. A written decision log keeps rules and trade-offs consistent as the product changes.

## How I work on it

- Needs come from students, parents, my co-founder and a user community group.
- Each one becomes a requirement with acceptance criteria before anything is built.
- Small releases, preview first, then production.

  ----
  <img width="1062" height="1876" alt="SuccessWay-github-screenshot-4" src="https://github.com/user-attachments/assets/aa8fbaf9-b1ea-424b-9a2b-a35a4febf0d9" />
<img width="1082" height="4558" alt="SuccessWay-github-screenshot-3" src="https://github.com/user-attachments/assets/48485152-2ade-4e71-9edf-7f2c6f548f40" />
<img width="1066" height="6874" alt="SuccessWay-github-screenshot-2" src="https://github.com/user-attachments/assets/71f24b91-cd73-48b1-a9a4-b0220aabc7c2" />
<img width="1122" height="12096" alt="SuccessWay-github-screenshot-1" src="https://github.com/user-attachments/assets/345c91bb-c007-493c-bd6a-0516aeb75dc0" />
