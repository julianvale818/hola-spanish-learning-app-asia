# Hola Amigo Privacy Policy

**Effective date:** 8 September 2026<br>
**Status:** Offline-beta draft. The contact placeholder below must be replaced before public distribution.

Hola Amigo is a Spanish-learning Android app produced by **Light-Seeds Productions** and intended for people aged 13 and older. This policy explains what the current offline-beta app stores and how its optional voice features interact with Android services.

## Summary

- Hola Amigo does not require or provide an app account.
- The app has no advertising or analytics SDKs.
- The app does not request Android's internet permission and does not send learning progress to the developer.
- Learning progress and preferences are stored locally on the learner's device.
- A learner may explicitly export a JSON copy using Android's system document picker. Hola Amigo does not upload or receive the exported file.
- Pronunciation practice is optional. It uses the device's Android speech-recognition service only after the learner starts the feature and grants microphone access.
- Learners can avoid speech recognition and use the typed alternative.

## Information stored on the device

Hola Amigo stores learning information in a local Room database and local app preferences so that lessons and review can continue between sessions. This may include:

- the learner's selected interface language, study reason, daily goal, Spanish variety, and display preferences;
- completed lessons, passed checkpoints, placement status, unlocked progress, XP, streak, and last-practice day;
- exercise identifiers and review-scheduling information such as due dates, intervals, repetitions, and lapses;
- saved session state needed to resume an unfinished activity; and
- exercise-problem reports created by the learner, including the exercise identifier, selected issue category, optional report note, and creation time; and
- an append-only learning-event history containing a random event identifier, event type, activity mode and source identifier, local practice day, event time, course-content version, and—when the event represents an answer—the exercise identifier, correctness, and memory rating where applicable.

This information remains within the app's private storage. Exercise-problem reports and learning events are not uploaded or otherwise submitted in this beta. Hola Amigo does not include developer-operated accounts, cloud synchronization, ads, analytics, crash-reporting services, or social features in this beta.

Learning events are appended during normal use for rated answers, placement answers, and completed sessions. Earlier events are not edited through the app's normal learning flows. The recent-mistakes list, 28-day practice trail, and topic memory estimates are calculated locally from learning events, review state, completed lessons, and existing profile dates. These estimates are learning aids, not exam results or CEFR certification.

Android may include app data in a device or cloud backup when system backup is enabled. Backup storage and restoration are controlled by the learner's Android device, Google account, device manufacturer, and backup settings—not by Hola Amigo.

## Exporting learning data

The learner can choose **Settings > Export my learning data** and confirm the disclosure to create a portable JSON file. The export contains a summary plus the database-backed profile and learning preferences, lesson and checkpoint progress, achievements, mastery estimates, review schedule, active-session state, exercise-problem reports, and learning-event history. It may therefore contain optional free-text notes the learner entered in exercise reports. It does not contain the separately stored interface-language preference, passwords, raw microphone audio, or recognized speech transcripts; Hola Amigo does not store the latter two items.

Export uses Android's system document picker and does not require broad storage permission. Hola Amigo writes only to the destination explicitly selected by the learner. If the learner selects a cloud-backed or third-party storage provider, that provider may receive and process the file under its own terms. Once a file is outside Hola Amigo's private storage, its protection, sharing, retention, and deletion are controlled by the learner and the selected provider or recipient. Resetting or uninstalling Hola Amigo does not delete separately exported copies.

## Microphone and pronunciation practice

Hola Amigo requests microphone permission only when a learner chooses to start a pronunciation exercise. The app passes speech to the Android speech-recognition service selected on the device and receives a text transcript for immediate answer feedback.

Hola Amigo does not save the microphone recording or recognized transcript to its learning database and does not send either to a Hola Amigo server. Depending on the device, settings, installed language packs, and speech provider, Android's speech service may process speech on the device or may use the provider's online service. That provider's privacy terms and device settings apply to its processing. A learner may deny or revoke microphone access and use the typed alternative without losing access to the course.

## Device text-to-speech

Listening activities use the Android text-to-speech engine installed or selected on the device. Hola Amigo supplies the lesson phrase and requested Spanish locale to that system service. Voice availability, voice downloads, and any online processing are controlled by the device's text-to-speech provider and settings.

## Data collection, sharing, and sale

The current app code does not transmit personal information or learning records to the developer. The developer does not collect, share, or sell those records. Learner-directed export destinations, device-level speech services, and backup providers operate separately as described above.

## Retention and deletion

Local learning information, including the append-only learning-event history, remains on the device until the learner:

- uses **Settings > Reset all local progress** to clear Hola Amigo's local learning records and most profile preferences; or
- uninstalls Hola Amigo, which removes the app's on-device private storage under normal Android behavior.

An Android backup may retain a separate copy or restore data after reinstallation. Learners can manage or delete device backups through their Android or Google backup settings. Resetting progress before a new backup is created does not itself delete an older platform backup.

Hola Amigo provides a complete JSON export of the database-backed learning record but does not currently offer individual-history-event deletion or import. **Reset all local progress** attempts to clear legacy Hola Amigo preferences and all learner-owned Room tables; deletion within Room is transactional. The currently selected interface language is written back after reset so the app does not unexpectedly change languages. The app reports success only after both operations complete. If the operation fails, it reports that the reset was incomplete rather than presenting a false success. Reset and uninstall do not remove copies the learner previously exported elsewhere.

## Security

Hola Amigo relies on Android's private app storage and operating-system security controls. No method of storage is risk-free, so learners should keep their device software and lock-screen protection up to date.

## Children

Hola Amigo is positioned for learners aged 13 and older and is not directed to children under 13. The beta does not knowingly collect personal information from children because it does not transmit user data to the developer. A public release aimed at children would require a separate child-safety, consent, content, and legal review.

## Changes to this policy

This policy must be revised before adding accounts, cloud sync, analytics, advertising, third-party SDKs, hosted speech or AI features, or any other data transmission. Material changes should be shown in the app or store listing together with a new effective date.

## Contact

Public, non-sensitive questions may be submitted through the project issue tracker:<br>
https://github.com/julianvale818/hola-spanish-learning-app-asia/issues

Do not post personal, confidential, or sensitive information in a public GitHub issue. A dedicated private legal/privacy contact must be added before app-store publication where current policy or applicable law requires one. Because this beta has no accounts or developer-held learner records, the developer cannot identify or remotely delete a particular device's local data.

