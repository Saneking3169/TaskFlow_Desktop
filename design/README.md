# Design — TaskFlow

Prototip interactiv (Figma Design, 5 ecrane desktop, 1440 px):
https://www.figma.com/proto/fPY5BbocvjIHYqdWqpkVKg/TaskFlow-Desktop-Prototype?node-id=1-2&starting-point-node-id=1%3A2&t=Q90uNsAKf56keAvC-1

## Ecrane
1. **01 Lista de sarcini** — bară laterală, căutare, buton „+ Add task”, 6 sarcini cu termen și prioritate.
2. **02 Add task** — fereastră modală: titlu, descriere, dată, prioritate (Low / Medium / High), Save / Cancel.
3. **03 Căutare și filtrare** — căutare „design” și filtru High, 3 rezultate.
4. **04 Ștergere sarcină** — dialog „Delete this task?” cu Delete / Cancel.
5. **05 Sarcini finalizate** — sarcini bifate, titluri tăiate, insigne „Done”.

## Navigare (On click, Navigate to)
- 01 „+ Add task” → 02; 02 „Save” / „Cancel” → 01
- 01 bara de căutare → 03; 01 iconița de coș → 04
- 04 „Cancel” / „Delete” → 01
- Bara laterală: „Completed” → 05, „All tasks” → 01
- Punct de start: 01 Lista de sarcini

## Sistem de design
Font: Inter. Culori: albastru primar #2563EB, griuri neutre, roșu #EF4444 doar pentru Delete și High; culori de stare în insigne (verde, portocaliu, roșu).
Colțuri rotunjite: carduri 12 px, câmpuri și butoane 8 px, ferestre modale 16 px. Auto Layout, straturi denumite.

## Capturi
Capturile ecranelor se adaugă în acest folder (01-lista.png, 02-add-task.png, 03-cautare.png, 04-stergere.png, 05-finalizate.png).
