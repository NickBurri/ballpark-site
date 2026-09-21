# Ballpark Privacy Policy

**Effective date: September 21, 2026**

Ballpark is a meal and macro tracking application for iPhone. This Privacy Policy explains what information Ballpark processes, why it is processed, where it is stored, which service providers may process it, and the choices available to you.

## 1. Developer and Data Controller

Ballpark is developed and operated by:

**Nick Burri**  
Switzerland  
Email: [ballparkmacrotracker@icloud.com](mailto:ballparkmacrotracker@icloud.com)

Nick Burri is the data controller for personal data processed through Ballpark's backend service.

Ballpark does not require an account. Most information is stored only on your device and is not accessible to the developer.

## 2. Summary

Ballpark is designed with data minimization in mind:

- Your meals, nutrition goals, settings, and synced weight measurements are stored locally on your iPhone.
- AI processing is optional and requires your explicit permission.
- When AI processing is enabled, the information needed for the requested AI feature is sent through Ballpark's backend service to OpenAI.
- Ballpark does not contain third-party advertising.
- Ballpark does not sell personal data.
- Ballpark does not track you across apps or websites.
- HealthKit information is not sent to OpenAI or Ballpark's backend.
- Ballpark's backend does not intentionally store meal descriptions, photographs, or audio recordings after processing.

## 3. Information Stored on Your Device

Ballpark may store the following information locally on your iPhone:

- meal entries;
- meal descriptions, titles, summaries, and assumptions;
- estimated calories and macronutrients;
- reusable or saved meals;
- nutrition goals;
- incomplete-day markers;
- reminder preferences;
- app and display settings;
- your AI-processing consent preference;
- Apple Health weight measurements, if you enable Apple Health weight sync; and
- technical preferences needed for the app to operate.

This information is used to provide Ballpark's core features, including meal tracking, daily summaries, history, trends, nutrition goals, maintenance-calorie estimates, reminders, backups, and CSV exports.

This locally stored information is not automatically transmitted to the developer.

## 4. AI Meal Estimates and Voice Processing

Ballpark can provide meal estimates using:

- meal descriptions and clarifications you enter;
- photographs you select or take;
- your language and measurement-unit preferences; and
- recorded audio when OpenAI voice transcription is enabled.

When you explicitly allow OpenAI processing, the information required for the feature you requested is transmitted:

1. from your device to Ballpark's backend service, which is hosted by Cloudflare; and
2. from Ballpark's backend service to OpenAI for processing.

This information is used only to:

- estimate calories and macronutrients from meal descriptions or photographs;
- generate a short meal title, summary, confidence indication, and assumptions; or
- transcribe or refine a spoken meal description.

Meal photographs are used for the current estimate and are not saved as part of your meal history by Ballpark.

Ballpark configures OpenAI response storage as disabled where the relevant API supports that setting.

## 5. OpenAI

Ballpark uses OpenAI, L.L.C. as an AI-processing provider.

Depending on the feature, OpenAI may receive:

- meal descriptions and clarifications;
- selected meal photographs;
- recorded meal-description audio;
- language preferences;
- measurement-unit preferences; and
- instructions needed to generate the requested result.

OpenAI states that data submitted through its API is not used to train its models by default. OpenAI may, however, retain certain API inputs, outputs, and related metadata in abuse-monitoring logs for up to 30 days, unless longer retention is required by law. Retention may vary by API endpoint and by OpenAI's current data-control configuration.

For more information, see:

