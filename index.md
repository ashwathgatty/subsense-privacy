# SubSense --- Privacy Policy

**Effective Date:** March 2026
**Last Updated:** March 2026

---

## 1. Introduction

SubSense ("we," "our," "us," or "the App") is an Android application that helps users track and manage their recurring subscriptions. We are committed to protecting your privacy and being transparent about how your data is handled.

This Privacy Policy explains what data SubSense collects, how that data is used, where it is stored, and what rights and controls you have over it. By installing and using SubSense, you agree to the practices described in this policy.

SubSense is developed by Akshan Technologies.

---

## 2. Data We Collect

### 2.1 Data Stored Locally on Your Device

The following data is created and stored entirely on your device in a local Room database. This data is **never** transmitted to our servers or any third party:

- **Subscription information** -- names, amounts, billing dates, billing cycles, categories, and user-added notes.
- **Notification scan metadata** -- source app package name, matched keyword, extracted amount, confidence score, and timestamp. This metadata is derived from on-device processing of push notifications; the raw notification text itself is **never** stored.
- **Price history** -- historical price data points for each tracked subscription, used to show price trend information.
- **User preferences** -- selected currency, alert and reminder settings, theme preferences, and other app configuration choices.

### 2.2 Data Collected by Third-Party SDKs

SubSense integrates the following third-party services, each of which may collect certain data as described below:

