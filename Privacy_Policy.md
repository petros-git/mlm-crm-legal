---
permalink: /privacy/
---

# Privacy Policy

**Effective Date:** 16 May 2026

**Last Updated:** 16 May 2026

This Privacy Policy describes how DialDay ("the Application", "we", "us", or "our") collects, uses, stores, and shares your personal data. The Application is operated by Petros Chatzianastasiou ("Service Provider"), based in Greece (European Union), and is provided as a Freemium service.

By downloading, installing, or using DialDay, you agree to the practices described in this Privacy Policy.

---

## 1. Data Controller

The data controller responsible for your personal data is:

**Petros Chatzianastasiou**
Greece
Email: petros.canon@gmail.com

If you have any questions about this Privacy Policy or wish to exercise your rights under GDPR, you can contact us at the email address above. As a solo operator, we are not required to appoint a dedicated Data Protection Officer under GDPR Article 37; the Data Controller above handles all privacy inquiries directly.

---

## 2. What Information We Collect

### 2.1 Account Information

When you create an account, we collect:
- Email address (for authentication and account recovery)
- Password (stored hashed via Supabase Auth — we never see your plaintext password)
- First name and last name
- Country
- Phone number (optional)
- Organization name and role (optional, for industry context)

### 2.2 CRM Data You Create

The Application is a customer relationship management tool. You provide and we store:
- Contact records (names, phone numbers, email addresses, notes, tags, status, lead source, birthday)
- Call logs (date, duration, outcome, notes)
- Activities and conversions
- Cadences and scheduled tasks
- Daily call goals and progress

This data belongs to you. We process it solely to provide the Application's features.

### 2.3 Phone Contacts (with your permission)

If you grant the Application permission to access your device contacts, the Application syncs your phone book into your CRM:
- Names, phone numbers, and email addresses from your device contacts
- Internal contact identifiers from your device (used to detect updates and removals)

You can revoke contacts permission at any time through your device settings. Doing so will stop further syncing but will not automatically delete previously synced contacts from the Application — you can delete them manually from within the Application.

### 2.4 Subscription Information

If you subscribe to DialDay Pro:
- Subscription status and billing period (managed via RevenueCat)
- Anonymous transaction identifiers from Apple App Store or Google Play
- We do not see, store, or process your payment card details. All payment processing is handled by Apple App Store or Google Play.

### 2.5 Microphone & Speech Recognition (optional)

If you use voice features to dictate notes:
- The Application requests microphone access and speech-recognition permission via your device's operating system.
- Audio is processed by the operating system's on-device speech-recognition service (Apple Speech Recognition on iOS, Android SpeechRecognizer on Android). The resulting transcript is returned to the Application locally.
- Raw audio is not transmitted to our servers, and we do not store recordings. Only the resulting text — once you save the note — is stored as part of your CRM data.
- These permissions are optional; the Application functions without them. You can revoke them at any time via your device settings.

### 2.6 AI-Assisted Features (Pro)

DialDay offers optional AI-assisted features (objection coach, message drafter, transcript parsing, weekly digest). When you invoke one of these features:
- The text you submit — and, for the weekly digest, summary statistics derived from your CRM data — is sent to **OpenAI, L.L.C.** (USA) for processing as a sub-processor on our behalf.
- Per OpenAI's API data usage policy, inputs and outputs are not used to train OpenAI's models.
- This transfer is from the European Economic Area to the United States; we rely on Standard Contractual Clauses for the lawful basis of transfer.
- We recommend you do not paste highly sensitive third-party personal data into AI inputs.
- AI features only activate when you explicitly invoke them, and require an active Pro subscription.

### 2.7 Push Notification Tokens (optional)

If you enable notifications:
- Your device's Apple Push Notification service (APNs) or Firebase Cloud Messaging (FCM) token is stored in our database, linked to your account, and used solely to deliver reminders you have scheduled within the Application.
- Apple and Google operate the push delivery infrastructure. We do not send notification content through any third party other than Apple's / Google's push services themselves.
- You can disable notifications at any time via your device settings.

### 2.8 Information We Do NOT Collect

For transparency, the Application does NOT collect:
- Your precise device location (no GPS access)
- Your camera, photos, or videos
- Your web browsing history outside the Application
- Biometric or health data
- Behavioral profiling data for advertising

The Application contains no advertising and does not share your data with advertising networks.

---

## 3. How We Use Your Information

We process your personal data for the following purposes:

| Purpose | Lawful Basis (GDPR) |
|---|---|
| Provide CRM functionality (store and display your contacts, call logs, activities) | Contract performance |
| Authenticate your account and prevent unauthorized access | Contract performance |
| Sync device contacts when you grant permission | Contract performance and your consent |
| Process subscription purchases and manage Pro entitlements | Contract performance |
| Deliver AI-assisted features when you invoke them | Contract performance and your consent |
| Send essential service notifications (e.g., account changes, important updates) | Legitimate interest |
| Send push reminders you have scheduled | Contract performance and your consent |
| Crash reporting and error diagnostics (production builds only) | Legitimate interest (security, stability) |
| Comply with legal obligations | Legal obligation |
| Investigate and prevent fraud or abuse | Legitimate interest |

