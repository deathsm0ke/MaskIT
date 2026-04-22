# Privacy Policy — MaskID

**Effective date:** 2026-04-22
**Developer:** Amrit Natarajan — Chennai, India
**Contact:** sushant.bhandi94@gmail.com

## Plain-English summary

- MaskID processes your photo **entirely on your device**.
- Your ID image, the recognised text, and the masked output **never leave your phone**.
- We do not collect, store, or transmit any image, document number, name, address, or biometric data.
- We do not require you to create an account.
- The only network traffic MaskID makes is to Google AdMob to request a single banner/interstitial ad — the same network contract every AdMob-funded Android app has.

## What MaskID does

MaskID is a free Android utility that helps you mask sensitive ID numbers in a photo before you share it with a hotel, SIM store, courier, gym, landlord, or similar third party. It detects common identity-document numbers across regions, including but not limited to:

- **India** — Aadhaar, PAN, Driving Licence, Voter ID
- **United States** — SSN, ITIN
- **United Kingdom** — National Insurance Number (NINO), NHS Number
- **Canada** — Social Insurance Number (SIN)
- **Australia** — Tax File Number (TFN), Medicare
- **Worldwide** — ICAO-format passport numbers, credit/debit card numbers

By default MaskID uses your device locale to pick which IDs to look for; you can switch region at any time from the Mask screen.

MaskID then:

1. Receives an image either through Android's share sheet or the Photo Picker.
2. Runs Google ML Kit's on-device text recognizer to locate ID-number-shaped text.
3. Draws a black rectangle over the sensitive digits (first 8 of 12 for Aadhaar, 5 letters of a PAN, etc.).
4. Stamps a watermark showing the purpose and date, so the image cannot be reused for another purpose later.
5. Hands the masked image back to you via the Android share sheet.

## Data we process

| Data | Collected? | Stored off-device? | Shared? |
|---|---|---|---|
| Your ID photo | Read only during active processing | No | No |
| Extracted text | Held in RAM only, discarded when processing ends | No | No |
| Masked image | Written to the app's private cache; you may re-share it via any app you choose | No | Only where you explicitly share it |
| Share history (purpose, doc type, timestamp) | Stored in an app-private database on your phone | No | No |
| Advertising identifier (AdID) | Accessed by the Google AdMob SDK under Google's standard policy | Sent to Google AdMob only | By Google, per AdMob policy |
| Personal info (name, email, phone) | Never collected | N/A | N/A |
| Location | Never accessed | N/A | N/A |
| Contacts, Calendar, Messages | Never accessed | N/A | N/A |

## Permissions we request

- `INTERNET` / `ACCESS_NETWORK_STATE` — required by the AdMob SDK only.
- `com.google.android.gms.permission.AD_ID` — Google's mandatory declaration when AdMob is used on Android 13+.

We do **not** request `READ_MEDIA_IMAGES`, `READ_EXTERNAL_STORAGE`, `MANAGE_EXTERNAL_STORAGE`, `CAMERA`, `CONTACTS`, `LOCATION`, `READ_SMS`, or `PHONE_STATE`. All image access flows through Android's Photo Picker or explicit share intents, which require no runtime permission.

## Advertising

MaskID shows at most one Google AdMob interstitial per app launch to cover development costs. AdMob may collect device and ad-interaction data per its own [privacy terms](https://policies.google.com/technologies/ads). You can opt out of personalised ads in your Android settings (Settings → Privacy → Ads → Delete advertising ID).

## Children's data

MaskID is not directed at children under 13. We do not knowingly collect data from children.

## Data retention

Share-history entries stay on your phone until you delete them from the app (History → Clear) or uninstall MaskID. The masked image written to the share cache is kept for the current and previous ~5 share actions and is auto-deleted thereafter.

## Your rights

Because we do not collect personal data, there is nothing stored with us for you to request, correct, or delete. Uninstalling MaskID removes all app data from your device.

## Changes to this policy

We will post material changes to this document before they take effect and update the effective date above.

## Contact

For any privacy question, email **sushant.bhandi94@gmail.com**.
