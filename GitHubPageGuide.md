# Οδηγός Δημιουργίας Repository στο GitHub και Εμφάνισης Στατικής Ιστοσελίδας στο GitHub Pages

Ακολουθεί ένας εύχρηστος οδηγός για να δημιουργήσεις ένα repository στο GitHub, να ανεβάσεις τον κώδικά σου για μια στατική ιστοσελίδα και να τη δεις ζωντανά μέσω του GitHub Pages.

## Εγγραφή και Ρύθμιση GitHub

* Επισκέψου το [GitHub](https://github.com) και κάνε εγγραφή ή σύνδεση.

* Αν δεν το έχεις κάνει ήδη, κατέβασε και εγκατέστησε το [Git](https://git-scm.com/) στον υπολογιστή σου.

  ## Δημιουργία Repository

* **Επιλογή 1: Δημιουργία Private Repository στο GitHub και Κλωνοποίηση Τοπικά**

  * Στο GitHub, κάνε κλικ στο εικονίδιο **\+** στην πάνω δεξιά γωνία και επίλεξε **New repository**.

  * Δώσε όνομα στο repository (π.χ., `skillcyprus-website`).

  * Επίλεξε **Initialize this repository with a README** για αρχικοποίηση με ένα αρχείο README.

  * Κάνε κλικ στο **Create repository**.

  * Κλωνοποίησε το repository τοπικά

`git clone https://github.com/<username>/<repo-name>.git`

* Συνέχισε στο επόμενο βήμα για να προσθέσεις τα αρχεία σου.

* **Επιλογή 2: Δημιουργία Repository Τοπικά και Σύνδεση με GitHub**

  * Δημιούργησε έναν νέο φάκελο στον υπολογιστή σου και μπες σε αυτόν:

`mkdir skillcyprus-website`  
`cd skillcyprus-website`

* Αρχικοποίησε ένα νέο Git repository:

`git init`

* Δημιούργησε ένα αρχείο `README.md` ή το βασικό αρχείο της σελίδας σου `index.html`:

`echo "# SkillCyprus Website" > README.md`

* Πρόσθεσε τα αρχεία στο Git:

`git add .`

`git commit -m "Αρχικό commit για τοπικό repository"`

* Δημιούργησε ένα νέο repository στο GitHub μέσω του browser, **χωρίς να επιλέξεις Initialize this repository with a README**.

  * Σύνδεσε το τοπικό repository με το GitHub:

`git remote add origin https://github.com/<username>/<repo-name>.git`

`git branch -M main`

`git push -u origin main`

* **Προσθήκη Στατικών Αρχείων**

  * Πρόσθεσε τα στατικά αρχεία σου (`index.html`, CSS, εικόνες, κλπ) στον φάκελο του project.

`git add .`

`git commit -m "Προσθήκη στατικών αρχείων"`

* Στείλε τις αλλαγές στο GitHub:

`git push`

* **Ενεργοποίηση GitHub Pages**

  * Πήγαινε στο repository σου στο GitHub.

  * Κάνε κλικ στο **Settings** \> **Pages** (στο αριστερό μενού).

  * Στην επιλογή **Source**, επίλεξε το **main** branch και στη συνέχεια τον φάκελο `/ (root)`.

  * Κάνε κλικ στο **Save**.

  * Το GitHub θα σου παρέχει έναν σύνδεσμο για την ιστοσελίδα σου (π.χ., `https://<username>.github.io/<repo-name>`).

* **Δες τη Σελίδα Σου**

  * Μετά από 1-2 λεπτά, η ιστοσελίδα σου θα είναι ζωντανή στον σύνδεσμο του GitHub Pages.

  * Επισκέψου τον σύνδεσμο για να δεις την ιστοσελίδα σου σε δράση\!