We do not use your personal data for marketing communications. We do not sell your personal data to anyone, ever.

---

## 4. Where Your Data Is Stored

We engage the following sub-processors under written Data Processing Agreements compliant with GDPR Article 28:

- **Supabase, Inc.** (Delaware, USA). Your data is stored in Supabase's EU-North (Stockholm) region. Acts as our backend database, authentication, and storage provider. Supabase may access data from its US offices in limited support and security scenarios; this transfer is covered by Standard Contractual Clauses.
  See Supabase's Privacy Policy: [https://supabase.com/privacy](https://supabase.com/privacy)

- **RevenueCat, Inc.** (California, USA)
  Manages subscription state and validates Pro entitlements. Receives a pseudonymous app user identifier (your DialDay account UUID), subscription status, and the platform transaction ID. Does not receive your name, email, or CRM data.
  <!-- MAINTENANCE NOTE: the data-minimization claim above assumes RevenueCat appUserID is wired to the Supabase user UUID, not the user's email. If that wiring ever changes, this paragraph and the §16 mapping must be updated in lockstep. -->
  See RevenueCat's Privacy Policy: [https://www.revenuecat.com/privacy](https://www.revenuecat.com/privacy)

- **Sentry** (Functional Software, Inc., California, USA)
  Receives crash reports and error diagnostics from production builds only (transmission is disabled in development). Data sent includes device model, OS version, app version, stack traces, and a pseudonymous user identifier. Sentry does not receive your name, email, CRM data, or contact information. Cross-border transfer to the US is covered by Standard Contractual Clauses.
  See Sentry's Privacy Policy: [https://sentry.io/privacy/](https://sentry.io/privacy/)

- **OpenAI, L.L.C.** (California, USA)
  Processes inputs to AI-assisted features (see §2.6) on our behalf. Inputs and outputs are not used by OpenAI to train its models per OpenAI's API data usage policy. Cross-border transfer to the US is covered by Standard Contractual Clauses.
  See OpenAI's Privacy Policy: [https://openai.com/policies/privacy-policy/](https://openai.com/policies/privacy-policy/)

- **Apple App Store** (for iOS subscriptions) or **Google Play** (for Android subscriptions)
  Process payments and operate the push-notification delivery infrastructure (APNs / FCM). We do not see your payment card details.

If your data is transferred outside the European Economic Area (EEA), we ensure appropriate safeguards under GDPR Articles 44–49, including Standard Contractual Clauses where required.

---

## 5. Who Has Access to Your Data

Within the Service Provider's operations:
- Only Petros Chatzianastasiou has access to backend data, and only when necessary for technical support, debugging, or compliance with legal requirements.

We may disclose your information:
- When required by law (e.g., subpoena, court order, regulatory request)
- When necessary to protect rights, safety, or property of the Service Provider or others
- To investigate fraud, security breaches, or violations of our Terms

We do NOT share your data:
- With advertisers
- With data brokers
- With social networks (we do not integrate any social media SDKs)
- For any commercial purpose other than providing the Application's features

---

## 6. Data Retention

| Data Category | Retention Period |
|---|---|
| Active account data (profile, CRM data) | While your account is active |
| Account data after deletion request | Deleted within 30 days of your request |
| Soft-deleted (archived) contacts | 30-day grace period, then permanently deleted |
| Subscription transaction records | As required by tax and accounting law in Greece (typically 5 years) |
| Authentication logs | 90 days |
| Crash reports and error diagnostics | 90 days |

When you delete your account, we erase your personal data from our systems within 30 days, except where retention is required by law.

---

## 7. Your Rights Under GDPR

If you are located in the European Economic Area (EEA), the United Kingdom, or another jurisdiction with similar privacy laws, you have the following rights:

