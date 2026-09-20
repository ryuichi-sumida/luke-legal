---
title: Luke Privacy Policy
permalink: /privacy/
---
# Luke Privacy Policy

**Last updated:** September 20, 2026

Luke ("the App") is developed and published by Ryuichi Sumida, an individual developer based in Kyoto, Japan ("we", "us"). This policy explains what information the App handles, what stays on your iPhone, what leaves it and why, and the choices you have. It applies to Luke on the App Store worldwide. Region-specific information for the United States and Japan is at the end.

## Summary

- Luke keeps your memory library on your iPhone. We run no server, have no account system, and never receive your photos, conversations, memories, journal, location history, recordings, face data, or voice data.
- Nothing leaves your iPhone except: limited requests to Apple (coordinates for place names, search text when you label a place, and speech language assets); the chat model and voice assets downloaded from Hugging Face if you turn on Talk or calls, which sees your IP address; and copies you choose to make or allow (Agent Access, Export, Back Up, and iOS device backups you have turned on).
- No advertising, no tracking, no sale of data, and no use of your data to train any model. Anonymous usage statistics are sent only if you turn them on (off by default) and never include your content.
- You can delete everything in the App with Settings → Privacy & Data → Clear All Data, or by uninstalling the App.

## Information Stored on Your Device

Luke stores the following on your device: the name and birthday you enter during setup, chat history with Luke, AI-generated memories, photo descriptions and tags, people you name in photos, place visits and place labels, journal entries and notes, voice memos, recorded conversations and their transcripts, face feature data, voice feature data, and app preferences.

This data lives inside the iOS app sandbox, encrypted by iOS with your device passcode. You can additionally require Face ID or your passcode to open the App (Settings → App Lock). We have no technical ability to read, copy, or restore it.

## On-Device AI

All AI features (chat, voice conversation, memory extraction, photo understanding, timeline and life analysis) run on your iPhone, using open-weight models that ship inside the app (photo, memory and speaker models) or are downloaded to your device when you turn on Talk or calls (the chat model and voice assets), plus Apple's built-in on-device models. No prompt, photo, transcript, or memory is sent to an external AI service by Luke, and nothing you do in Luke is used by us to train any model.

## Photos and Camera

With your permission, Luke reads your photo library on your device to build memories, using Apple's Vision framework and the on-device models. Photos you take with the camera inside Luke are stored on your device. Luke never uploads a photo, thumbnail, or derived description to us or to any AI service. Photo thumbnails can leave your iPhone only through Agent Access, Export, or backups, described below.

## Faces and Voices

To group photos of the same person and to recognize who is speaking in a recording, Luke computes face feature data and voice feature data on your iPhone.

- **Where it is stored:** face feature data is stored in Luke's database on your iPhone. Voice feature data is stored in a separate file on your iPhone.
- **Where it goes:** neither is sent to us or to anyone else, and neither is matched against any external database. Neither is included in Export. Face feature data is included in Back Up files you create and in iOS device backups you have enabled. Voice feature data is not included in Back Up files but is included in iOS device backups you have enabled.
- **Naming:** face groups stay unnamed until you choose to name them.
- **Deleting:** Clear All Data deletes all face feature data and all voice feature data. Deleting a person removes their name and signals and hides their group, but the face feature data for those photos stays on your iPhone until you use Clear All Data or uninstall the App; otherwise the same faces would simply be regrouped from your photo library. Uninstalling the App deletes all of it from the device.
- **Other people:** the people in your photos and recordings have not agreed to anything through you. You are responsible for using these features lawfully where you live, and some places regulate face and voice recognition of other people even when it happens on a personal device.

## Voice and Speech

Luke has three speech features, and they behave differently.

- **Voice conversations with Luke and voice memos in the journal** use Apple's speech recognition in on-device mode only. If on-device recognition for your language is not yet available on your iPhone, Luke shows an error instead of sending audio anywhere; enabling Dictation for that language in iOS Settings downloads it.
- **Recorded conversations** are transcribed by Apple's on-device transcriber. It downloads language assets from Apple as needed but does not send audio.
- **Luke's spoken replies** are generated by an on-device text-to-speech engine.

Voice audio never leaves your iPhone.

## Recorded Conversations

You can record real-life conversations only by an explicit tap. Recordings and transcripts are stored on your device. Nothing you record is uploaded by Luke. You are responsible for complying with the recording and consent laws that apply where you are; some places, including several US states, require the consent of everyone in a conversation.

## Location

If you grant location access, Luke records the places you visit to build your personal timeline, including in the background if you allow "Always" access. Visit history is stored on your device. To show place names, Luke sends the coordinates of each visit to Apple's geocoding service. When you search for or label a place, your search text and the map area are sent to Apple Maps. These requests go from your device to Apple, are governed by Apple's privacy policy, and carry no Luke identity, because Luke has none. You can pause location capture or delete your location history at any time in Settings.

