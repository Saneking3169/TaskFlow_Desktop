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
- Filtre pe listă: Today, Upcoming, All, Completed.
- Sincronizare între dispozitive prin cont.
- Setări de profil și deconectare.

## 3. Cerințe de interfață
- Layout: fereastră desktop cu panou de navigare în stânga (logo, All tasks, Today, Completed, profil utilizator), antet cu titlul „My Tasks”, bară de căutare și butonul „+ Add task”, lista de sarcini în zona principală; adăugarea și ștergerea apar ca ferestre modale.
- Culori: maximum 3 culori dominante — primară albastru #2563EB, griuri neutre și roșu #EF4444 (doar pentru Delete și prioritatea High); verde, portocaliu și roșu din insigne sunt culori de stare.
- Tipografie: un singur font, Inter, cu greutăți diferite pentru ierarhie; contrast al textului de minimum 4.5:1.
- Forme: colțuri rotunjite consecvente (12 px pentru carduri, 8 px pentru câmpuri și butoane, 16 px pentru ferestre modale).
- Navigare: panou lateral cu secțiunile All tasks, Today, Completed (aplicația web are în plus Upcoming și Settings); butonul „+ Add task” este mereu accesibil; ferestre modale pentru adăugare și ștergere.
- Elemente UI: de intrare (câmpuri text, selector de dată, selector de prioritate, bifă), de ieșire (carduri de sarcini, etichete de prioritate, insigne „Done”, mesaje de confirmare) și auxiliare (panou lateral de navigare, containere modale).

## 4. Cerințe non-funcționale
- Viteza de reacție: acțiunile frecvente (bifare, adăugare) se reflectă în interfață imediat.
- Ușurință în utilizare: maximum 3 clicuri pentru crearea unei sarcini; mesaje de eroare clare.
- Securitate: fiecare utilizator vede doar propriile sarcini (Row Level Security în Supabase).
- Adaptabilitate: interfață utilizabilă pe desktop, tabletă și telefon.
- Citibilitate: contrast suficient, text lizibil, suport pentru diacritice românești.
