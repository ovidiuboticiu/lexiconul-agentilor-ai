# Metodologie, verificări și limite

## Scop și domeniu

Lexiconul este o resursă **educațională bilingvă EN–RO** pentru noțiuni despre AI, LLM, agenți, automatizare, RAG, securitate, evaluare și instrumente conexe. Ediția curentă **v0.9.6a** conține **361 de intrări**. Unele concepte se suprapun intenționat; o intrare nu echivalează obligatoriu cu un concept complet independent.

Fiecare intrare include denumirea engleză, echivalentul sau categoria în română, o definiție și o explicație „De ce contează?”. Sunt incluse, unde este cazul, legături interne și surse.

## Proces editorial

Materialul a fost construit iterativ **cu asistență AI substanțială**, cu selecția, integrarea, corectarea și deciziile editoriale supravegheate de autor. Au existat mai multe runde de audit critic realizate cu sisteme AI distincte, în special Claude și Codex. Aceste audituri nu trebuie prezentate drept certificări umane independente.

Metoda a inclus:
1. Îmbunătățirea definițiilor și a exemplelor practice, cu delimitarea termenilor apropiați.
2. Verificări selective ale documentației primare și ale surselor bibliografice.
3. Compararea automată a edițiilor pentru a evita pierderea accidentală a intrărilor.
4. Teste ale funcțiilor de căutare, navigare, afișare, tipărire și adaptare la ecrane diferite.
5. Închiderea constatărilor documentate înainte de publicarea acestei copii.

## Rezultatele și acoperirea verificărilor

- În tranziția **v0.9.4a → v0.9.5** au fost adăugate 14 intrări, de la 347 la 361; audituri ulterioare au analizat toate cele 14 intrări noi și relațiile lor cu termeni existenți.
- În **v0.9.5 → v0.9.6**, opt intrări au primit corecții punctuale, fără modificări ale CSS sau JavaScript. Au fost verificate păstrarea celor 361 de intrări și integritatea legăturilor interne.
- Auditul Claude pentru v0.9.6 a raportat **GO**, cu teste în Chromium pe Linux prin `file://` la 1440, 390 și 320 px.
- Auditul Codex pentru v0.9.6 a raportat **GO WITH MINOR CORRECTIONS**, indicând o sursă lipsă pentru afirmația GraphRAG și un efect minor al potrivirii de căutare.
- Ediția **v0.9.6a** adaugă exclusiv referința [Microsoft GraphRAG](https://microsoft.github.io/graphrag/) la intrarea **Knowledge graph**, pe lângă actualizarea etichetei de versiune. Definițiile, explicațiile, CSS și JavaScript nu au fost schimbate.
- Testele de integrare asupra v0.9.6a, prin încărcarea HTML-ului în Chromium, au confirmat 361 de intrări, căutările relevante și afișarea la cele trei lățimi. Deschiderea automată prin `file://` nu a putut fi efectuată în mediul acestor teste.
- Autorul a verificat local pe Windows că fișierul **pare funcțional**, dar nu a raportat o matrice completă de teste.

**Aceste rezultate nu certifică factual toate afirmațiile din cele 361 de intrări.** Auditurile de regresie se concentrează pe zonele schimbate; numeroase definiții au fost verificate doar structural sau editorial. Testele locale nu înlocuiesc evaluarea de accesibilitate cu cititor de ecran, testarea completă pe Android sau verificarea tipăririi pe hârtie.

## Surse și niveluri de certitudine

Trimiterile din fișele unor concepte indică surse tehnice, lucrări, standarde sau documentație de produs. Acestea pot susține doar o parte din afirmațiile unei fișe și nu echivalează cu verificarea tuturor exemplelor. În cazul produselor și al framework-urilor, documentația se poate modifica în timp.

Materialul conține și expresii operaționale sau descriptive pentru care nu există un standard terminologic unic. Etichetele din lexicon ajută la identificarea lor.

## Limite funcționale cunoscute

- Potrivirea după aliasuri poate aduce rezultate nespecifice pentru cuvinte comune: de exemplu, interogarea „cu” poate găsi intrarea PII prin aliasul „date cu caracter personal”.
- Unele denumiri diferă între implementări, platforme și ediții de documentație.
- Lexiconul funcționează ca fișier HTML autonom, fără dependențe de rețea pentru afișare sau căutare; legăturile către surse externe necesită internet.
- Textul este informativ și nu constituie consultanță juridică, medicală sau de securitate.

## Integritate și proveniență

Fișierul HTML folosit pentru pagina publică este copia nealterată a versiunii **v0.9.6a**, cu identificatorul SHA-256:

`e03faf59bba6b74ac082640f8ee8f57d23b3925198f190b06a4f0ad60fba496b`

Pagina principală din repository este acest fișier redenumit **index.html**. Renumirea nu modifică conținutul.

## Îmbunătățiri ulterioare

Observațiile documentate pot fi transmise prin [Issues](https://github.com/ovidiuboticiu/lexiconul-agentilor-ai/issues). O corecție trebuie să delimiteze problema de fond, să indice o sursă când este relevant și să poată fi verificată după aplicare.

## Licențiere

Nu este atribuită încă o licență de reutilizare. Documentul public este disponibil pentru consultare, fără a implica acordarea unor drepturi suplimentare asupra materialului.