## Network Connections

Luke has no server of its own. Your device connects to the following services, and only for the purposes listed.

| Purpose | Who receives the request | What they receive |
| --- | --- | --- |
| Downloading the chat model and voice assets when you turn on Talk or calls, when a model is updated, and if a file needs re-downloading. The photo, memory and speaker models ship inside the app and are never downloaded. | Hugging Face (huggingface.co) | Your IP address and standard download request metadata. No personal content. |
| Checking for model updates at launch (a small manifest file) | Hugging Face | Your IP address and request metadata. |
| Place names and place search | Apple | Coordinates of visits; search text and map area when you label a place. |
| Speech language assets | Apple | Asset downloads only. Audio is never sent. |
| Luke Pro subscription | Apple App Store | Apple processes the purchase. The App receives only the subscription status on your device. We never see your payment details or Apple ID. |
| Agent Access (off by default) | A tool on your own computer | See below. |
| Daily anonymous usage summary (off by default; only if you turn on Share Anonymous Usage Data) | TelemetryDeck GmbH (telemetrydeck.com), Germany | Feature-usage day counts, action counts, technical failure codes, average response times, Pro status, device model, iOS and App version, language, and a random one-time identifier. No content. Like any internet request it carries your IP address; TelemetryDeck states that it does not store IP addresses. |

The chat model (about 3.4 GB) and the voice models wait for Wi-Fi unless you allow cellular downloads. The launch-time update check may use any connection.

## Agent Access

Agent Access is off by default. If you turn it on, Luke listens on your local network while the App is open, and any tool that has the address and your access token (for example Claude Code on your Mac) can search your memories and receive matching text and photo thumbnails. That information leaves your iPhone and goes to the connected tool. Depending on the tool and how you configured it, the tool may send what it retrieved to a cloud AI provider or store it. Those copies are controlled by that tool and provider, not by Luke, and turning Agent Access off does not delete information a tool already retrieved.

Agents can read but never change your data. Luke does not publish the address to the internet; your network's configuration determines who can reach devices on it. Turning Agent Access off stops the server immediately, you can regenerate the token at any time, and Clear All Data deletes it.

## Backups and Export

- **Back Up (manual):** creates a single compressed file containing Luke's database (including face feature data), your recorded audio and voice memos, and your settings. It does not contain voice feature data or the downloaded models. Luke does not encrypt this file; you choose where to keep it (for example the Files app or your own iCloud Drive), and from then on it is outside the App. Treat it as sensitive, since Restore rebuilds Luke from it.
- **Export Data:** writes your memories, journal, people, places, and conversations as portable Markdown and JSON with copies of the related photos and audio, for your own use. Derived data such as face and voice feature data is never exported.
- **iOS and iCloud device backups:** if you have iCloud Backup or computer backups turned on, iOS includes Luke's data (database, audio, voice feature data, and settings, but not the downloaded models) in those backups, encrypted and handled by Apple under Apple's terms.
- **Deleting in Luke does not delete copies you have already made** with Back Up, Export, Agent Access, or device backups, and it never touches your Photos library.

## Anonymous Usage Statistics (Optional)

The App contains no advertising SDKs, sets no cookies, and does not track you across apps or websites. We do not sell or share personal information and we do not engage in targeted advertising.

Sharing usage statistics is **off by default**. If you turn on Share Anonymous Usage Data (offered during setup and available in Settings → Privacy & Data), the App sends one anonymous summary per day to TelemetryDeck GmbH, a privacy-focused analytics provider in Germany. The summary contains: which features you used; how long each area of the App was open; how far the photo analysis has progressed; counts of actions such as messages sent, calls started, recordings, imports, and backups; technical failure codes (for example a paused photo analysis or a failed model download); average response times; whether Luke Pro is active; whether Photos, Location, and Notifications access is granted; the approximate size of your photo library (in ranges); how many weeks since you installed the App; and device details: model, iOS version, App version, language, region, time zone, screen size, and display and accessibility settings. Each summary carries a random identifier generated for that summary alone, so summaries cannot be linked to you, your device, or to each other. Summaries never include photos, messages, prompts, answers, recordings, names, places, or any other content. Nothing is counted while the setting is off. Turning it off stops counting immediately and discards the unsent day. We use these statistics only to understand which features are used and what fails. Because this data cannot identify you, Do Not Track and Global Privacy Control signals do not change it.

Apple may share crash reports with us if you chose to share analytics with app developers in iOS Settings; that sharing is controlled by Apple.

