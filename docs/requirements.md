# Analiza și specificarea cerințelor — TaskFlow

## 1. Scopul aplicației și tipul utilizatorilor
TaskFlow ajută utilizatorii să își organizeze activitățile zilnice într-o listă de sarcini cu termene și priorități.

Utilizatori țintă:
- elevi și studenți care își planifică temele și proiectele;
- angajați și freelanceri care gestionează sarcini de lucru;
- orice persoană care vrea o listă de sarcini accesibilă de pe mai multe dispozitive.

## 2. Funcționalități de bază
- Înregistrare și autentificare (email și parolă, link magic prin email, resetare parolă).
- Adăugarea unei sarcini (titlu, descriere, termen, prioritate).
- Vizualizarea listei de sarcini (Astăzi, Următoarele, Toate, Finalizate).
- Căutarea sarcinilor după titlu și descriere.
- Prioritizarea sarcinilor (mică, medie, mare).
- Editarea și ștergerea sarcinilor.
- Marcarea sarcinilor ca finalizate și bară de progres.
- Vizualizare calendar (sarcini grupate pe date).
- Sincronizare între dispozitive prin cont.
- Setări de profil și deconectare.

## 3. Cerințe de interfață
- Layout: fereastră desktop cu bară de titlu, bară de meniu (File, Edit, View, Help), panou de navigare în stânga, zonă principală de conținut, panou de detalii în dreapta și bară de stare în partea de jos.
- Culori: maximum 3 culori dominante — primară #4F46E5, secundară #0F172A, de accent #F59E0B, plus nuanțe neutre.
- Tipografie: două fonturi — Poppins pentru titluri, Inter pentru textul de bază; contrast al textului de minimum 4.5:1.
- Forme: colțuri rotunjite consecvente (12 px pentru carduri și butoane, 8 px pentru câmpuri), grilă de spațiere de 8 px.
- Navigare: panou lateral cu secțiunile Today, Upcoming, All, Completed, Settings; butonul „+ New task” este mereu accesibil; ferestre modale pentru creare și editare.
- Elemente UI: de intrare (câmpuri text, selector de dată, listă derulantă, bifă, comutator), de ieșire (carduri de sarcini, etichete de prioritate, bară de progres, notificări) și auxiliare (meniu, navigare, file, containere modale, bară de stare).

## 4. Cerințe non-funcționale
- Viteza de reacție: acțiunile frecvente (bifare, adăugare) se reflectă în interfață imediat.
- Ușurință în utilizare: maximum 3 clicuri pentru crearea unei sarcini; mesaje de eroare clare.
- Securitate: fiecare utilizator vede doar propriile sarcini (Row Level Security în Supabase).
- Adaptabilitate: interfață utilizabilă pe desktop, tabletă și telefon.
- Citibilitate: contrast suficient, text lizibil, suport pentru diacritice românești.
