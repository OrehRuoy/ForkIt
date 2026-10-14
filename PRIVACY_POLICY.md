# Privacy Policy for **Fork It**

**Last updated:** October 14, 2026  

**Package name:** `com.forkit.randomrestaurant`  

**Public page:** [https://orehruoy.github.io/ForkIt/](https://orehruoy.github.io/ForkIt/)

This Privacy Policy describes how the mobile application **Fork It** ("the App") handles information when you use it. By using the App, you agree to this policy.

---

## 1. Who we are

The App is provided by:

**Brock Hall**  
**Contact email:** hallanhype@gmail.com  

---

## 2. Summary

- The App does **not** require an account, and it does not offer sign-in.
- The App uses your device location to find places open near you. That location is sent only to Fork It's server so it can ask Google Places for nearby results. We do not store your location.
- Place details (name, address, rating, photos, reviews) come from **Google Places** through that server. The App may open links in **Google Maps** or a delivery search when you tap those buttons.
- Settings, history, favorites, streak, and reminder times stay **on your device**.
- Meal reminders are optional and stay off until you turn them on. They are scheduled on the device.
- The App shows ads through **Google AdMob** (banner, interstitial, and optional rewarded). It does not show app-open ads. **Fork It Plus**, bought through Google Play, turns these ads off.
- The App uses **Firebase App Check** and **Firebase Analytics**. Analytics events do not include coordinates, place names, or other information that identifies you.
- A random install id is sent with place searches so the server can limit request volume. The server stores those request counts. It does not store your location, history, or favorites.

---

## 3. Information the App processes

### 3.1 Data stored locally on your device

The App stores data in app-local storage (for example, Godot `user://` data). This data stays on the device:

- Search radius and whether device location is on
- Restaurant preference toggles, exclusion filters, and excluded names you add
- Place thumbs-up and thumbs-down choices used to influence future picks
- History, favorites, hidden places, and your fork streak
- Whether meal reminders are on, and the lunch and dinner times you pick
- Whether Fork It Plus is owned on this device
- A random install id used only for request limits

Clearing the App's data or uninstalling it removes this local data, subject to your device backup and restore behavior.

### 3.2 Location data

Before the first location prompt, the App explains that location is used to find places open near you and is not stored.

The App then asks the operating system for a current location and sends that latitude and longitude to Fork It's server (`fork-it-restaurant-finder`, Cloud Functions in `us-central1`) together with the install id. The server forwards the search to Google Places and does not write the coordinates to a database.

Approximate distance shown in the App is calculated on the device. Nearby search cannot run if you deny location permission.

### 3.3 Network requests and third-party services

When you use the App, it can send requests to these services:

| Service | Purpose |
|---|---|
| **Fork It server (Cloud Functions)** | Receives location and search options, checks App Check, applies rate limits, and calls Google Places. It does not store coordinates. It stores request counts keyed by the install id. |
| **Google Places API** | Nearby places and place metadata (name, address, rating, user rating count, reviews, photos, map URI). |
| **Google Maps / maps URLs** | Open navigation when you tap "Take me there". |
| **Google-hosted image endpoints** | Load place photos for result cards. |
| **Google Play Billing** | Handle the Fork It Plus purchase. |
| **Sites or apps you open** | Delivery search and share actions open a link or the system share sheet only when you tap them. |

These services receive standard technical request data (such as IP address, device or network metadata, and request timing) according to their own policies.

### 3.4 Advertising (Google AdMob)

The App uses **Google AdMob** to show banner, interstitial, and optional rewarded ads. It does not show app-open ads. Ads load only after Google's consent flow finishes. Fork It Plus turns these ads off.

**Firebase Analytics** records product events such as a fork, a result, or an ad outcome. Event parameters stay small and do not include coordinates, names, or other personal details.

**Firebase App Check** proves the request comes from the Fork It app. Debug builds print an App Check debug token in logcat so it can be registered. Release builds use Play Integrity.

Google may process identifiers (including advertising ID), device and app information, and ad interaction data to provide, measure, and protect ad services, and to personalize ads where allowed.

Please review:

- [Google Privacy Policy](https://policies.google.com/privacy)
- [How Google uses information from sites or apps that use our services](https://policies.google.com/technologies/partner-sites)

Depending on your region and device, you may be able to adjust ad personalization in your Google account and device Ads settings.

### 3.5 Purchases

Fork It Plus is sold through Google Play. Google Play processes the payment. Fork It does not receive your card number. The App stores on the device whether Plus is owned, so ads stay off and the higher daily fork limit applies.

### 3.6 Meal reminders

Reminders are off until you enable them in Settings. The times you choose are stored on the device. Android shows the notifications locally. Those times are not sent to Fork It's server.

---

## 4. We do not sell your personal data

We do not sell your personal information. We do not operate an account server. Favorites, history, and settings stay on this device. The server keeps rate-limit counts for the install id and does not keep a profile of places you picked.

---

## 5. Children's privacy

The App is not directed to children under 13 (or the minimum age required in your country). We do not knowingly collect personal information directly for our own backend services. Third-party services (for example Google APIs and AdMob) may process technical data as part of normal app operation.

---

## 6. Security

We aim to keep user settings local to the device. Requests to Fork It's server use HTTPS. No transmission or storage method is 100% secure.

---

## 7. International users

If you use the App outside your home country, data handled by Google, Firebase, or Play services may be processed in other countries where those services or their infrastructure operate.

---

## 8. Your choices

- **Location:** Deny location permission. Fork It cannot search nearby without it.
- **Reminders:** Leave them off, or turn them off in Settings.
- **Ads:** Use device and Google settings to limit ad personalization where available. Fork It Plus removes the App's ads.
- **Local data:** Clear app data or uninstall to remove settings, favorites, history, and the install id stored on the device.
- **Questions:** Contact us at the email listed above.

---

## 9. Changes to this policy

We may update this Privacy Policy from time to time. The "Last updated" date will change when we do. Continued use of the App after updates means you accept the revised policy.

---

## 10. Third-party policy references

- Google Privacy Policy: [https://policies.google.com/privacy](https://policies.google.com/privacy)
- Google partner sites/apps data use: [https://policies.google.com/technologies/partner-sites](https://policies.google.com/technologies/partner-sites)
