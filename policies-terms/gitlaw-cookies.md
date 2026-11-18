---
title: GitLaw Cookies
slug: gitlaw-cookies
category: policies-terms
excerpt: GitLaw uses cookies and similar technologies to run and secure the site, to remember your preferences, to measure how the product is used, and to measure our advertising. This page lists what we set, who sets it, and how long it lasts.
---

GitLaw uses cookies and similar technologies to run and secure the site, to remember your preferences, to measure how the product is used, and to measure our advertising. This page lists what we set, who sets it, and how long it lasts. See the Cookies and similar technologies section of our [Privacy Policy](https://git.law/privacy-policy) for how we handle the personal data these technologies collect.

# Cookies

"Cookie" is used loosely on this page. Alongside HTTP cookies we use local storage, session storage, IndexedDB and pixel trackers, and each entry below says which one applies. Local and session storage that only holds in-product state you created yourself — a setting, a dismissed hint, a pending notice — carries no identifier and is not listed.

You can change your choice at any time through **Manage cookies**, linked in the footer of every page. Essential cookies cannot be turned off, because the site does not work without them.

Since the number and names of cookies change as we add and remove providers, the tables below may be updated from time to time. Cookie names containing `#` vary per property, per session or per environment.

## Essential cookies

Required to sign you in, keep the session secure, remember the choices you make on this page, protect our forms from abuse, and prevent payment fraud.

| Name                    | Provider         | Type          | Duration                                      | Purpose                                                                                                                            |
| ----------------------- | ---------------- | ------------- | --------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| gls_auth                | GitLaw           | Cookie        | Session, or 30 days if you tick "remember me" | Your signed-in session                                                                                                             |
| gls                     | GitLaw           | Cookie        | 14 days                                       | Temporary state for Google sign-in and account linking, and the referral code from a signup link, kept across the sign-in redirect |
| \_glaw                  | GitLaw           | Cookie        | 1 year                                        | Your cookie consent choice                                                                                                         |
| redirect_to             | GitLaw           | Cookie        | Session                                       | Where to return to after sign-in                                                                                                   |
| gl_pending_jurisdiction | GitLaw           | Cookie        | Session                                       | The jurisdiction you picked before signing up, so it can be applied to your new account                                            |
| gl_signup_answers       | GitLaw           | Cookie        | 1 hour                                        | What you told us in the sign-up chat before creating your account, so it can be saved to your new account                          |
| \_glui                  | GitLaw           | Cookie        | 1 year                                        | Interface preferences you set yourself (view mode, sidebar state)                                                                  |
| \_gltry                 | GitLaw           | Cookie        | 1 year                                        | Which home-page Try cards you have completed, and whether you minimised them                                                       |
| chat-message-requests   | GitLaw           | IndexedDB     | Until the message is sent                     | Holds a chat message you have just submitted while it is handed between pages                                                      |
| \_\_stripe_mid          | Stripe           | Cookie        | 1 year                                        | Fraud prevention: identifies the browser across payment sessions                                                                   |
| \_\_stripe_sid          | Stripe           | Cookie        | 30 minutes                                    | Fraud prevention: identifies the current payment session                                                                           |
| m                       | Stripe           | Cookie        | 400 days                                      | Fraud prevention: records which checks your browser supports. Set on `m.stripe.com`                                                |
| \_GRECAPTCHA            | Google reCAPTCHA | Cookie        | 6 months                                      | Distinguishes people from bots on the sign-in, sign-up, account-linking and signing forms. Set on `www.google.com`                 |
| \_grecaptcha            | Google reCAPTCHA | Local storage | Persistent                                    | Supports the same check                                                                                                            |

Stripe's cookies are set only when a payment screen is opened. reCAPTCHA loads only on the forms named above.

## Functional cookies

Remember a choice you made about how the site behaves.

| Name    | Provider       | Type   | Duration | Purpose                                                                          |
| ------- | -------------- | ------ | -------- | -------------------------------------------------------------------------------- |
| g_state | Google Sign-In | Cookie | 6 months | Remembers that you dismissed the Google sign-in prompt, so it is not shown again |

## Analytics cookies

Used to understand how the product is used so we can improve it. These identify a browser, a device or a signed-in account — they are not anonymous.

| Name                         | Provider         | Type            | Duration   | Purpose                                                                                                                                  |
| ---------------------------- | ---------------- | --------------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| gl_d_id                      | GitLaw           | Cookie          | 1 year     | Identifies this device across visits                                                                                                     |
| gl_s_id                      | GitLaw           | Cookie          | 1 year     | Groups events into a single session                                                                                                      |
| gl_ft                        | GitLaw           | Cookie          | 90 days    | How you first reached GitLaw (channel, referring site, campaign). Stored only for the browser session until you accept analytics cookies |
| gl_anonymous_id              | GitLaw           | Session storage | Session    | Identifies this browser before you sign in                                                                                               |
| gl_session_id                | GitLaw           | Session storage | Session    | Groups the events in one visit                                                                                                           |
| EXP\_#_identity              | Amplitude        | Cookie          | 1 year     | Keeps you in the same variant of an A/B test between visits                                                                              |
| EXP\_#                       | Amplitude        | Local storage   | Persistent | Which A/B test variants you are assigned to                                                                                              |
| EXP\_#_DEFAULT_USER_PROVIDER | Amplitude        | Local storage   | Persistent | Supports the same assignment                                                                                                             |
| EXP_MKTG\_#                  | Amplitude        | Local storage   | Persistent | Which marketing A/B test variants you are assigned to                                                                                    |
| amplitude.engagement.#       | Amplitude        | Local storage   | Persistent | Amplitude user id and in-product guide state                                                                                             |
| sentryReplaySession          | Sentry           | Session storage | Session    | Links the errors recorded during a visit so a crash can be traced back through the steps that caused it. Sensitive information is masked |
| \_ga                         | Google Analytics | Cookie          | 400 days   | Identifies a visitor for usage statistics                                                                                                |
| \_ga\_#                      | Google Analytics | Cookie          | 400 days   | Counts visits and records first and most recent visit                                                                                    |

Amplitude also records session replays — clicks, scrolling and typing behaviour — to show how people move through the product. Sensitive information is masked automatically.

We use **Segment** to route analytics events, and **Jitsu** on our own infrastructure to collect them. Neither stores anything in your browser: our Segment SDK runs with client-side storage switched off, so GitLaw's own identifiers above are the only ones used.

## Marketing cookies

Used to measure our advertising and to credit affiliate referrals.

| Name                     | Provider   | Type          | Duration   | Purpose                                                                                              |
| ------------------------ | ---------- | ------------- | ---------- | ---------------------------------------------------------------------------------------------------- |
| \_fbp                    | Meta       | Cookie        | 3 months   | Measures ads and delivers advertising products                                                       |
| lastExternalReferrer     | Meta       | Local storage | Persistent | Records the last URL you arrived from                                                                |
| lastExternalReferrerTime | Meta       | Local storage | Persistent | Records when you arrived from that URL                                                               |
| log/error                | Meta       | Pixel tracker | Session    | Detects and logs tracking errors                                                                     |
| \_fbc                    | Meta       | Cookie        | 90 days    | Records the Facebook or Instagram ad you clicked to reach the site                                   |
| multiFbc                 | Meta       | Local storage | Persistent | Supports the same ad-click record                                                                    |
| \_gcl_au                 | Google Ads | Cookie        | 3 months   | Measures ad efficiency across sites using Google services                                            |
| \_gcl_ls                 | Google Ads | Local storage | Persistent | Measures conversion between you and advertising banners                                              |
| \_gcl_aw                 | Google Ads | Cookie        | 90 days    | Records the Google Ads ad you clicked to reach the site                                              |
| \_gcl_dc                 | Google Ads | Cookie        | 90 days    | Records the Display & Video 360 or Campaign Manager ad you clicked to reach the site                 |
| \_gcl_gb                 | Google Ads | Cookie        | 90 days    | Records a Google Ads click that led you to the site                                                  |
| \_gcl_ag                 | Google Ads | Cookie        | 90 days    | Records a Google Ads click that led you to the site                                                  |
| \_gcl_gs                 | Google Ads | Cookie        | 90 days    | Records a Google Ads click that led you to the site                                                  |
| GCL_AW_P                 | Google Ads | Cookie        | 90 days    | Supports the same ad-click record. Set on `google.com`, `googleadservices.com` and `doubleclick.net` |
| IDE                      | Google Ads | Cookie        | 400 days   | Measures ad performance and presents targeted ads. Set on `doubleclick.net`                          |
| test_cookie              | Google Ads | Cookie        | 15 minutes | Checks whether your browser accepts cookies. Set on `doubleclick.net`                                |
| NID                      | Google Ads | Cookie        | 6 months   | Identifies your browser to Google for security and advertising. Set on `google.com`                  |
| pagead/1p-user-list/#    | Google Ads | Pixel tracker | Session    | Tracks interest in products or events across sites                                                   |
| pagead/gen_204           | Google Ads | Pixel tracker | Session    | Reports ad tag activity back to Google                                                               |
| rewardful.referral       | Rewardful  | Cookie        | 30 days    | Which affiliate referred you, so the referral can be credited                                        |

Google Analytics (`_ga`, `_ga_#`) is listed under Analytics rather than here, because it follows your analytics choice, not your marketing choice.

The ad-click cookies (`_fbc`, `multiFbc`, `_gcl_aw`, `_gcl_dc`, `_gcl_gb`, `_gcl_ag`, `_gcl_gs`, `GCL_AW_P`) are set only when you arrive by clicking one of our ads.

Rewardful runs on every page but sets `rewardful.referral` only when you arrive through an affiliate link.

## Questions

Email [privacy@git.law](mailto:privacy@git.law).

## Related

- [GitLaw Subprocessors](/knowledge-base/gitlaw-subprocessors) - the providers that process data on our behalf
- [Privacy Policy](https://git.law/privacy-policy) - how GitLaw handles personal data
- [Where we store data](/knowledge-base/where-we-store-data)
