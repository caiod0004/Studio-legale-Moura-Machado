# Pagina "Empresas na Europa": consegna

## Modifiche
- Ricostruita solo la vista `<div data-view="empresas">` di `index.html`. Router, header, questionario (`openQuiz`), modale `#ins` e le altre pagine non sono stati toccati.
- CSS nuovo nel blocco `/* ===== Página Empresas ===== */`, con tutte le classi prefissate `.emp-`. Riusa i token di `:root`.
- JS nuovo nel blocco `// ---------- Página Empresas ----------`, prima di `route()`: contiene il finder "Qual é o seu caminho?" e i punti della timeline.
- Sezioni della pagina:
  1. apertura con mappa SVG animata;
  2. finder con 3 scelte (risultato annunciato con `aria-live`);
  3. 4 strade per l'Italia, con il box "Descendente de italianos?";
  4. visto D2 e confronto Itália | Portugal;
  5. processo in 5 tappe, sticky da 980px in su;
  6. blocco Caterinho con `sala-madeira.jpg`;
  7. ruoli (assessoria jurídica / apoio operacional);
  8. Nota do escritório (invariata);
  9. FAQ con 7 domande e JSON-LD `FAQPage`;
  10. chiusura con CTA.
- Animazioni disattivate con `prefers-reduced-motion`.
- Nessuna immagine nuova.
- Verifiche fatte:
  - console senza errori;
  - questionario aperto da tutte le pagine;
  - modale `#ins` → questionario `empresa`;
  - screenshot a 1440 e 390.
- Per scelta di Caio, nel corpo della pagina non compaiono fonti. Restano solo nella Nota do escritório, come nelle altre pagine.

## Frasi e fonti
| Frase in pagina | Fonte |
|---|---|
| 650 vagas para trabalho autônomo em 2027, todos os países fora da UE | DPCM Flussi 2026-2028, GU 15/10/2025: https://www.gazzettaufficiale.it/ |
| Parâmetros financeiros da Câmara de Comércio (trabalho autônomo) | DPCM Flussi / Ministero dell'Interno, portale ALI |
| Italia Startup Visa: ≥ €50.000 e aprovação do Comitê do MIMIT | MIMIT: https://www.mimit.gov.it/ (Italia Startup Visa) |
| Visto para investidores: €250k / €500k / €1 mi / €2 mi (art. 26-bis TU, L. 232/2016) | Embaixada da Itália, checklist: https://ambwellington.esteri.it/wp-content/uploads/2026/07/5.-investors-visa-checklist_AMBWELL_ITA.pdf |
| Vale também via sociedade da qual é representante legal (DL 76/2020) | Il Sole 24 Ore NT+ Fisco: https://ntplusfisco.ilsole24ore.com/art/visto-investitori-esteri-piu-ampio-chance-anche-i-legali-rappresentanti-ADQ0dxn |
| Descendentes brasileiros: visto subordinado fora das cotas (DM 17/11/2025) | GU n. 273 del 24/11/2025: https://www.gazzettaufficiale.it/eli/id/2025/11/24/25A06275/SG · Ministero del Lavoro: https://lavoro.gov.it/node/30662 |
| Visto D2: plano de negócios, meios financeiros, formalização; residência emitida pela AIMA | AIMA: https://aima.gov.pt/ (da riverificare, vedi todo) |
| Permesso di soggiorno rilasciato dalla Questura | Polizia di Stato: https://www.poliziadistato.it/ (permesso di soggiorno) |
| Cittadino UE apre l'impresa senza visto | Libertà di stabilimento, art. 49 TFUE: https://eur-lex.europa.eu/ |

## Todo rimasti (visibili in pagina come `.todo`)
1. Ruolo esatto dell'avvocato in visura: oggi c'è `[verificare in visura: consigliere senza deleghe]`. Deve restare "sócio", mai "administrador" (art. 18 L. 247/2012).
2. Servizio operativo di Caio: nome, foto, descrizione e contratto separato.
3. Calendario Decreto Flussi 2027 da riverificare sul portale ALI. Attenzione: la home (articolo "Decreto Flussi 2027") pubblica già "Pré-cadastro até 7 de dezembro de 2026" come fatto.
4. Marchio ufficiale dello studio (oggi c'è la bilancia SVG ridisegnata).
5. Visto D2: prima di pubblicare, verificare i requisiti su AIMA o sul Diário da República.
6. Golden visa portoghese: non trattato per mancanza di una fonte verificata. La FAQ parla solo del visto per investitori italiano.
7. SEO: `#empresas` non è un URL indicizzabile a sé. Valutare una pagina `/empresas/` dedicata.
