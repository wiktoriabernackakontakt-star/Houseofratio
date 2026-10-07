# Strona www House of Ratio

Jeden statyczny plik `index.html` (fonty Poppins i TAN Nimbus wklejone jako base64, więc strona nie
ładuje ich z Google Fonts; podpis „Wiktoria” w kroju Ms Madi na razie nadal ładuje się z Google
Fonts, do zmiany przy wdrożeniu, patrz sprawa S-185 w rejestrze).

Źródło do dalszej edycji (nieskompilowane, bez wklejonych fontów) zostaje w repo `SystemOS`,
w folderze `Nala — Copywriting/Probki/`, plik `index.src.html` z historii sesji Nali. Tu, w tym
osobnym repozytorium, leży tylko wersja gotowa do wdrożenia, bo to repozytorium jest publiczne
(albo widoczne dla Netlify i GitHuba), a `SystemOS` jest prywatne i nie wychodzi poza ten komputer.

Formularz kontaktowy wysyła się przez Netlify Forms (zgłoszenia trafiają na wiktoria@houseofratio.pl,
widać je też w panelu Netlify → Forms, zakładka tego site'u). Polityka prywatności w wersji 10
(07.10.2026) jest wklejona w stronę jako warstwa, otwierana ze stopki, i stoi też jako osobna strona
`polityka-prywatnosci.html`: ten adres mają formularze w reklamach Meta. Osobną stronę buduje z warstwy
skrypt w `SystemOS`, `Nala — Copywriting/Probki/2026-10-01-hor-strona-www-polityka-strona.py`; przy każdej
zmianie polityki uruchomić go ponownie, żeby obie wersje miały ten sam tekst.

Domena: houseofratio.pl, zarejestrowana na Hostido. Hostido zostaje tylko rejestratorem domeny,
Netlify hostuje stronę. Jak je połączyć: dopisać w panelu Hostido rekordy DNS, które pokaże Netlify
po dodaniu domeny w swoim panelu (Domain settings → Add a domain), nie zmieniać serwerów nazw (NS),
żeby nie zepsuć poczty na tej domenie.
