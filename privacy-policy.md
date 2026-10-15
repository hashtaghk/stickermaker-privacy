# Privacy Policy — Sticker Maker

**Last updated: 15 October 2026**

This policy explains what the Sticker Maker app ("the app", "we") collects, why, and what
choices you have.

App package: `hk.android.free.truesticker.stickermakerforwhatsapp.stickercreater`
Publisher: HashtagHK
Contact: **admin@hashtaghk.com**

---

## 1. Photos, camera and the stickers you make

To make a sticker you choose a photo from your device or take one with the camera. The app
requests these permissions for that purpose only:

| Permission | Why |
|---|---|
| `READ_MEDIA_IMAGES` (Android 13+) | Show your gallery so you can pick a photo |
| `READ_EXTERNAL_STORAGE` (Android 12 and below) | Same, on older Android versions |
| `CAMERA` | Take a new photo, only when you open the camera screen |
| `INTERNET` | Personal sticker packs, purchases, ads, crash reporting, analytics, and cloud backup |

**The sticker editor works on your device.** Cropping, cutting out, adding text and the automatic
background removal all run locally. The background-removal model runs on-device through Google
Play Services and does not send your photo to a server.

**Finished stickers are stored on your device**, in the app's private storage.

Your photos leave the device in two cases only, both started by you: making a personal sticker
pack (section 2) and cloud backup (section 3).

## 2. Personal sticker packs

Personal sticker packs turn photos of one person or pet into a sticker pack of that face. To
make one:

- **You choose 10–20 photos.** Before anything is uploaded, the app checks each photo on your
  device for a clear face, using Google ML Kit face detection. That check runs locally and is not
  sent anywhere.
- **The photos are uploaded** to Google Firebase Storage, along with the name you give the
  pack and the style you picked.
- **Our server sends the photos to Google Cloud Vertex AI**, which generates the sticker images.
  Vertex AI processes them on our behalf under Google Cloud's terms, which do not allow Google to
  use them to train its models. The photos are not used for anything other than making your pack.
- **The finished stickers** are stored in Firebase Storage so the app can download them, and are
  then saved on your device like any other pack.

To keep track of your packs and credits without asking you to sign in, the app creates an
**anonymous account ID** (Firebase Authentication). It is not linked to your name, email or
Google account. Your uploaded photos and generated stickers are stored in a folder under that ID,
and only our server can read them.

We do not use your photos, or the faces in them, to identify you, and we do not share them with
anyone except the Google Cloud services above that make the pack.

## 3. Cloud backup

If you use **Export / Backup**, the app uploads your sticker images to Google Firebase Storage so
you can restore them later or move them to another phone. They are stored in a folder linked to
your signed-in account.

This only happens when you choose to export. If you never use Export/Backup, your images are not
uploaded.

**Restore** downloads those files back to your device.

## 4. Signing in

Backup uses Google sign-in. If you sign in, we receive your **email address**. It is used to
identify your backup folder so you can restore your own stickers. We do not use it for marketing.

Personal sticker packs do not require you to sign in — they use the anonymous ID described in
section 2.

## 5. Purchases

Personal sticker packs are paid for through **Google Play Billing**. We never see your card or
payment details; Google handles payment.

When you buy, the app sends the purchase's **Google Play purchase token** to our server, which
checks it with Google and adds the credits to your anonymous ID. We store the token, the product
you bought, and when it was redeemed, so that one purchase cannot be spent twice and so that a
subscription renews correctly.

## 6. Sharing to WhatsApp and Telegram

When you add a sticker pack to WhatsApp or Telegram, the app hands those stickers to that app at
your request. Once shared, the receiving app's own privacy policy applies. We do not control what
they do with it.

## 7. Analytics and crash reporting

We use **Google Firebase Analytics** to understand which features are used — for example, that a
sticker was created, a pack was added to WhatsApp, or a purchase succeeded. These are records of
actions, not the content of your photos or stickers. If you installed the app from a link someone
shared, the app also records that link's referral code once, so we know the link worked.

We use **Firebase Crashlytics** to receive crash reports so we can fix bugs. A crash report
includes the error, the device model, and the Android version. It does not include your photos.

We also use **Firebase Remote Config** to adjust app settings without an update, and **Firebase
App Check** with Google Play Integrity to make sure requests to our server come from the genuine
app. These send technical information about the app and device, not your content.

## 8. Advertising

The app shows ads through **Google AdMob**. AdMob may use your device's **advertising ID** and
an approximate location derived from your IP address to show relevant ads, to limit repeated
ads, and to prevent fraud. You can reset or delete the advertising ID at any time in
**Settings → Privacy → Ads** on your device, and you can opt out of ad personalisation there.

Where the law requires it, the app asks for your consent before showing personalised ads.

## 9. Third-party services

These services process data on our behalf, under their own privacy policies:

- Google Firebase — Analytics, Crashlytics, Authentication, Storage, Remote Config, App Check:
  https://firebase.google.com/support/privacy
- Google Cloud Vertex AI (personal sticker pack generation):
  https://cloud.google.com/terms/cloud-privacy-notice
- Google Play Billing: https://policies.google.com/privacy
- Google AdMob: https://policies.google.com/technologies/ads
- Google Sign-In, ML Kit and Play Services: https://policies.google.com/privacy

## 10. Children

The app is not directed at children under 13, and we do not knowingly collect personal
information from them. If you believe a child has provided us personal information, contact us
and we will delete it.

## 11. Keeping and deleting your data

- **On your device:** uninstalling the app removes the stickers and settings it stored locally.
- **Personal sticker packs:** the photos you uploaded and the generated stickers are kept so your
  pack can be downloaded again. To have them deleted, email **admin@hashtaghk.com** with the
  Google Play order number from your purchase receipt and roughly when you made the pack. We will
  delete the photos and stickers for that account.
- **Cloud backup:** to delete backups you exported, email **admin@hashtaghk.com** from the address
  you signed in with and ask for deletion. We will delete the backup folder for that account.
- **Purchase records** are kept for as long as needed to honour your credits and for our
  accounting obligations.
- Analytics and crash data are retained according to Google Firebase's standard retention
  periods.

## 12. Security

All data sent from the app to Firebase and Google Cloud travels over encrypted connections
(HTTPS/TLS). Uploaded photos, generated stickers and backups are stored in folders scoped to your
account, and storage rules stop other users from reading them. No system is perfectly secure, and
we cannot guarantee absolute security.

## 13. Changes to this policy

If this policy changes we will update this page and the "Last updated" date above. Significant
changes will be highlighted in the app or the store listing.

## 14. Contact

Questions or data-deletion requests: **admin@hashtaghk.com**
