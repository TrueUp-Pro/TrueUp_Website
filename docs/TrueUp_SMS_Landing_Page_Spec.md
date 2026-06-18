# TrueUp SMS Landing Page Spec

## Purpose

Create a public SMS disclosure and campaign collateral page for TrueUp VidSummary A2P 10DLC registration.

The goal of this page is to give carrier reviewers a clear, verifiable explanation of how users opt in to receive SMS/MMS messages from TrueUp and what disclosures are shown before a user sends a message.

Recommended URL:

```text
https://trueup.pro/sms
```

---

# Key Concern: Public Phone Number

TrueUp's SMS/MMS phone number is:

```text
+1 (206) 761-0690
```

If TrueUp does not want this number broadly discoverable, the page can still be public but not prominent.

Recommended approach:

- Publish the page at `https://trueup.pro/sms`
- Do not link it from the main navigation
- Add `noindex` metadata so search engines are asked not to index it
- Use the page primarily as Twilio/carrier campaign collateral
- Include the phone number on the page because reviewers need to verify the opt-in path

Suggested page metadata:

```html
<meta name="robots" content="noindex, nofollow">
```

Important: The page must still be accessible without login or authentication.

---

# Page Title

```text
TrueUp VidSummary SMS Service
```

---

# Page Summary

TrueUp VidSummary lets users submit a property video by SMS/MMS and receive a property analysis report.

Users initiate the interaction by texting a property video to the TrueUp phone number. TrueUp responds with transactional messages related to that request, including confirmation, processing updates, and a secure link to the completed report.

---

# Required Page Content

## Hero Section

### Heading

```text
TrueUp VidSummary SMS Service
```

### Body Copy

```text
Text a property video to TrueUp and receive a property analysis report.
```

### Phone Number Display

```text
Text your property video to: +1 (206) 761-0690
```

---

# How It Works Section

```text
1. Record a property video.
2. Text the video to +1 (206) 761-0690.
3. TrueUp processes the video.
4. TrueUp sends transactional SMS updates about your request.
5. When your report is ready, TrueUp sends a secure link to your property analysis report.
```

---

# Consent / Opt-In Disclosure Section

This section is the most important part for A2P approval.

Use this exact or near-exact language:

```text
By texting a property video to TrueUp at +1 (206) 761-0690, you consent to receive transactional SMS/MMS messages from TrueUp related to your property analysis request.

Messages may include confirmation that your video was received, processing updates, error notices, and a secure link to your completed report.

Message frequency varies based on your activity. Message and data rates may apply. Reply HELP for help. Reply STOP to opt out.
```

---

# Message Frequency Section

```text
Message frequency varies based on user activity. Most property video submissions result in 1-5 messages, including receipt confirmation, processing updates, and report delivery.
```

---

# HELP / STOP Section

```text
For help, reply HELP.

To stop receiving messages, reply STOP. You may also use other standard opt-out keywords such as CANCEL, END, QUIT, or UNSUBSCRIBE.
```

---

# Non-Marketing Disclosure

```text
TrueUp VidSummary messages are transactional and are sent only in response to a user-initiated property video submission. TrueUp does not use this SMS service to send marketing or promotional messages.
```

---

# Privacy and Terms Links

Include visible links to:

```text
Privacy Policy: https://trueup.pro/privacy-policy/
Terms of Service: https://trueup.pro/terms-of-service/
```

Suggested display text:

```text
Review our Privacy Policy and Terms of Service.
```

---

# Suggested Full Page Copy

```markdown
# TrueUp VidSummary SMS Service

Text a property video to TrueUp and receive a property analysis report.

Text your property video to: **+1 (206) 761-0690**

## How It Works

1. Record a property video.
2. Text the video to **+1 (206) 761-0690**.
3. TrueUp processes the video.
4. TrueUp sends transactional SMS updates about your request.
5. When your report is ready, TrueUp sends a secure link to your property analysis report.

## SMS Consent

By texting a property video to TrueUp at **+1 (206) 761-0690**, you consent to receive transactional SMS/MMS messages from TrueUp related to your property analysis request.

Messages may include confirmation that your video was received, processing updates, error notices, and a secure link to your completed report.

Message frequency varies based on your activity. Message and data rates may apply. Reply HELP for help. Reply STOP to opt out.

## Message Frequency

Message frequency varies based on user activity. Most property video submissions result in 1-5 messages, including receipt confirmation, processing updates, and report delivery.

## Help and Opt-Out

For help, reply HELP.

To stop receiving messages, reply STOP. You may also use other standard opt-out keywords such as CANCEL, END, QUIT, or UNSUBSCRIBE.

## Non-Marketing Use

TrueUp VidSummary messages are transactional and are sent only in response to a user-initiated property video submission. TrueUp does not use this SMS service to send marketing or promotional messages.

## Privacy and Terms

Review our [Privacy Policy](https://trueup.pro/privacy-policy/) and [Terms of Service](https://trueup.pro/terms-of-service/).
```

