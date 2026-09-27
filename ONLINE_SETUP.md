# Real online app setup

`online.html` में Firebase Web App configuration भरनी होगी। Firebase Console में:

1. नया Web App बनाएं और config copy करें।
2. Authentication → Email/Password enable करें।
3. Firestore Database बनाएं।
4. Storage बनाएं।
5. इस repository की `firestore.rules` और `storage.rules` publish करें।
6. `online.html` को Firebase Hosting, Vercel या Netlify पर deploy करें।

यह starter real email login, cloud video upload, online feed, likes और share link देता है। Production में moderation, report/block, pagination, thumbnail generation, rate limits, privacy policy, copyright checks और abuse protection जोड़ना जरूरी है। Firebase config browser में public होती है; सुरक्षा rules से आती है—service-account key कभी frontend में न डालें।

स्थानीय preview के लिए `python -m http.server 8080` चलाएं और `http://localhost:8080/online.html` खोलें। `file://` से ES modules/Firebase सही तरह काम नहीं कर सकते।
