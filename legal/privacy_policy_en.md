---
layout: legal
title: Privacy Policy
description: Vestimentum — Privacy Policy (GDPR + CCPA + KVKK)
permalink: /legal/privacy_policy_en/
lang: en
---
# Privacy Policy

**Effective date:** May 25, 2026
**Last updated:** May 25, 2026

This Privacy Policy explains how the Vestimentum mobile application
("**App**", "**Vestimentum**") collects, uses, shares, and protects
your personal data.

Vestimentum is developed by Oğuzcan Özüpek ("**we**", "**us**", "**our**").
This Policy will be updated if Vestimentum is later incorporated as
a legal entity.

For inquiries, contact: **privacy@vestimentum.app**

---

## 1. Scope

This Policy covers all personal data we collect when you use the
Vestimentum mobile application. Data sent to third-party services
outside the App (Cloudinary, Firebase, Anthropic, Open-Meteo, etc.)
is also governed by those parties' own privacy policies (see
Section 4).

If you do not agree with this Policy, please do not use the App.

---

## 2. Data We Collect

### 2.1 Account Data
- **Identity:** Email address (via Firebase Authentication); for Google
  sign-in, your Google account email and name; for anonymous sign-in,
  a synthetic identifier.
- **Profile:** Name (optional), date of birth (optional — for zodiac),
  gender (optional), avatar photo (optional), language preference,
  style preferences.
- **Location:** Approximate coordinates (latitude/longitude). Obtained
  via GPS OR selected from a curated city list. Used for weather
  lookup. We do **not** collect precise / street-level location.

### 2.2 Wardrobe Data
- Photos of clothing items you upload.
- AI-extracted metadata: category (top / bottom / outer / footwear /
  accessory), color, material guess, formality score, style tags,
  season tags.
- Your names, notes, and "last worn" timestamps for each item.

### 2.3 Usage Data
- Outfit suggestions you receive and their context (weather, mood,
  occasion, zodiac context if opted in).
- Outfit history: which you saved, wore, or shared.
- Discover posts: outfit illustrations (abstract line art, **not** your
  real photos), captions, likes.
- Subscription state (Free / Vestimentum+) and history.

### 2.4 Technical Data
- **Crash reports** via Sentry: anonymous device info, stack traces.
  No PII. Only active when `SENTRY_DSN` is configured (production).
- **IP address:** Transiently visible to Firebase Authentication during
  token verification; we do not persist it.
- **Device info:** App version, OS version, device model (only in
  crash reports).

### 2.5 What We Do **Not** Collect
- **Behavioral tracking:** Advertising IDs, cross-app tracking, browse
  history — none.
- **Sensitive data:** Health, biometric, financial account numbers,
  political / religious views, sexual orientation, ethnicity — none.
- **Precise location:** Street-level GPS — not collected.
- **Messaging content:** None today (this section will be updated
  when comments are added in a future release).

---

## 3. How We Use Your Data

We use collected data only for the following purposes:

| Purpose | Legal basis (GDPR Art. 6 / KVKK §5) |
|---|---|
| Create and manage your account | Performance of contract |
| Generate AI outfit suggestions | Performance of contract |
| Look up weather based on your location | Contract + legitimate interest |
| Zodiac-influenced suggestions (opt-in) | Explicit consent (premium toggle) |
| Show your posts to other users on Discover | Explicit consent (share action) |
| Diagnose app crashes (Sentry) | Legitimate interest |
| Subscription billing records | Contract + legal obligation |
| Comply with GDPR/KVKK obligations (erasure requests, etc.) | Legal obligation |

**What we don't do:**
- We do not sell your data for advertising.
- We do not share behavioral data with advertising networks.
- We do not perform automated profiling that produces legal effects.
- We do not send marketing newsletters (only transactional notifications:
  account security, subscription state).

---

## 4. Third-Party Services

For Vestimentum to function, some data is shared with the providers
below. Each processes your data under its own privacy policy.

