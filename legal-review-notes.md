# Stella — Points for Legal Review

**Do not publish this file.** It is an internal note listing the questions to put to a lawyer or company secretary before Stella takes payment from users.

The published Privacy Policy and Terms of Service are drafts prepared without legal review. They are considered adequate for a Play Console listing and closed testing, but should be reviewed before public launch or before charging users.

---

## Priority 1 — before charging users

**1. Entity status and personal liability.**
Northpath is currently a trading name and domain, not a registered company. Until an entity is incorporated, the individuals operating Stella are the Data Fiduciaries under the DPDP Act, 2023, and bear personal responsibility. Both published documents name "Northpath" and must be updated on incorporation. Ask: what is the exposure in the interim, and does incorporation need to precede taking payment?

**2. Medical positioning.**
Stella targets users who struggle with focus and starting tasks, and collects behavioural and self-reported state data. The Terms disclaim any medical purpose. Ask: are the disclaimers sufficient given the app's positioning and target audience, and could any feature be construed as health-related processing under DPDP or as a medical device claim?

Note: disclaimers in the Terms do not cure a medical claim made in advertising. All Meta ad copy, Play Store listing text, and onboarding copy must be consistent.

**3. Cross-border transfer to a China-based provider.**
Task text is sent to DeepSeek, which is based in China. Voice audio is sent to Groq. The DPDP Act permits the Government to restrict transfers to specified countries by notification. Ask: what is the current notification status, and what is the exposure if a restriction is introduced after launch?

Business continuity note: an alternative provider (e.g. GPT-4o mini) should remain switchable in the implementation.

**4. Age assurance.**
Stella is 18+ by declaration. Under the DPDP Act a child is anyone under 18, and processing children's data without verifiable parental consent carries a penalty ceiling of up to ₹200 crore. The Act also restricts behavioural monitoring directed at children — and behavioural monitoring (app usage, notification access, screen on/off) is central to how Stella works. Ask: is a self-declared 18+ gate adequate assurance given the nature of the monitoring?

**5. Subscription and consumer protection.**
Auto-renewal, trial-to-paid conversion, cancellation, and refund terms should be checked against Indian consumer protection law. Ask: are the disclosures adequate, and is the auto-renewal consent mechanism compliant?

**6. Limitation of liability.**
The clause caps liability at amounts paid in the preceding twelve months. Indian courts read such clauses narrowly and some liabilities cannot be excluded. Ask: is the drafting enforceable, and what should be carved out?

---

## Priority 2 — accuracy checks (internal, not legal)

These are factual claims in the published policy that must remain true. Re-verify whenever the implementation changes.

**Deletion.** The policy states that personal data is deleted immediately on account deletion. Confirmed by Sameer. This must be verified as working before publication, and re-verified if the deletion flow changes.

**Data minimisation to AI providers.** The policy states that no name, phone number, email, user ID, or check-in data is sent to DeepSeek or Groq — only task text and voice audio. Confirmed by Sameer. If any identifier is later attached to these calls, the policy becomes inaccurate and must be corrected.

**Third-party retention.** Deletion promises cover Northpath's own systems. AI providers may retain data on their side under their own terms. Section 7 of the policy carries a caveat covering this. Do not represent to users that deletion reaches inside third-party systems.

**Play Data Safety form.** The declarations in Play Console must exactly match Section 2 of the Privacy Policy. Mismatches are a common cause of listing rejection and of regulatory complaint.

---

## Regulatory timeline context

The DPDP Rules, 2025 were notified on 13 November 2025 with a staggered implementation runway:

- **13 November 2025** — Data Protection Board provisions in force; complaints can be filed.
- **13 November 2026** — Consent Manager provisions take effect.
- **13 May 2027** — Substantive compliance obligations fully enforceable.

Soft enforcement and guidance are expected through 2026. Early Data Protection Board actions have targeted app developers processing data without valid consent, so consent flow quality is the practical priority.
