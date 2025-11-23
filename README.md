# Simple Login Page

Μια minimal σελίδα εισόδου (login form) υλοποιημένη αποκλειστικά με **HTML** και **CSS**.  
Στόχος είναι ένα καθαρό, κεντραρισμένο login card με πεδία `username` και `password`, έτοιμο για χρήση σε μικρά projects ή ως βάση για πιο σύνθετα συστήματα αυθεντικοποίησης.

---

## Χαρακτηριστικά

- Κεντραρισμένη κάρτα login στη μέση της οθόνης
- Σκούρο, modern background (`#0b0f16`)
- Card-style layout με rounded corners και διακριτικό border
- Δύο βασικά πεδία:
  - `Username`
  - `Password`
- Placeholder κείμενα για καθοδήγηση του χρήστη
- Κουμπί **Login** με hover effect
- Responsive συμπεριφορά (δουλεύει και σε μικρές οθόνες / mobile)

---

## Τεχνολογίες

- **HTML5**
- **CSS3** (inline στο `<style>` του αρχείου)
- Χωρίς JavaScript (front-end μόνο, καθαρή φόρμα)

---

## Δομή αρχείου

Το project αποτελείται από ένα μόνο αρχείο:

- `index.html` (ή οποιοδήποτε άλλο όνομα επέλεξες, π.χ. `login.html`)

Βασικά sections:

- `<head>`  
  - Ορισμός χαρακτήρων (`UTF-8`)
  - Meta viewport για mobile
  - Inline CSS με όλα τα styles
- `<body>`  
  - Container `.card` που περιέχει:
    - Τίτλο `Login`
    - Μικρή περιγραφή
    - `<form>` με πεδία:
      - `input#username` (type `text`)
      - `input#password` (type `password`)
      - `button` για υποβολή

---

## Πώς το τρέχω

1. Αποθήκευσε τον κώδικα ως `index.html` (ή όποιο όνομα θέλεις με κατάληξη `.html`).
2. Άνοιξε το αρχείο με έναν browser (Chrome, Firefox, Edge κ.λπ.):
   - διπλό κλικ στο αρχείο **ή**
   - δεξί κλικ → *Open with* → επέλεξε τον browser.
3. Θα δεις τη σελίδα login με τη φόρμα στο κέντρο της οθόνης.

---

## Ενσωμάτωση σε πραγματικό σύστημα

Αυτή τη στιγμή η φόρμα είναι **στατική** και δεν στέλνει δεδομένα σε κάποιο backend.

Για να τη συνδέσεις με πραγματική αυθεντικοποίηση μπορείς:

- Να ορίσεις attribute `action` στο `<form>` με το URL του endpoint, π.χ.:

  ```html
  <form id="loginForm" action="/login" method="POST">
