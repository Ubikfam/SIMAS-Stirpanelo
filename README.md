# SIMAS Stirpanelo

Pulpit właściciela projektu BliSperanto: stan STOP, postęp, otwarte PR i karty decyzji. Działa w każdej
przeglądarce, bez claude.ai i bez ChatGPT.

**Adres:** https://ubikfam.github.io/SIMAS-Stirpanelo/

## Jak działa

- Repozytorium zawiera tylko kod strony. Ilustracje Bliss do kart decyzji są w repozytorium prywatnym; tutaj ich nie ma (strona je pomija). **Nie ma tu żadnych danych projektu ani tokenów.**
- Dane strona czyta dopiero po połączeniu: przy pierwszym otwarciu prosi o własny token GitHub właściciela
  (fine-grained, tylko repozytorium `Ubikfam/BliSperanto`, uprawnienia *Issues: Read and write* i
  *Pull requests: Read-only*, z datą wygaśnięcia).
- Token zostaje wyłącznie w przeglądarce tego urządzenia i jest wysyłany tylko do `api.github.com`.
  Przycisk „Zapomnij token” usuwa go z urządzenia.
- Strona czyta #1, #47, #50 i listę otwartych PR; jedyny zapis to komentarz decyzji „Bogusław zatwierdza: Dnn=n” w #50.
- Otwarta jako artefakt w claude.ai korzysta z konektora GitHub zamiast tokenu.

## Źródło

Plik `index.html` to kopia `cockpit/simas_cockpit_v0.html` z prywatnego repozytorium `Ubikfam/BliSperanto`
(tam są testy i historia zmian). Zmiany robi się najpierw tam, potem kopiuje tutaj.
