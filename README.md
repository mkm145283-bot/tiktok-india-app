# Bharat Short Video App

यह repository अभी frontend demo और real-online app के foundation के साथ शुरू की गई है।

## Run locally

```bash
npm install
npm run dev
```

## Firebase जोड़ना

1. Firebase Console में नया project बनाएं।
2. Authentication में Email/Password और Google provider enable करें।
3. Firestore Database और Storage बनाएं।
4. `firebase-config.example.js` की copy बनाकर `firebase-config.js` नाम दें।
5. अपनी Firebase web configuration भरें।

`firebase-config.js` को public repository में commit न करें।

## Important

300 MB का package बनाना लक्ष्य नहीं होना चाहिए। App का code हल्का रखा जाता है; users की uploaded videos cloud storage में रहती हैं। असली production features—authentication, moderation, upload limits, comments, notifications, live streaming और payments—के लिए Firebase configuration, security rules और deployment account आवश्यक हैं।
