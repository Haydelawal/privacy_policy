# Guangel Privacy Policy

## 1. Introduction

Guangel collects only what it needs to alert the people you trust, never sells your data, and shows no ads. This policy explains what the Guangel Android app ("Guangel", "the app") collects, why, where it is stored, who can see it, how long it is kept, and how you can delete it.

Guangel is developed and operated by Hayde117 ("we", "us", "our"), an independent developer. Hayde117 is the data controller for the personal data described here.

- **Effective date:** 8 November 2026
- **Contact:** haydelawal@gmail.com
- **Applies to:** the Guangel app on Google Play, and the web page your trusted contacts open from a Guangel link (the "viewer").

By creating an account or using Guangel you agree to this policy. If you do not agree, please do not use the app.

## 2. Summary

Everything Guangel stores in the cloud lives in Google Firebase and Google Cloud in the European Union (Madrid, Spain region), encrypted in transit and at rest.

| Data | Why we need it | Where it is stored | Who else can see it | How long it is kept |
| --- | --- | --- | --- | --- |
| Email address and password | To sign you in | Firebase Authentication (password stored only as a one-way hash by Google) | No one | Until you delete your account |
| Trusted contacts (name, phone, optional email) and groups | To know who to alert | Cloud Firestore | No one; the people themselves receive your alert texts | Until you delete them or your account |
| Your own alert messages | To send the text you wrote | Cloud Firestore | Your chosen recipients, when you send an alert | Until you delete them or your account |
| Location during an alert or check-in | To show your recipients where you are | Cloud Firestore | Anyone holding that alert's link, until the alert is deleted (read-only once sharing ends) | Your auto-delete setting (default 30 days, maximum 180) |
| Audio recorded during an alert | Evidence you choose to capture | Cloud Storage for Firebase | Anyone holding that alert's link, until the alert is deleted (read-only once sharing ends) | Your auto-delete setting (default 30 days, maximum 180) |
| Alert and check-in records | Your History, and to make links work | Cloud Firestore | No one | Your auto-delete setting |
| Names your recipients give when they tap "I've got this" | So you, and the others you alerted, know who is responding | Cloud Firestore | You, and anyone holding that alert's link, until the alert is deleted (read-only once sharing ends) | With the alert (your auto-delete setting) |
| Checklist progress and app settings | So they follow you between phones | Cloud Firestore and your phone | No one | Until you delete your account |
| App PIN and decoy settings | To lock the app | Your phone only (PIN as a salted hash) | No one | Until you turn the lock off or uninstall |
| Crash reports and basic usage events | To fix bugs and keep the app reliable | Firebase Crashlytics and Google Analytics for Firebase | Google, as our processor | Up to 90 days (crashes); up to 14 months (analytics) |
| Notification token | To deliver Cate safety tips you opted into | Firebase Cloud Messaging | Google, as our processor | Until you turn tips off or uninstall |

We do **not** sell personal data, share it for advertising, or use it to profile you.

## 3. Information we collect

We collect information you give us, information created when you use safety features, and limited technical data about the app.

### 3.1 Information you give us

- **Account details.** Your email address and a password. Google Firebase Authentication stores the password as a one-way hash; we never see it.
- **Trusted contacts.** For each person you add: a name, a phone number with its country code, and optionally an email address. You can add up to 50 individuals.
- **Groups.** A group name and which of your contacts belong to it (up to 10 groups of 5 people).
- **Your chosen recipients.** Which contacts or group receive your SOS by default.
- **Custom messages.** Up to 10 messages you write yourself (160 characters each), with optional event tags such as "Airport".
- **Settings.** Your preferences, such as the default sharing time, how the SOS screen starts, the SOS button style, the auto-delete period and reminder choices.
- **Checklist progress.** Whether each Cate checklist item is marked Done, Not yet or N/A.

You choose to give us information about your trusted contacts. Please only add people who have agreed to receive safety alerts from you.

### 3.2 Information created when you use safety features

- **Precise location.** Collected **only** while an SOS alert or a check-in alert is active. It includes latitude, longitude, accuracy and time. Guangel does not track your location at any other time.
- **Route.** While an alert is active, Guangel saves a point when you move about 25 metres or more, so your recipients can see where you started and where you were last seen.
- **Audio recordings.** If you allow microphone access, Guangel records audio during an active SOS alert, for up to 10 minutes per alert. Recording stops when you stop the alert or the limit is reached. Android always shows the microphone indicator and a notification while recording.
- **Alert records.** For each alert: when it started and ended, which message was used, the sharing time you chose, and its status.
- **Check-in timers.** The due time you set and whether you checked in. This is kept on your phone only. If a check-in alert goes out, it is stored like any other alert.