- [OpenAI API Data Controls](https://platform.openai.com/docs/guides/your-data)
- [OpenAI Privacy Policy](https://openai.com/policies/privacy-policy)

Ballpark does not permit OpenAI to use this information for advertising or cross-app tracking.

## 6. Cloudflare and Ballpark's Backend Service

Ballpark uses Cloudflare, Inc. to host and protect its backend service.

Cloudflare processes requests in order to:

- securely route requests between Ballpark and OpenAI;
- verify that access to paid AI features is authorized;
- apply rate limits;
- reject duplicate or replayed requests;
- monitor reliability and errors; and
- protect the service against misuse.

Depending on the request, Cloudflare may process:

- the meal description, photograph, or audio needed for the requested AI operation;
- a randomly generated Ballpark installation identifier;
- a randomly generated request identifier;
- the app version;
- network information such as an IP address and approximate request location;
- a short-lived authorization token;
- StoreKit subscription transaction information;
- the request endpoint, response status, timing, and error category; and
- pseudonymous hashes derived from the installation identifier and the original App Store transaction identifier.

The installation identifier is randomly generated by Ballpark and is not an advertising identifier. It is used for service operation, security, and authorization.

Ballpark's backend verifies subscription information with Apple before allowing access to paid AI features. It processes the product identifier, bundle identifier, transaction identifier, subscription expiration, revocation status, and App Store environment for this purpose.

### Backend content retention

Ballpark's backend does not intentionally write meal descriptions, photographs, audio recordings, or AI responses to its operational logs or to a persistent application database.

Meal descriptions, photographs, and audio pass through the backend temporarily while the request is being processed.

Short-lived security information is retained as follows:

- authorization sessions are valid for approximately 15 minutes;
- request identifiers used for replay protection are cached for approximately 20 minutes; and
- rate-limiting information is retained only as needed to enforce the configured request limits.

### Operational logs

Ballpark records limited technical logs for reliability, security, debugging, and abuse prevention. These logs may include:

- a server-generated request identifier;
- the requested API path;
- response status;
- request duration;
- error category;
- pseudonymous installation and subscription hashes; and
- subscription-verification events.

Ballpark's custom log messages do not intentionally include meal descriptions, photographs, audio recordings, complete installation identifiers, complete transaction identifiers, authorization tokens, or OpenAI credentials.

Cloudflare may also generate infrastructure and request metadata as part of operating the Worker service. Cloudflare Workers logs are retained according to the applicable Cloudflare plan and configuration, currently for no longer than seven days. Aggregated service metrics may remain available for up to approximately three months.

For more information, see the [Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/).

## 7. Apple Health and Weight Information

If you enable Apple Health weight sync, Ballpark requests read-only access to body-weight information from HealthKit.

Ballpark uses this information to:

- show weight history and trends; and
- estimate maintenance calories based on logged nutrition and weight changes.

Ballpark:

- does not write weight information to Apple Health;
- does not send HealthKit weight information to OpenAI;
- does not send HealthKit weight information to Ballpark's backend;
- does not use HealthKit information for advertising, marketing, data mining, or cross-app tracking; and
- does not sell HealthKit information.

Synced weight measurements are cached locally on your device so Ballpark can show trends without repeatedly requesting your complete HealthKit history.

Turning off weight sync stops Ballpark from requesting new weight measurements, but does not delete measurements already cached locally. The cached measurements remain on your device until you use **Delete Synced Weight Data** in Settings or uninstall Ballpark. Removing Ballpark's local cache does not delete the original measurements from Apple Health.

Each time weight sync runs, Ballpark reconciles its local cache with the Apple Health weight measurements currently available to the app. If an available measurement was deleted from Apple Health, its cached copy is removed from Ballpark during the next successful sync. If HealthKit access is restricted, Ballpark can reconcile only the measurements Apple Health makes available to it.

You can revoke Ballpark's access to HealthKit at any time in the Health app or iOS Settings. Revoking access prevents future access but does not automatically remove information previously cached by Ballpark.

## 8. Camera, Photo Library, Microphone, and Speech Recognition

Ballpark may request permission to use:

- the camera, so you can take a meal photograph;
- the photo picker or photo library, so you can select a meal image;
- the microphone, so you can record a meal description; and
- Apple speech recognition, so spoken input can be converted to text.

These permissions are used only when you choose the related feature.

When Apple dictation or speech recognition is used, Apple may process audio or transcription information according to Apple's privacy practices and your device settings.

You can manage these permissions in iOS Settings.

## 9. Subscription Information

Ballpark uses Apple StoreKit to offer and manage the Ballpark AI subscription.

Apple processes purchases, payment information, subscription status, refunds, and billing. Ballpark does not receive or store your complete payment-card information.

To protect paid AI features, Ballpark sends Apple-signed subscription transaction information to Ballpark's backend. The backend validates that information using Apple's App Store Server API.

Ballpark uses the verified subscription information only to:

- confirm access to Ballpark AI;
- issue a short-lived authorization session;
- prevent unauthorized use of the AI service;
- apply subscription-level rate limits; and
- investigate technical failures or abuse.

For information about Apple's handling of purchase and subscription information, see [Apple's Privacy Policy](https://www.apple.com/legal/privacy/).

## 10. Notifications

If you enable meal reminders, Ballpark schedules local notifications on your device.

Reminder times and notification preferences are stored locally. Ballpark does not use a remote push-notification service for these reminders.

You can disable notifications in Ballpark or in iOS Settings.

## 11. Backups and Exports

Ballpark allows you to create JSON backups and CSV exports.

Depending on the export format, these files may contain:

- meal entries;
- estimated nutrition information;
- saved meals;
- goals;
- incomplete-day markers; and
- other information shown in the export.

Exports are created only when you request them. After an export is created, you decide where it is saved or shared. Copies stored in Files, iCloud Drive, email, or another service are controlled by you and by the provider of that destination.

Deleting information inside Ballpark does not automatically delete copies you previously exported.

## 12. Retention and Deletion

### Meal information

Individual meals and saved meals can be deleted inside Ballpark.

You can use the clear-meal-data function in Settings to permanently delete all meal entries and reusable meals stored by Ballpark. This action does not delete your goals, app settings, or locally cached HealthKit weight measurements.

### AI consent

You can withdraw permission for OpenAI processing at any time:

1. Open **Ballpark**.
2. Open **Settings**.
3. Select **Privacy & Data**.
4. Select **Turn Off OpenAI Processing**.

After you turn it off, Ballpark stops sending new meal descriptions, photographs, and audio recordings to Ballpark's backend and OpenAI. Manual meal entry remains available, and voice entry can continue using Apple dictation.

Withdrawal does not affect processing that was completed before consent was withdrawn or information that a provider must temporarily retain for security or legal reasons.

### HealthKit information

You can stop future weight syncing from Ballpark's Settings and revoke HealthKit permission through Apple Health or iOS Settings.

Locally cached weight measurements remain on the device after syncing is turned off. You can permanently remove them using **Delete Synced Weight Data** in Settings or by uninstalling Ballpark. This deletes only Ballpark's cache and does not change the original data in Apple Health. A later sync can import measurements that remain available in Apple Health again.

### Complete local deletion

Because Ballpark does not use user accounts or maintain a server-side meal database, the developer generally cannot remotely access or delete information stored on your device.

To remove all locally stored Ballpark information, delete Ballpark from your iPhone. Information included in an iCloud or device backup may remain in that backup according to Apple's backup-retention behavior.

### Provider retention

Information already transmitted to OpenAI or processed in Cloudflare infrastructure may remain for the limited periods described in this policy, including security, abuse-monitoring, operational-log, and legal-retention periods.

If you have a deletion or privacy question, contact [ballparkmacrotracker@icloud.com](mailto:ballparkmacrotracker@icloud.com). Because Ballpark has no user accounts, you may need to provide a relevant request identifier or other information that allows a backend event to be located. Ballpark may not be able to associate an email address with app activity if no identifying information was originally collected.

## 13. Purposes and Legal Bases

Depending on applicable law, Ballpark processes information on the following bases:

- **Consent:** for optional OpenAI processing, camera access, microphone access, speech recognition, photo selection, HealthKit access, and notifications.
- **Performance of the requested service:** to provide meal estimates, voice transcription, subscription features, backups, exports, and other functions you request.
- **Legitimate interests:** to secure the backend, prevent fraud and abuse, enforce rate limits, diagnose failures, and maintain service reliability.
- **Legal obligations:** when processing or retention is required by applicable law.

Where processing is based on consent, you may withdraw that consent at any time. Withdrawal does not affect processing that was lawful before withdrawal.

## 14. Service Providers and International Processing

Ballpark relies on the following principal providers:

- **Apple:** app distribution, StoreKit subscriptions, App Store Server API verification, HealthKit, device permissions, speech recognition, and optional device or iCloud backups.
- **Cloudflare:** backend hosting, network delivery, security, rate limiting, replay protection, and operational logging.
- **OpenAI:** meal estimation and optional audio transcription or refinement.

These providers may process information in countries other than the country where you live, including the United States. They process information under their applicable contractual, privacy, and security obligations.

Ballpark selects providers that maintain safeguards intended to protect information consistently with this policy and applicable data-protection requirements.

Ballpark does not authorize these providers to use Ballpark data for third-party advertising or cross-app tracking.

## 15. No Advertising, Sale, or Cross-App Tracking

Ballpark does not:

- display third-party advertisements;
- sell or rent personal information;
- use third-party advertising SDKs;
- create advertising profiles;
- share information with data brokers; or
- track users across apps or websites owned by other companies.

Ballpark does not use Apple's advertising identifier.

## 16. Security

Ballpark uses reasonable technical and organizational measures intended to protect transmitted information, including HTTPS encryption, server-side subscription verification, short-lived authorization sessions, request replay protection, rate limiting, restricted provider credentials, and minimized operational logging.

No transmission or storage system can be guaranteed to be completely secure. You should protect access to your iPhone, Apple Account, device backups, and exported Ballpark files.

## 17. Children

Ballpark is not specifically directed to children. Ballpark does not knowingly collect information from children through an account system because the app does not have user accounts.

If you believe a child has provided personal information through an AI request in a manner that requires deletion or other action, contact [ballparkmacrotracker@icloud.com](mailto:ballparkmacrotracker@icloud.com).

## 18. Your Privacy Rights

Depending on where you live, you may have rights concerning personal information, including rights to:

- receive information about processing;
- access personal information;
- correct inaccurate information;
- request deletion;
- restrict or object to certain processing;
- withdraw consent; and
- lodge a complaint with a competent data-protection authority.

Most Ballpark information is stored only on your device and can be accessed, corrected, exported, or deleted directly through the app.

Because Ballpark does not use accounts and does not intentionally log directly identifying meal content, the developer may be unable to associate backend activity with a particular person without additional information from that person.

To make a privacy request, email [ballparkmacrotracker@icloud.com](mailto:ballparkmacrotracker@icloud.com).

## 19. Changes to This Policy

This policy may be updated when Ballpark's features, providers, data practices, or legal obligations change.

The latest version will be published at the same privacy-policy URL with a revised effective date. If a change materially affects how Ballpark processes information, notice will be provided in the app or through another appropriate method before the change takes effect where required by law.

Continued use of optional features after an updated notice does not replace consent where new consent is legally required.

## 20. Approximate Nutrition Information

Ballpark's nutrition estimates are approximate and may be inaccurate.

They are provided for general informational purposes only and are not medical advice. They should not be used to diagnose, treat, or manage a medical condition.

## 21. Contact

For questions, privacy requests, or concerns about this policy, contact:

**Nick Burri**  
Switzerland  
Email: [ballparkmacrotracker@icloud.com](mailto:ballparkmacrotracker@icloud.com)