Notifications are generated on your device. Luke does not send notifications from a server.

## Retention and Deletion

Your data stays on your device for as long as you keep it. You can delete individual items (a memory, a visit, a recording, a chat), or everything at once with Settings → Privacy & Data → Clear All Data. Uninstalling the App permanently deletes all Luke data on that device. See Faces and Voices for what deleting a person does.

## Security

Your data is protected by the iOS sandbox and device encryption, and optionally by App Lock. Model downloads are fetched over HTTPS. Since we hold no copy of your data, there is no Luke database that could be breached. Protect your device passcode, your Agent Access token, and any backup files you create.

## Support Correspondence

If you contact us, we receive what you send: your email address, your name if you include it, your message, and any screenshots or files you attach. We use it only to answer you and to investigate the problem you report. We receive and store this email through Google's Gmail service, whose servers may be located outside your country. We keep support threads until the issue is resolved and delete them within one year after that. Please do not send memories, recordings, or other people's information unless it is needed to solve your problem. In-app deletion does not delete email you have sent us; ask us and we will delete it.

## Children

Luke is not directed to children under 13, and we do not knowingly collect personal information from children under 13. If you believe a child has sent us personal information, contact us and we will delete it.

## Your Rights and Choices

You control your Luke data directly in the App: view, correct, export, and delete it there, because that is the only place it exists. Permissions for Photos, Location, Microphone, Speech Recognition, Camera, Local Network, and Notifications can be changed at any time in iOS Settings. For information we actually hold, which is limited to support correspondence, you can ask us to access, correct, or delete it at the address below, and we will respond as applicable law requires. Sharing anonymous usage statistics is optional; turn it off at any time in Settings → Privacy & Data.

## Additional Information for Users in the United States

This section supplements the policy for residents of US states with privacy laws, to the extent those laws apply to us.

- **Personal information we collect:** support correspondence only (contact details and message content), used to provide support. Everything else described in this policy is processed and stored on your device and is not disclosed to us. Anonymous usage statistics (if you turn them on) contain no identifiers and are not personal information.
- **Sale or sharing:** we do not sell personal information and do not share it for cross-context behavioral advertising, and have not in the preceding 12 months.
- **Sensitive personal information:** precise location, face and voice feature data, and audio are processed on your device for the App's functionality at your request. They are not disclosed to us.
- **Your requests:** rights to know, access, correct, delete, and port apply to the support correspondence we hold; email us. Your on-device data is under your direct control in the App. We will never discriminate against you for exercising a privacy right.
- **Third-party disclosures for direct marketing (California "Shine the Light"):** none.
- **Opt-out preference signals:** nothing is sold or shared, so there is nothing to opt out of.

## Additional Information for Users in Japan (日本のお客様へ)

This section supplements the policy under the Act on the Protection of Personal Information (個人情報保護法). A Japanese-language version of this section is published alongside the Japanese translation of this policy.

- **Business operator:** Ryuichi Sumida (individual). Address is provided without delay upon request.
- **Personal information we receive and its purpose of use:** support correspondence (email address, name if given, message and attachments), used solely to respond and to investigate the reported issue.
- **Provision to third parties and joint use:** none. **Service providers:** we use Google's Gmail service to receive and store support email; Google's servers may be located outside Japan, mainly in the United States. If you turn on anonymous usage statistics, TelemetryDeck GmbH (Germany) receives them; they contain no personal data.
- **Servers outside Japan contacted by your device:** when downloading models or using Apple features, your device communicates with servers operated by Apple and Hugging Face, which may be located in the United States, and, if you turn on anonymous usage statistics, by TelemetryDeck GmbH in Germany, as described in Network Connections. We do not send your personal data to them.
- **Requests regarding retained personal data:** we retain no personal data other than support correspondence. Requests for disclosure, correction, suspension of use, or deletion of that correspondence, and complaints, are accepted at the contact address below, free of charge, after identity verification.
- **Governing language:** if the Japanese translation and this English policy differ, this English version prevails.

## Third-Party Services

Your use of Apple services is governed by Apple's Privacy Policy (https://www.apple.com/legal/privacy/). Downloads from Hugging Face are governed by its privacy policy (https://huggingface.co/privacy). Support email is handled under Google's Privacy Policy (https://policies.google.com/privacy). Anonymous usage statistics, if you turn them on, are processed by TelemetryDeck GmbH under its privacy policy (https://telemetrydeck.com/privacy/).

## Changes to This Policy

We may update this policy when the App changes. The current version is always available in Settings → Legal → Privacy Policy and at the published URL. If a change materially affects what leaves your device, we will show it in the App before it takes effect.

## Contact

Ryuichi Sumida
Email: rui.sumida1@gmail.com