- **Firebase Analytics (Google)** -- Collects the Android Advertising ID (AAID), device model, operating system version, app version, and aggregated feature-usage event counts. Firebase Analytics does **not** collect or have access to your subscription content or notification data. For details, see the [Firebase Privacy Policy](https://firebase.google.com/support/privacy).

- **Firebase Crashlytics (Google)** -- Collects crash stack traces, device model, operating system version, and app state at the time of a crash. This data is used solely for identifying and fixing bugs. For details, see the [Crashlytics Data Collection documentation](https://firebase.google.com/docs/crashlytics/troubleshoot-faq).

- **Google AdMob** -- Displays banner and interstitial advertisements within the App. AdMob may collect advertising identifiers and other data in accordance with Google's advertising privacy policies. For details, see the [Google Advertising Privacy Policy](https://policies.google.com/technologies/ads).

### 2.3 Data We Do NOT Collect

SubSense does **not** collect, request, or access:

- Bank account details, credit card numbers, or any financial login credentials.
- SMS messages (the App does **not** request the `READ_SMS` permission).
- Contacts, photos, location, microphone, or camera data.
- Raw notification text (discarded immediately after on-device processing).
- Personal identification information such as your name, email address, or phone number (no account creation is required to use SubSense).

---

## 3. How We Use Data

| Data | Purpose | Stored Where |
| --- | --- | --- |
| Subscription information | Core app functionality -- tracking, reminders, spending summaries | Local device only |
| Notification scan metadata | Automatic detection of subscription renewals from push notifications | Local device only |
| Price history | Display price trends and alert users to price changes | Local device only |
| User preferences | Personalize the app experience | Local device only |
| Firebase Analytics data | Understand which features are used, guide app improvements | Google servers (aggregated) |
| Firebase Crashlytics data | Identify and fix crashes, improve app stability | Google servers |
| Google AdMob data | Display relevant advertisements to support free access to the App | Google servers |

---

## 4. Notification Access

SubSense uses Android's `NotificationListenerService` to read push notifications on your device. This section explains how that access works:

- **Purpose:** Automatically detect subscription-related notifications (such as renewal confirmations or payment receipts) so that subscription details can be captured without manual entry.
- **On-device processing only:** All notification reading and analysis happens entirely on your device. Notification content is **never** sent to any external server.
- **What is stored:** Only extracted metadata is retained -- specifically the source app package name, the matched keyword, the extracted amount, a confidence score, and a timestamp.
- **What is discarded:** The raw notification text is discarded immediately after processing. It is not stored in the local database or anywhere else.
- **User control:** You can revoke Notification Access at any time by navigating to **Android Settings > Apps > Special access > Notification access** and disabling SubSense.
- **Not required:** SubSense functions fully without Notification Access. If Notification Access is not granted, you can manage all subscriptions through manual entry.

---

## 5. Data Sharing

- **We do not sell, trade, rent, or otherwise share your subscription data with any third party.** Your subscription information, notification scan metadata, price history, and preferences remain on your device.
- Firebase Analytics and Firebase Crashlytics data is processed by Google under their respective privacy policies. This data consists of aggregated usage metrics and crash diagnostics -- it does not include your subscription content.
- Google AdMob may use advertising identifiers to serve personalized advertisements. You can opt out of ad personalization through **Android Settings > Privacy > Ads** (on Android 12+) or **Settings > Google > Ads** (on older versions). The exact path may vary by device manufacturer.

---

## 6. Data Storage and Security

- **Local storage:** All subscription data is stored on your device using Android's Room persistence library (an SQLite-based database). No custom remote servers or cloud databases are used.
- **Optional backup:** SubSense supports Android Auto Backup, which may back up app data to your personal Google Drive account. On Android 9+, this backup is end-to-end encrypted. On Android 8, backup encryption depends on having a device lock screen set. Backup is controlled entirely by you — you can manage or disable Auto Backup through **Android Settings > System > Backup**. Note: if Auto Backup is enabled, subscription data may leave your device to your Google Drive, which is an exception to the general "data never leaves your phone" principle.
- **Code protection:** Release builds of SubSense use ProGuard/R8 code obfuscation and minification to protect application code.
- **No remote access:** Because subscription data exists only on your device, there is no remote server that could be breached to expose your data.

---

## 7. Data Retention

- **Subscription data:** Retained on your device until you manually delete it or uninstall the App.
- **Notification scan log:** Automatically purged after 90 days to keep the local database efficient.
- **Price history:** The most recent 12 data points per subscription are retained; older data points are automatically removed.
- **Firebase Analytics and Crashlytics:** Data is retained on Google's servers according to Google's standard retention policies. Refer to [Google's data retention information](https://firebase.google.com/support/privacy) for specifics.

---

## 8. Your Rights and Controls

You have full control over your data in SubSense:

- **View your data:** All subscription data, notification scan logs, and price history are viewable within the App.
- **Export your data:** You may export your subscription data as CSV or JSON files (available as a Premium feature).
- **Delete all data:** Navigate to **Settings > Clear All Data** within the App to permanently erase all locally stored data.
- **Revoke Notification Access:** Go to **Android Settings > Apps > Special access > Notification access** and disable SubSense at any time.
- **Opt out of personalized ads:** Go to **Android Settings > Google > Ads** and enable the option to opt out of ads personalization.
- **Uninstall:** Uninstalling SubSense removes all locally stored data from your device. Note that any data previously backed up via Android Auto Backup may persist in your Google Drive until you manually remove it.

---

## 9. Children's Privacy

SubSense is not directed at children. Under the India DPDP Act 2023, the age threshold for children is 18 years. We do not knowingly collect personal data from children under 18. If you believe that a child under 18 has provided data through the App, please contact us at support@akshantech.com and we will take appropriate steps to delete such information.

---

## 10. Compliance with the India Digital Personal Data Protection Act, 2023 (DPDP Act)

SubSense is designed with the principles of the India Digital Personal Data Protection Act, 2023 in mind. The draft DPDP Rules were published for public consultation in January 2025, with the final Rules officially notified in November 2025. Phased enforcement timelines are set by the Central Government.

- **Local processing:** Personal data in the form of subscription information is processed and stored solely on the user's device. No personal data is transmitted to servers controlled by the developer.
- **Transparency:** This Privacy Policy discloses all data collection practices, including data collected by integrated third-party SDKs (Firebase Analytics, Firebase Crashlytics, and Google AdMob).
- **Consent-based processing:** Data processing is based on user consent, obtained through explicit in-app consent mechanisms (not merely app installation) and when the user enables Notification Access permission.
- **Right to access:** Users can view all their stored data within the App at any time.
- **Right to correction:** Users can edit and update their subscription data directly within the App.
- **Right to erasure:** Users can delete all personal data via **Settings > Clear All Data**, or by uninstalling the App.
- **Data Fiduciary contact:** For any queries related to data protection or to exercise your rights under the DPDP Act, please contact the Data Fiduciary at **support@akshantech.com**.

---

## 11. Compliance with Google Play Policies

SubSense complies with Google Play's Developer Program Policies, including:

- **Data Safety disclosures:** The App's Google Play listing includes accurate Data Safety information reflecting the practices described in this policy.
- **Notification Listener disclosure:** The use of `NotificationListenerService` is disclosed in the App's Play Store listing and is limited to the core functionality of detecting subscription notifications.
- **Ads policy:** Advertisements served through Google AdMob comply with Google's advertising policies.

---

## 12. Changes to This Policy

We may update this Privacy Policy from time to time to reflect changes in the App's functionality, third-party SDK updates, or applicable laws. When we make changes:

- The "Last Updated" date at the top of this policy will be revised.
- A notice will be posted within the App informing you of the update.
- Continued use of the App after changes are posted constitutes acceptance of the revised policy.

We encourage you to review this policy periodically.

---

## 13. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy or SubSense's data practices, please contact us:

- **Email:** support@akshantech.com
- **Google Play Store:** https://play.google.com/store/apps/details?id=com.subsense.app

---

*This Privacy Policy is written in English and governs the English-language version of SubSense.*