- **Right to access** — Request a copy of the personal data we hold about you.
- **Right to rectification** — Correct inaccurate or incomplete data.
- **Right to erasure** ("right to be forgotten") — Request deletion of your personal data.
- **Right to restrict processing** — Limit how we use your data.
- **Right to data portability** — Receive your data in a structured, machine-readable format.
- **Right to object** — Object to processing based on legitimate interest.
- **Right to withdraw consent** — Where processing is based on consent, withdraw it at any time.
- **No automated decision-making (GDPR Article 22)** — We do not make decisions about you based solely on automated processing that produce legal or similarly significant effects. AI suggestions (objection coach, message drafts, transcript parses, weekly digest) are non-binding assistance; you remain in full control.
- **Right to lodge a complaint** — File a complaint with the Hellenic Data Protection Authority ([www.dpa.gr](https://www.dpa.gr)) or your local supervisory authority.

To exercise any of these rights, email petros.canon@gmail.com. We will respond within 30 days as required by GDPR.

You can also delete your account at any time from within the Application via **Settings → Delete Account**, or by emailing the address above.

---

## 8. Permissions Requested by the Application

The Application requests the following device permissions:

- **Contacts** — Required to sync your phone book into your CRM. You may decline; the Application will function with manually entered contacts only. Permission can be revoked at any time in your device's system settings.
- **Microphone & Speech Recognition** (when you initiate voice features) — Used solely for on-device transcription of your dictated notes. Audio is processed locally by your operating system's speech-recognition service and is not transmitted to our servers. Optional; the Application functions without it.
- **Notifications** (when enabled) — To deliver reminders for scheduled calls and tasks. Optional.

The Application does NOT request access to:
- Location
- Camera
- Photos or media library
- System Calendar — the Application does not read from or write to your device's system calendar; any calendar-style features inside the Application use only internal records you create within DialDay.
- Health data
- Bluetooth or local network

---

## 9. Children's Privacy

The Application is intended for adult professional users (typically 18+). The Application is not directed to children under 16 (or under 13 in the United States per the Children's Online Privacy Protection Act, "COPPA"), and we do not knowingly collect personal data from children below these ages.

In Greece, the digital-consent age set by Greek Law 4624/2019 (implementing GDPR Article 8) is 15; the Application remains directed to adult professional users regardless and does not lower its baseline below 16.

If you are a parent or guardian and believe your child has provided personal data to the Application, please contact us at petros.canon@gmail.com. We will delete the data promptly upon verification.

---

## 10. Security

We take reasonable measures to protect your data:

- All data transmitted between the Application and our servers is encrypted using TLS.
- Passwords are protected using strong one-way hashing via Supabase Auth — never stored in plaintext.
- Database access is restricted to authorized personnel only and audited.
- Row-level security (RLS) is enforced at the database level, ensuring users can only access their own data.

However, no method of electronic transmission or storage is 100% secure. While we strive to protect your data, we cannot guarantee absolute security. In the event of a data breach affecting your personal data, we will notify you and the relevant supervisory authority as required by GDPR Article 33–34.

---

## 11. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in our practices, technology, legal requirements, or other factors. When we make changes:

- We will post the updated policy at the same URL
- We will update the "Last Updated" date at the top
- For material changes, we will notify users through the Application or via email

We encourage you to review this Privacy Policy periodically. Your continued use of the Application after changes are posted constitutes your acceptance of the updated policy.

---

## 12. Third-Party Links

The Application may contain links to third-party websites or services not operated by us. We are not responsible for the privacy practices of those third parties. We encourage you to read their privacy policies before providing personal data.

---

## 13. Contact Us

For questions, concerns, or to exercise your rights under this Privacy Policy:

**Email:** petros.canon@gmail.com

We aim to respond to all inquiries within 5 business days, and to formal GDPR requests within 30 days.

---

## 14. App Tracking Transparency

The Application does not track you across other companies' apps or websites. We do not use the iOS Identifier for Advertisers (IDFA), and we do not integrate any advertising or analytics SDKs that perform cross-app tracking. Because no cross-app tracking occurs, the Application does not display the iOS App Tracking Transparency prompt.

---

## 15. California Residents (CCPA / CPRA)

If you are a California resident, the California Consumer Privacy Act (as amended by the California Privacy Rights Act) gives you certain rights regarding your personal information:

- **Right to know** what personal information we collect and how it is used
- **Right to request deletion** of your personal information
- **Right to request correction** of inaccurate personal information
- **Right to opt out of sale or sharing** — not applicable: **we do not sell or share your personal information** as those terms are defined under the CCPA/CPRA, and we have not done so in the preceding 12 months
- **Right to limit use of sensitive personal information**
- **Right to non-discrimination** for exercising any of these rights

To exercise these rights, email petros.canon@gmail.com.

---

## 16. Sub-Processor Data Mapping

For App Store nutrition-label alignment, the following table summarises which data categories each sub-processor receives, whether the data is linked to your identity, and whether it is used for tracking:

| Sub-processor | Data categories received | Linked to your identity? | Used for tracking? |
|---|---|---|---|
| Supabase | Account info, CRM data, authentication metadata | Yes (account-bound) | No |
| RevenueCat | Pseudonymous user UUID, subscription status, transaction ID | Pseudonymous (UUID only) | No |
| Sentry | Device model, OS version, app version, stack traces, pseudonymous user ID | Pseudonymous | No |
| OpenAI | AI feature inputs (text you submit); for weekly digest, summary statistics | Pseudonymous (no name/email sent) | No |
| Apple / Google (StoreKit / Play Billing, APNs / FCM) | Payment, subscription, push token | Linked (by platform account) | No |

"Used for tracking" means tracking across other companies' apps or websites under Apple's App Tracking Transparency framework. No sub-processor receives data for that purpose.

---

*This Privacy Policy is provided in English. In case of conflict between this policy and any translated version, the English version prevails.*