### 4.1 Firebase (Google LLC) — Authentication
- **Data shared:** Email, password hash, session tokens, IP (transient).
- **Location:** US data centers (Standard Contractual Clauses apply).
- **Privacy policy:** https://firebase.google.com/support/privacy

### 4.2 Cloudinary (Cloudinary Ltd.) — Image Hosting
- **Data shared:** Your clothing photos and avatar, generated
  thumbnails.
- **Location:** US/EU data centers.
- **Privacy policy:** https://cloudinary.com/privacy

### 4.3 Anthropic (Anthropic PBC) — AI Processing (Claude)
- **Data shared:** Clothing photos (for classification), outfit
  suggestion context (weather, mood, wardrobe summaries).
- **Location:** US data centers.
- **Note:** Anthropic does not use API data to train its models.
- **Privacy policy:** https://www.anthropic.com/legal/privacy

### 4.4 remove.bg (Kaleido AI GmbH) — Background Removal
- **Data shared:** Original clothing photo (transient processing).
- **Location:** EU.
- **Retention:** Photos are deleted by remove.bg after processing,
  per their policy.
- **Privacy policy:** https://www.remove.bg/privacy

### 4.5 Open-Meteo — Weather Data
- **Data shared:** Only latitude/longitude coordinates. No personal
  identifiers are sent.
- **Location:** Germany.
- **Privacy policy:** https://open-meteo.com/en/terms

### 4.6 Sentry (Functional Software, Inc.) — Crash Reporting
- **Data shared:** Stack traces, device type, app version. No PII
  (`sendDefaultPii=false` enforced).
- **Location:** US/EU.
- **Only active in production configurations.**
- **Privacy policy:** https://sentry.io/privacy

### 4.7 App Stores

#### 4.7.1 Apple App Store (Apple Inc.)
- **Data shared:** Subscription identifier (anonymous purchase
  token), billing records, IP address, Apple ID (user-facing; we
  do not see this identifier).
