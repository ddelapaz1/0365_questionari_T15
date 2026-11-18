# T1.5 Modulacions i desmodulacions

Qüestionari d'autoavaluació del **mòdul 0365 – Radiocomunicacions** (EE30), tema 1.5, convertit des del banc de preguntes de Moodle.

Web: https://ddelapaz1.github.io/0365_questionari_T15/

- 73 preguntes: AM, FM, receptor superheterodí, digitalització, constel·lacions I/Q i modulacions digitals, amb senyals i constel·lacions per identificar.
- Retroacció immediata amb l'explicació de cada resposta i, si n'hi ha, per què l'opció triada no és correcta.
- Nota final sobre 10 en acabar: +1 per encert, −0,25 per error (com al Moodle) i puntuació proporcional a les preguntes d'aparellar i d'ordenar.
- Preguntes, opcions i elements barrejats a cada intent.

## Regenerar les dades

Si es modifica el banc `moodle/T1.5_modulacio_desmodulacio.xml`:

```bash
python3 tools/moodle2quiz.py moodle/T1.5_modulacio_desmodulacio.xml data/t1-5-modulacio.js --id t1-5-modulacio --title "T1.5 Modulacions i desmodulacions"
sed -i '' 's#"\.\./img/#"img/#g' data/t1-5-modulacio.js
```

El conversor escriu les rutes de les imatges per a una pàgina en una subcarpeta (`../img/`). Aquí el qüestionari és a l'arrel, i per això el `sed` les canvia per `img/`.