### 3.3 Information collected automatically

- **Crash reports** (Firebase Crashlytics): device model, Android version, app version, and the technical details of the crash. Crash reports do not include your contacts, messages, location or recordings.
- **Usage events** (Google Analytics for Firebase): basic events such as app opens and screen views, with an app-instance identifier. We never log contact details, message text, locations or links.
- **Notification token** (Firebase Cloud Messaging): a device token used to deliver safety tips if you turn them on.
- **Network status:** the app checks whether you are online or on a weak connection, on your phone only, so it can tell your recipients the link may be delayed. This is not sent to us.

### 3.4 Information about people who open your link

When a trusted contact opens your Guangel link, our viewer service receives the standard information any website receives: their IP address, browser type and the time of the request. We use the IP address only to limit abusive traffic (120 requests per minute) and do not store it with your data. Google Cloud keeps standard request logs for up to 30 days. Their browser also loads map images from OpenStreetMap (see section 8).

If someone you alerted taps **I've got this** on that page, they are asked who they are. The name they type (up to 40 characters) and the time are saved with your alert. You see them in the app and in History, and everyone else who opens the link sees them too, so your contacts can coordinate. They are deleted with the alert. To prevent abuse, each IP address can send only a few of these a minute.

## 4. App permissions

Guangel asks for each permission only when a feature needs it, and explains why first. You can refuse or withdraw any permission in your phone's Settings; the app tells you what will not work and offers a button to open Settings.

| Permission | What it is used for | If you refuse |
| --- | --- | --- |
| Precise and approximate location | Sharing where you are during an active alert or check-in alert | Alerts still send your message, but without a working location |
| Microphone | Recording audio during an active SOS alert | Alerts work without a recording |
| Send SMS (optional) | **Only** to text your chosen contacts automatically when you miss a check-in. Guangel asks for your agreement in the app before you turn this on, and never uses it for anything else | When a check-in is missed, Guangel rings and opens your messaging app with the alert ready for you to send |
| Notifications | Showing that location sharing is on, check-in timer warnings, and safety tips you opt into | You will not see timer warnings or tips |
| Foreground service (location, microphone, data sync) | Keeping an alert running and uploading safely while the app is in the background | Required for alerts to work |
| Exact alarms | Firing a check-in alert on time | The check-in alert may fire a few minutes late |
| Internet and network state | Talking to our servers and detecting a weak connection | The app cannot sync |

Guangel does **not** request access to your camera, your address book, your SMS inbox, or your location in the background outside an active alert. Guangel never reads your messages. SOS alerts are sent through your phone's own messaging app, where you tap Send yourself.

## 5. How we use your information

We use your information only to run Guangel's safety features, keep the service secure, and fix problems.

| Purpose | Data used | Legal basis (EU/UK GDPR, Nigeria NDPA) |
| --- | --- | --- |
| Create and secure your account | Email, password | Performance of our agreement with you |
| Send alerts and show your location and recording to your recipients | Contacts, messages, location, audio, alert records | Performance of our agreement; your explicit action of starting an alert |
| Send an SMS automatically when you miss a check-in | Check-in timer, chosen contacts, message, location link | Your consent, which you can withdraw in Settings |
| Keep your History, checklists and settings | Alert records, checklist progress, settings | Performance of our agreement |
| Send Cate safety tips | Notification token | Your consent (off by default) |
| Prevent abuse and control costs | Alert counts per hour and day, viewer IP addresses | Our legitimate interest in keeping the service safe and available |
| Fix crashes and improve reliability | Crash reports, usage events | Our legitimate interest in a working app |
| Meet legal obligations | Any data required by law | Legal obligation |

We do **not**:

- show ads or include any advertising SDK;
- sell, rent or trade your personal data;
- use your location, recordings or contacts for marketing, profiling or automated decisions;
- send messages to your contacts except the alerts you start or the check-in alerts you set up.

## 6. How alerts and links work

An alert is a text message from your own phone number containing your message and a private web link that shows your location, and your recording if there is one.