- **Location:** US / European data centers (Apple's own policy).
- **Privacy policy:** https://www.apple.com/legal/privacy/

#### 4.7.2 Google Play (Google LLC)
- **Data shared:** Subscription identifier (anonymous purchase
  token), billing records, IP address, Google Play account
  (user-facing; we do not see this identifier).
- **Location:** Global data centers.
- **Privacy policy:** https://policies.google.com/privacy

---

## 5. Data Retention

- **Active account data:** Retained until you delete your account.
- **When your account is deleted:** All personal data is permanently
  removed from servers within 30 days. The database row is purged
  immediately when you tap "Delete account"; backup purges can take
  up to 30 days.
- **Cloudinary photos:** When you delete your account, all Cloudinary
  assets including your profile photo and garment images are deleted
  within 30 days.
- **Logs (Sentry / server logs):** Automatically deleted after 90 days.
- **Legal retention:** Billing records may be retained up to 10 years
  due to tax-law obligations (e.g., Turkish Tax Procedure Law).

---

## 6. Where Data Is Stored & International Transfers

Vestimentum's production infrastructure is not yet live; once the
production environment goes live, servers will be hosted in **EU
data centers** (Fly.io or Railway EU region). Some third-party
services (Firebase, Anthropic) process data in the **US**. These
transfers rely on **Standard Contractual Clauses (SCCs)** under
GDPR Chapter V and KVKK Article 9.

---

## 7. Your Rights

### 7.1 Under GDPR (EU Residents)
Under GDPR Articles 15-22, you have the right to:

- **Access** — request a copy of your data.
- **Rectification** — correct inaccurate data.
- **Erasure ("right to be forgotten")** — delete your data.
- **Restriction of processing** — pause processing in specific cases.
- **Portability** — receive your data in a structured format.
- **Object** — to processing based on legitimate interest.
- **Withdraw consent** — opt out of consent-based processing (e.g.,
  the zodiac toggle) at any time.
- **Lodge a complaint** with your local data protection authority.

### 7.2 Under KVKK (Turkish Citizens)
Under KVKK Article 11, you additionally have the right to:

- Learn whether your data is being processed
- Request information about processing
- Learn about the purpose and whether it matches the actual use
- Know which third parties (domestic / international) receive your data
- Have incomplete / incorrect data corrected
- Request deletion or destruction
- Have correction/deletion notified to onward third parties
- Object to a result derived purely from automated analysis that
  affects you adversely
- Seek compensation for damages arising from unlawful processing
- Request that your data be provided to you in a structured, commonly
  used, machine-readable format (consistent with KVKK Board guidance
  interpretation)

### 7.3 Under CCPA (California Residents)
Under CCPA, you additionally have the right to:

- **Know** — what categories of data we collect, for what purposes.
- **Delete** — same flow as Section 7.4.
- **Opt out of "sale"** — Vestimentum **does not sell** personal data
  (no "sale" exists under CCPA definitions).
- **Non-discrimination** — we will not treat you differently for
  exercising your rights.

### 7.4 How to Exercise Your Rights

**Easiest — in the app:**
- Profile → "Delete my account" → all your data is removed.
- Download my data: write to privacy@vestimentum.app to request a
  copy of your data in JSON format.
- Use the profile settings for other changes.

**By email:**
- Write to privacy@vestimentum.app from the email associated with
  your account so we can verify identity.
- Response time: within 30 days (KVKK), with possible 1-month
  extension (GDPR).

---

## 8. Children's Privacy

Vestimentum is **not intended for children under 13.** If you provide
a date of birth during registration, the system automatically rejects
DOBs that imply under-13. By using the App without providing a DOB,
you represent that you are 13 or older.

If we discover that we have collected data from a child under 13, we
will delete the account immediately. If you believe your child is
using Vestimentum, please write to privacy@vestimentum.app.

---

## 9. Security

Measures we take to protect your data:

- **In transit:** All client–server traffic uses HTTPS / TLS 1.2+.
- **Authentication:** Session handling via Firebase Authentication;
  passwords are hashed by Firebase with bcrypt-class algorithms —
  we never see your password.
- **Access control:** Only operationally necessary personnel can
  access the database.
- **At rest:** Database-level Transparent Data Encryption (TDE);
  Cloudinary encrypts assets at rest with AES-256 by default.
- **Monitoring:** Sentry observes anomalous behavior (production
  only).

No system is 100% secure. In the event of a breach, we will notify
the relevant authorities within 72 hours per KVKK Data Breach
Notification regulations and GDPR Articles 33-34, and affected users
without undue delay.

---

## 10. Cookies and Tracking

Vestimentum is a **mobile app** and does not use browser cookies. We
also do not use:

- Third-party analytics (Google Analytics, Mixpanel, etc.)
- Advertising identifiers (IDFA, AAID)
- Social media tracking pixels
- Cross-app behavioral tracking

If in-app analytics are added later, this Policy will be updated and
opt-out will be offered.

---

## 11. Changes to This Policy

If we update this Policy:

- **Material changes** (e.g., new data categories, new third parties,
  changes to your rights): We will display an in-app banner and
  announce the effective date at least 14 days in advance.
- **Minor changes** (typos, third-party link updates): Silently
  updated; the "Last updated" date is refreshed.

We recommend you periodically review this page.

---

## 12. Contact

For questions or requests about this Policy:

- **Email:** privacy@vestimentum.app
- **Data Controller / Veri Sorumlusu:** Oğuzcan Özüpek (individual
  data controller / gerçek kişi) — İzmir, Türkiye
  (privacy@vestimentum.app — to be updated after incorporation)

If you are not satisfied with our response to a KVKK request, you may
file a complaint with the Turkish Personal Data Protection Authority:
https://www.kvkk.gov.tr

For GDPR complaints, contact your local data protection authority:
https://edpb.europa.eu/about-edpb/about-edpb/members_en

---

*This Privacy Policy was prepared with reference to KVKK (Turkish Law
No. 6698), GDPR (EU 2016/679), CCPA (Cal. Civ. Code §1798.100 et seq.),
and Google Play / Apple App Store requirements. It is not a substitute
for formal legal advice; review by a lawyer is recommended before
production launch.*
