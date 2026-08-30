# Φιλοξένηση Privacy Policy / Terms of Service στο GitHub Pages

Τα stores (Google Play, App Store) θέλουν ΔΗΜΟΣΙΟ URL, όχι αρχείο μέσα στο app.
Βήματα:

1. Φτιάξε ένα public repo στο GitHub, π.χ. `fancytetris-legal`
   (ή χρησιμοποίησε ένα ήδη υπάρχον repo σου).

2. Ανέβασε μέσα:
   - `privacy-policy.html`  (μπορείς να αντιγράψεις το περιεχόμενο από
     `assets/legal/privacy_policy.html`)
   - `terms-of-service.html` (από `assets/legal/terms_of_service.html`)

3. Πήγαινε στο repo → Settings → Pages → Source: "Deploy from a branch"
   → Branch: main / root → Save.

4. Μετά από ~1 λεπτό, τα αρχεία σου θα είναι διαθέσιμα στο:
   `https://<το-github-username-σου>.github.io/<όνομα-repo>/privacy-policy.html`
   `https://<το-github-username-σου>.github.io/<όνομα-repo>/terms-of-service.html`

5. Άνοιξε το `lib/legal_screen.dart` και αντικατέστησε τα:
   ```dart
   const String kPrivacyPolicyUrl = 'https://YOUR-GITHUB-USERNAME.github.io/...';
   const String kTermsOfServiceUrl = 'https://YOUR-GITHUB-USERNAME.github.io/...';
   ```
   με τα πραγματικά URLs σου.

6. Βάλε τα ίδια URLs και στις φόρμες του Google Play Console / App Store
   Connect όπου ζητούν "Privacy Policy URL".

Μην ξεχάσεις να αντικαταστήσεις και το `YOUR-CONTACT-EMAIL@example.com` και
το `YOUR-COUNTRY/JURISDICTION` μέσα στα δύο .html αρχεία με τα πραγματικά σου
στοιχεία πριν τα δημοσιεύσεις.