---

# Twilio Campaign Message Flow Update

When resubmitting the A2P campaign, use this updated message flow language:

```text
Users discover the TrueUp VidSummary SMS service through the public SMS disclosure page at https://trueup.pro/sms.

The page instructs users to text a property video to TrueUp at +1 (206) 761-0690 to receive a property analysis report.

Before sending a message, users are shown the following disclosures:

- By texting a property video to TrueUp, users consent to receive transactional SMS/MMS messages from TrueUp related to their property analysis request.
- Messages may include receipt confirmation, processing updates, error notices, and a secure link to the completed report.
- Message frequency varies based on user activity.
- Message and data rates may apply.
- Reply HELP for help.
- Reply STOP to opt out.

After reviewing the disclosures, the user voluntarily sends an SMS/MMS message containing a property video. TrueUp responds with transactional messages related only to that request, including acknowledgement, processing updates, and a secure report link.

No marketing or promotional messages are sent.
```

---

# Twilio Campaign Call-To-Action Update

Use this language if Twilio asks for a Call to Action:

```text
Users are instructed on the TrueUp SMS disclosure page to text a property video to +1 (206) 761-0690 to receive a property analysis report. The page includes SMS consent language, message frequency disclosure, message and data rates disclosure, HELP instructions, STOP opt-out instructions, and links to the TrueUp Privacy Policy and Terms of Service.
```

---

# Sample Messages for Campaign

## Video Received

```text
TrueUp: We received your property video and are generating your report. Message frequency varies. Msg & data rates may apply. Reply HELP for help or STOP to opt out.
```

## Processing Update

```text
TrueUp: Your property analysis is currently being processed. We'll notify you when your report is ready.
```

## Report Ready

```text
TrueUp: Your property report is ready: https://trueup.pro/report/abc123 Reply STOP to opt out.
```

## Processing Error

```text
TrueUp: We were unable to process your video. Please resend a clearer recording of the property. Reply HELP for help or STOP to opt out.
```

## HELP Response

```text
TrueUp Support. Reply STOP to opt out. Visit https://trueup.pro for assistance.
```

## STOP Response

```text
You have been unsubscribed from TrueUp messages. Reply START to re-subscribe.
```

---

# Implementation Checklist

## Web Page

- [ ] Create `https://trueup.pro/sms`
- [ ] Add `noindex, nofollow` metadata
- [ ] Include TrueUp phone number: `+1 (206) 761-0690`
- [ ] Include how-it-works section
- [ ] Include SMS consent language
- [ ] Include message frequency disclosure
- [ ] Include message and data rates disclosure
- [ ] Include HELP instructions
- [ ] Include STOP opt-out instructions
- [ ] Include Privacy Policy link
- [ ] Include Terms of Service link
- [ ] Make page publicly accessible without login

## Twilio Resubmission

- [ ] Update Message Flow with the new detailed language
- [ ] Update Call to Action with the new detailed language
- [ ] Use `https://trueup.pro/sms` as campaign collateral
- [ ] Confirm Privacy Policy URL: `https://trueup.pro/privacy-policy/`
- [ ] Confirm Terms URL: `https://trueup.pro/terms-of-service/`
- [ ] Resubmit campaign for carrier review

---

# Notes

The likely reason for the prior rejection was that the original campaign did not give reviewers enough information to verify the opt-in path. This page is designed to solve that problem by making the complete opt-in workflow public, reviewable, and explicit.

The phone number does not need to be promoted broadly, but it should appear on the SMS landing page so reviewers can verify what users see before initiating contact.
