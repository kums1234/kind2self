# Privacy Policy — Kind2Self

**Effective date:** 2026-05-10

This is the privacy policy for the Kind2Self iOS app ("the app"). It tells you exactly what the app does and does not do with your data. Where this policy makes claims about the app's behaviour, those claims correspond to specific code in the app — not marketing language.

## TL;DR

- The app does not have a server. No data is uploaded to us, ever.
- All your affirmations, voice recordings, small wins, and transcriptions live on your device. If you turn on iCloud Drive sync in Settings, they also live in *your* iCloud Drive — visible to you in the Files app, governed by Apple's iCloud terms.
- The app contains no analytics, no tracking, no advertising SDKs, and no third-party libraries that phone home.
- The microphone and speech recognition framework are used on-device only.

## What data the app collects

- **Affirmations** you select, edit, or write yourself, including any voice recordings of you reading them.
- **Small wins** you type or speak, including voice recordings.
- **Transcriptions** of your voice wins, generated on-device by Apple's Speech framework.
- **Settings** — your reminder times, which themes you've enabled, your favorited affirmations.

The app does not collect your name, email, contacts, location, device identifiers, IP address, or any analytics.

## Where your data is stored

- **By default:** in the app's private Documents directory on your iPhone. This data is included in your iPhone's local backup if you have iPhone backup enabled.
- **If you enable iCloud Drive sync:** in your personal iCloud Drive, in a folder named "Kind2Self." This is *your* iCloud Drive — Anthropic, Apple, and we have no privileged access to it. Apple's iCloud terms apply to that storage.

The app does not transmit data to us. There is no server endpoint we control.

## Permissions the app uses

- **Microphone (`NSMicrophoneUsageDescription`):** to record your affirmations in your own voice and to record voice notes for small wins. Recordings are saved to your device only.
- **Speech Recognition (`NSSpeechRecognitionUsageDescription`):** to transcribe your voice wins so the Insights view can surface recurring themes and a mood trend. Transcription runs **on-device** (`requiresOnDeviceRecognition = true`) — audio is never sent to Apple's servers from this app. (Apple's framework requires this permission whether you use on-device or cloud transcription; we use on-device only.)
- **Notifications:** to deliver your morning, evening, and Saturday weekly digest reminders. Notification content is generated on-device.

You can revoke any permission at any time in iOS Settings → Privacy & Security. The app will fall back gracefully — features that depend on the revoked permission stop working but the rest of the app continues.

## Third parties

The app contains no third-party SDKs. Specifically: no Firebase, no Mixpanel, no AppsFlyer, no Adjust, no Crashlytics, no Sentry, no Google Analytics, no Facebook SDK, no advertising frameworks. The only frameworks used are Apple's own (Foundation, SwiftUI, AVFoundation, Speech, NaturalLanguage, UserNotifications, Charts, FoundationModels).

If you enable iCloud Drive sync, your data is stored in Apple's iCloud, governed by [Apple's Privacy Policy](https://www.apple.com/legal/privacy/).

## Sending and receiving kindnesses

The "Send a kindness" feature lets you share an affirmation or short note with someone you choose. It works without any server we operate:

- The message you send is **encoded directly into the share link** you give to the recipient. We have no server to receive or store it. The message text never reaches us, GitHub, or anywhere else — the recipient's device decodes it locally when they open the link.
- The link travels through whichever messaging app you choose from the iOS share sheet (iMessage, WhatsApp, Mail, AirDrop, etc.). That messaging app's privacy policy governs the transport. We have no insight into who you sent it to, when, or whether it was received.
- Your sender name is attached only if you have explicitly turned on "Include my name" in Settings → Sharing kindnesses. The default is **off** (anonymous).
- Before a message is sent, it's reviewed on your device for content that doesn't fit the spirit of the feature (links, contact info, all-caps shouting, hostile wording). On capable devices (iPhone 15 Pro or later, iOS 18.1+) this review uses Apple Intelligence's on-device language model. Otherwise it uses simple structural checks plus Apple's NaturalLanguage sentiment scoring. **The text never leaves your device for this review.**
- When you receive a kindness, the sender's name (if any) and the message appear in a sheet inside the app. You can save it to your library or close it without saving. We never see what you receive either.
- If the sender's app flagged a message as borderline at compose time, you'll see a reveal gate first — you can choose to read it or close without revealing.

## Data retention and deletion

Your data lives on your device for as long as you keep the app installed. To delete it:

- **For specific items:** swipe to delete in the Wins or Library lists.
- **For all app data:** delete the app from your iPhone. iOS removes the local Documents directory automatically.
- **For iCloud copies:** if you enabled iCloud Drive sync, also open the Files app → iCloud Drive → Kind2Self → delete the folder.

We have no copies of your data, so there's nothing to request deletion of.

## Children

The app is not directed at children under 13. It does not knowingly collect data from anyone, but if you are a parent or guardian and you find that your child has been using the app, the deletion steps above remove all their data instantly.

## Changes to this policy

If the app's behaviour changes in ways that affect privacy — for example if a future version adds a backend or analytics — this policy will be updated and the in-app onboarding will surface the change before the new behaviour takes effect.

## Contact

For questions about this policy or how the app handles your data:

kumaran.pec@gmail.com

---