**SOS alerts.** When you start an SOS, Guangel opens your phone's messaging app with the message and recipients filled in. You tap Send. The text is sent by your mobile carrier like any other SMS, at your normal carrier rates. Guangel does not see the delivery or read replies.

**Check-in alerts.** When you set a check-in timer and do not cancel it in time, Guangel alerts the contacts you chose:

- **If you agreed to automatic sending,** Guangel sends the SMS directly from your phone, in the background, using the Send SMS permission. The message says you set a check-in timer and did not respond, and includes your location link. Guangel shows you this before you agree, and you can turn it off at any time in Settings.
- **If you did not agree,** Guangel rings and opens your messaging app with the alert ready, and you tap Send.
- Automatic sending needs your phone to be on and to have mobile signal. If your phone is off or out of coverage, the text cannot be sent.

**The link.** Each alert has its own link containing a long random code (256 bits). Anyone who has the link can open it in a browser, without an account, until the alert is deleted (see Expiry). It shows:

- your message;
- your latest location, its accuracy and when it was updated, plus your route (start and last-seen points);
- the audio recording, after the alert ends, if one was made;
- the names of anyone who has said "I've got this", and when;
- when live sharing ends.

It does **not** show your name, email, phone number or your other contacts.

**Expiry.** Live sharing lasts for the sharing time you chose (15, 30 or 60 minutes; default 30), counted from when the alert started. Our server enforces this: after that, the link shows a read-only replay: the route, your message and any recording, with no live updates, no "I've got this" button and no responders' names. The replay keeps working until the alert is deleted, by you or by automatic deletion. Stopping an alert early stops new location updates immediately.

**Forwarded links.** A link can be forwarded or copied by anyone who receives it, and we cannot undo what someone has already seen. Only send alerts to people you trust.

**Replay links.** In History you can make a separate replay link for a past alert, to show it to someone new. It opens the same read-only replay, works for 7 days, and stops working if you delete the alert. As with alert links, we store only a one-way hash of its code.

**Weak or no connection.** If you are offline, Guangel still prepares the text with the link, adds a note that the link may take a while to work, and uploads your location as soon as you are back online.

## 7. Where and how your data is stored and protected

Your cloud data is stored by Google in the **europe-southwest1 (Madrid, Spain)** region, in services Google runs on our behalf. The daily job that deletes old alerts runs in Google's Belgium region (europe-west1); it only deletes data and keeps nothing there.

| Service (Google) | What it holds |
| --- | --- |
| Firebase Authentication | Your email and hashed password |
| Cloud Firestore | Contacts, groups, messages, settings, checklist progress, alert records, locations |
| Cloud Storage for Firebase | Audio recordings |
| Cloud Functions and Cloud Run | The servers that register links and show the viewer page; they do not keep your data |
| Firebase Crashlytics, Google Analytics, Cloud Messaging, Remote Config | Crash reports, usage events, notification tokens, app configuration |

**How we protect it:**

- All traffic between the app, the viewer and Google uses HTTPS (TLS). Data is encrypted at rest by Google.
- Database rules let each signed-in user read and write only their own data. Link records and abuse counters can only be read by our servers.
- We store only a one-way **hash** of each link's code, never the code itself. Someone who obtained a copy of our database could not use it to open your links.
- Recordings are never public. The viewer gives a recipient a signed audio address that stops working after a few minutes.
- Our servers limit how many links each account can create (by default 10 per hour and 30 per day) and how often each IP address can load the viewer.
- The viewer page tells search engines not to index it and does not send the link to other websites.

**On your phone:** Guangel keeps a local copy of your contacts and checklist progress so they work offline. If you set an app PIN, only a salted bcrypt hash of it is stored, on your phone only. Recordings are kept in the app's private storage until uploaded, then deleted from the phone.

No system is perfectly secure. If we learn of a breach that affects your personal data, we will notify you and the relevant authorities as the law requires.

## 8. Who we share information with

We share your information only with the people you choose to alert and with the service providers that run Guangel. We do not sell it.

| Recipient | What they receive | Why |
| --- | --- | --- |
| **Your chosen recipients** | Your alert text, and through the link your location, route and recording until the alert is deleted (read-only once sharing ends) | Because you sent them an alert |
| **Your mobile carrier** | The text messages you send, like any SMS | To deliver them |
| **Google LLC / Google Ireland** (Firebase and Google Cloud) | All cloud data listed above, as our data processor | Hosting, sign-in, database, storage, crash reporting, analytics, notifications. See [Firebase privacy](https://firebase.google.com/support/privacy) |
| **OpenStreetMap Foundation** | The recipient's IP address and the map area being viewed, when their browser loads map images | To draw the map on the viewer page. See the [OSMF privacy policy](https://osmfoundation.org/wiki/Privacy_Policy) |
| **Authorities** | Only what the law requires | If we receive a valid legal request, or to protect someone's life or safety |
| **A buyer or successor** | Your data, under this same policy | If Guangel is sold or transferred; we will tell you first |

Guangel is a communication tool. **We do not contact emergency services for you,** and we do not share your data with them unless the law requires it.

## 9. How long we keep data, and how to delete it

Alerts, locations and recordings are deleted automatically 30 days after the alert by default; you can change this to anywhere up to 180 days in Settings.

**Automatic deletion.** A daily job on our server permanently deletes every alert older than your setting, with its locations, route, recording and link record. Alerts sent by a missed check-in follow the same setting.

**Removed links.** When an alert is deleted, or a day after a replay link runs out, we keep only a one-way hash of its code and the time it was removed, for up to 180 days. This lets the page say "This link is no longer available". It contains nothing about you, your contacts or your location, and cannot be used to open the link.

**Delete on demand.** In History you can delete a single alert, or all of them, at any time. This removes its locations, route, recording and link straight away, and its links (the alert link and any replay links) stop working.

**Delete your account.** In the app, open the menu, then Settings, then **Delete account**. You will be asked for your password. We then permanently delete:

- your sign-in account;
- your contacts, groups and messages;
- all alerts, locations, routes, recordings and link records;
- your settings and checklist progress;
- the data stored on your phone by Guangel.

Deletion from our live systems is immediate. Google's encrypted backups may hold copies for up to 30 more days before they are overwritten. Crash and analytics data is not linked to your account and expires on its own schedule (see section 2).

If you cannot use the app, email haydelawal@gmail.com from the address on your account and we will delete it within 30 days. You can also use our account deletion page: [github.com/Haydelawal/privacy_policy/…/account_deletion_guangel_app.md](https://github.com/Haydelawal/privacy_policy/blob/main/account_deletion_guangel_app.md).

Uninstalling Guangel deletes the data on your phone, but **not** your cloud account. Delete your account first if you want everything removed.

## 10. Your rights and choices

You can see, change, export or delete your data, and withdraw any consent, whenever you like.

Most of this you can do yourself in the app:

- **See and correct:** contacts, groups, messages, settings and History are all visible and editable in the app.
- **Delete:** single alerts, all alerts, or your whole account (section 9).
- **Withdraw consent:** turn off automatic check-in texts, Cate tips or the app lock in Settings, or revoke any permission in your phone's Settings.
- **Limit analytics:** you can reset your advertising ID or turn off usage and diagnostics in your phone's Google settings.

Depending on where you live, you may also have the right to:

- get a copy of your data in a portable format;
- restrict or object to some processing;
- know which categories of data we collect and why (California CCPA/CPRA);
- lodge a complaint with your data protection authority, such as the Nigeria Data Protection Commission, the Spanish AEPD, your EU or UK supervisory authority, or the California Privacy Protection Agency.

To make any request, email haydelawal@gmail.com. We will reply within 30 days, and may ask you to confirm you own the account. We will never treat you differently for using your rights.

## 11. Other important information

**Children.** Guangel is not intended for anyone under 13, and we do not knowingly collect data from children. If you believe a child has created an account, email haydelawal@gmail.com and we will delete it.

**International transfers.** Your data is stored in the EU. Google may process some of it in other countries, such as the United States, under Standard Contractual Clauses and the EU-US Data Privacy Framework.

**Safety disclaimer.** Guangel helps you reach people you trust. It does not replace calling emergency services, does not contact the police or ambulance for you, and cannot guarantee that a message is delivered, that a link loads, or that anyone responds. If you are in immediate danger, call your local emergency number.

**Recording laws.** Some places require everyone's consent before a conversation is recorded. You are responsible for using the audio feature in line with the law where you are.

**Changes to this policy.** If we make an important change, we will tell you in the app before it takes effect and update the date at the top. Earlier versions are available on request.

**Contact us.** Hayde117, haydelawal@gmail.com, 8 Oladosu Sanusi Street, Lagos 102215, Nigeria.
