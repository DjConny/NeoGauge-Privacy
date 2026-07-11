---
layout: default
title: Privacy Policy di NeoGauge
description: Informativa sul trattamento dei dati personali
---

# Privacy Policy di NeoGauge

Questa informativa descrive il trattamento effettuato dall'app NeoGauge. È pubblicata come pagina statica tramite GitHub Pages e non integra analytics, pubblicità, cookie aggiuntivi o moduli di contatto. GitHub può trattare dati tecnici di accesso secondo la propria informativa sulla privacy.

## 1. Chi tratta i dati

Il Titolare del trattamento dei dati personali trattati attraverso NeoGauge è:

**Fabio Francesco Conese**, persona fisica  
Indirizzo: **Via Carmine 54/B, 28047 Oleggio (NO), Italia**  
Email per privacy e questioni amministrative: **ffc80.lavoro@gmail.com**  
Email per assistenza tecnica e disservizi dell'app: **kawasaki.z650rs.italia@gmail.com**  
PEC: non disponibile  
Responsabile della protezione dei dati (DPO/RPD): non nominato

Nel resto di questa informativa viene indicato come “Titolare”.

## 2. A chi si applica questa informativa

Questa Privacy Policy riguarda l'app NeoGauge per iPhone e iPad e descrive quali dati vengono utilizzati, perché vengono utilizzati e quali scelte sono disponibili.

NeoGauge è un'app per gestire le informazioni relative alle proprie moto, registrare rifornimenti e chilometraggio, seguire i percorsi e consultare statistiche. L'app non utilizza un server proprietario del Titolare: i dati operativi vengono salvati sul dispositivo e, quando iCloud è disponibile, sincronizzati mediante il CloudKit privato associato all'account Apple dell'utente.

## 3. Dati trattati

### 3.1 Dati del profilo

NeoGauge può trattare:

- nome e cognome;
- indirizzo email;
- identificativo interno del profilo;
- identificativo univoco fornito da “Accedi con Apple”, se viene scelta questa modalità;
- informazioni di sessione e credenziali necessarie all'accesso locale.

Quando si usa “Accedi con Apple”, nome ed email possono essere comunicati da Apple soltanto in occasione del primo consenso. Se si sceglie “Nascondi la mia email”, NeoGauge riceve l'indirizzo relay messo a disposizione da Apple e non l'indirizzo email personale originario.

### 3.2 Dati delle moto e contenuti inseriti dall'utente

L'app può trattare i dati che l'utente decide di inserire, tra cui:

- soprannome, marca, modello, targa, data di immatricolazione e cilindrata della moto;
- foto della moto;
- stato della moto, ad esempio principale, attiva, archiviata o venduta;
- chilometraggio attuale e storico delle letture;
- rifornimenti, litri, costo totale, valuta, chilometraggio e indicazione di pieno;
- percorsi, nomi dei percorsi, date, distanze, orari, durata, velocità media e velocità massima;
- statistiche e riepiloghi annuali derivati dai dati inseriti o registrati nell'app;
- preferenze dell'interfaccia, filtri, schede statistiche preferite e impostazioni dei promemoria.

### 3.3 Posizione precisa

Con il permesso dell'utente, NeoGauge usa la posizione precisa mentre l'app è in uso. In particolare, il GPS viene utilizzato:

- quando viene aperta la dashboard di guida, per mostrare velocità, direzione, altitudine e dati del viaggio;
- durante un viaggio, per calcolare distanza e statistiche di percorrenza;
- quando viene registrato un rifornimento, per associare facoltativamente al rifornimento coordinate, precisione e momento di acquisizione;
- per richiedere a WeatherKit le condizioni meteo della posizione corrente;
- per mostrare su MapKit la posizione associata a un rifornimento o aprirla nell'app Mappe.

NeoGauge richiede l'accesso alla posizione soltanto “quando l'app è in uso”. Il codice dell'app non richiede il monitoraggio continuo della posizione in background. La posizione associata a un rifornimento può essere salvata insieme agli altri dati e sincronizzata tramite CloudKit. Le posizioni temporaneamente usate dalla dashboard e da WeatherKit non vengono trasformate dal codice in uno storico completo del tracciato GPS: vengono utilizzate per le funzioni visibili di guida, meteo e calcolo del viaggio.

Il permesso può essere modificato in qualsiasi momento nelle impostazioni di iOS o iPadOS. In assenza del permesso, le funzioni che dipendono dalla posizione possono essere limitate, mentre le altre funzioni dell'app restano disponibili.

### 3.4 Fotocamera e libreria foto

NeoGauge accede alla fotocamera o alla libreria foto soltanto quando l'utente sceglie di scattare o selezionare una foto della propria moto. L'immagine scelta viene ridimensionata e compressa dall'app, quindi salvata come parte dei dati della moto. Se la sincronizzazione iCloud è attiva, anche la foto può essere sincronizzata nel CloudKit privato dell'utente.

NeoGauge non analizza le immagini per pubblicità, riconoscimento facciale o profilazione.

### 3.5 Notifiche

Su iPhone, l'utente può attivare un promemoria locale per aggiornare il chilometraggio. NeoGauge conserva sul dispositivo lo stato del promemoria e la data dell'ultimo aggiornamento e programma una notifica locale dopo sette giorni.

Le notifiche locali non vengono usate per pubblicità. CloudKit può inoltre utilizzare notifiche remote silenziose gestite dal sistema per sincronizzare i dati tra i dispositivi dell'utente; non sono messaggi promozionali.

### 3.6 Acquisti in-app

L'eventuale acquisto per sbloccare ulteriori funzionalità o moto è gestito tramite StoreKit e App Store. Pagamento, metodo di pagamento, ricevute e gestione della transazione sono trattati da Apple secondo le proprie condizioni e informative.

NeoGauge verifica tramite StoreKit se l'acquisto è valido e se il diritto acquistato è attivo. Il codice dell'app non invia dati di pagamento a un server del Titolare e non conserva numeri di carta o credenziali di pagamento.

### 3.7 Backup

Nella sezione “Dati e backup” l'utente può avviare manualmente un backup. Quando tale schermata viene utilizzata, l'app può inoltre aggiornare automaticamente il backup se sono trascorse almeno 24 ore dall'ultimo.

Il backup esplicito attualmente creato da NeoGauge è un file JSON di riepilogo che contiene data di creazione, conteggi delle principali categorie di record, versione dell'app e numero di build. Il file viene salvato nell'area privata dell'app sul dispositivo e caricato come risorsa nel CloudKit privato dell'utente. Viene mantenuto un solo file denominato `latest-backup.json`: ogni nuovo backup sostituisce quello precedente.

Questo riepilogo di backup è distinto dalla normale sincronizzazione dei dati completi di NeoGauge, effettuata da SwiftData tramite CloudKit.

## 4. Dove vengono conservati i dati

### 4.1 Archivio locale SwiftData

NeoGauge usa SwiftData per mantenere sul dispositivo una copia operativa dei profili, delle moto, delle letture chilometriche, dei rifornimenti, dei percorsi e delle statistiche. Questo permette di utilizzare le funzioni principali anche quando la connessione non è disponibile.

Alcune preferenze non sensibili, come filtri, ordine delle schede e impostazioni dei promemoria, sono conservate in `UserDefaults` e `AppStorage` nell'area privata dell'app.

### 4.2 CloudKit privato

Nella configurazione ordinaria, l'archivio SwiftData è sincronizzato con il database CloudKit privato collegato all'account iCloud dell'utente. La sincronizzazione permette di ritrovare gli stessi dati sui dispositivi compatibili che utilizzano il medesimo account iCloud e NeoGauge.

Il database è privato dell'utente e utilizza l'infrastruttura iCloud di Apple. Disponibilità, conservazione tecnica e localizzazione dei dati nell'infrastruttura Apple dipendono dall'account, dalle impostazioni iCloud e dai termini applicabili ai servizi Apple.

### 4.3 Keychain e iCloud Keychain

NeoGauge usa il Keychain di Apple per proteggere piccole informazioni di autenticazione, tra cui email di accesso, credenziali locali e identificativo restituito da “Accedi con Apple”. Quando la voce è configurata come sincronizzabile e l'utente ha attivato iCloud Keychain, Apple può sincronizzarla in forma protetta tra i dispositivi dell'utente.

Il Keychain è separato dall'archivio SwiftData ed è protetto dai meccanismi di sicurezza del sistema operativo. NeoGauge può usare Face ID per sbloccare la sessione, ma il codice dell'app non riceve né conserva i dati biometrici: la verifica è effettuata dal sistema Apple.

## 5. Servizi Apple utilizzati

NeoGauge integra servizi e framework Apple necessari alle funzioni richieste dall'utente:

- **iCloud e CloudKit**, per sincronizzare dati e backup nel database privato dell'utente;
- **Keychain e iCloud Keychain**, per proteggere e, se abilitato, sincronizzare le credenziali;
- **Accedi con Apple**, per l'autenticazione facoltativa;
- **Core Location/GPS**, per posizione, velocità, direzione, altitudine e calcoli di viaggio;
- **MapKit e Mappe**, per mostrare o aprire le coordinate dei rifornimenti;
- **WeatherKit**, per ottenere temperatura e condizioni meteo relative alla posizione corrente;
- **Fotocamera e libreria foto di iOS**, per acquisire la foto scelta dall'utente;
- **UserNotifications**, per promemoria locali e supporto tecnico alla sincronizzazione CloudKit;
- **StoreKit e App Store**, per acquisti in-app e ripristino degli acquisti.

Apple tratta dati tecnici e richieste necessarie a fornire tali servizi secondo i propri termini e la propria informativa sulla privacy, disponibile all'indirizzo [https://www.apple.com/legal/privacy/](https://www.apple.com/legal/privacy/).

## 6. Finalità e basi giuridiche

I dati vengono trattati per le seguenti finalità:

| Finalità | Dati interessati | Base giuridica |
|---|---|---|
| Creare e gestire il profilo e la sessione | Nome, cognome, email, identificativi e credenziali | Esecuzione del servizio richiesto dall'utente, art. 6(1)(b) GDPR |
| Registrare e sincronizzare moto, foto, rifornimenti, chilometraggio, percorsi e statistiche | Dati e contenuti inseriti o generati usando l'app | Esecuzione del servizio richiesto dall'utente, art. 6(1)(b) GDPR |
| Fornire funzioni GPS, meteo e mappa | Posizione precisa e dati derivati | Consenso dell'utente, art. 6(1)(a) GDPR, espresso tramite il permesso del sistema e revocabile dalle impostazioni |
| Acquisire una foto della moto | Foto scelta o scattata dall'utente | Consenso dell'utente, art. 6(1)(a) GDPR, espresso mediante l'azione e il permesso del sistema |
| Inviare promemoria locali | Preferenza del promemoria, identificativo della moto e data dell'ultimo aggiornamento | Consenso dell'utente, art. 6(1)(a) GDPR, revocabile dalle impostazioni o nell'app |
| Proteggere sessione, credenziali e integrità dell'app | Informazioni di autenticazione e dati tecnici strettamente necessari | Esecuzione del servizio, art. 6(1)(b) GDPR, e legittimo interesse del Titolare alla sicurezza, art. 6(1)(f) GDPR |
| Gestire acquisti e ripristino dei diritti acquistati | Stato della transazione e diritto StoreKit | Esecuzione del contratto, art. 6(1)(b) GDPR; gli aspetti fiscali e di pagamento sono gestiti separatamente da Apple |
| Rispondere alle richieste privacy e adempiere agli obblighi normativi | Dati della richiesta e corrispondenza | Obbligo legale, art. 6(1)(c) GDPR |

Il rifiuto o la revoca dei permessi facoltativi impedisce soltanto le funzioni che richiedono tali permessi. La revoca non pregiudica la liceità del trattamento effettuato prima della revoca.

## 7. Destinatari dei dati

I dati non vengono venduti e non vengono comunicati a inserzionisti o società di profilazione.

Possono essere trattati o trasmessi a:

- **Apple**, attraverso iCloud, CloudKit, Keychain, Accedi con Apple, MapKit, WeatherKit, StoreKit, App Store e gli altri servizi di sistema descritti sopra;
- eventuali soggetti che assistano il Titolare per obblighi legali, sicurezza o supporto, soltanto se effettivamente nominati e nei limiti necessari;
- autorità pubbliche, quando la comunicazione sia richiesta dalla legge o da un provvedimento legittimo.

Dal codice attuale non risultano SDK pubblicitari, piattaforme di analytics, sistemi di profilazione, social tracker o server applicativi gestiti dal Titolare.

## 8. Trasferimenti internazionali

L'uso dei servizi Apple può comportare il trattamento di dati in Paesi diversi da quello dell'utente, compresi Paesi esterni allo Spazio economico europeo. Apple dichiara di utilizzare le garanzie previste dalla normativa applicabile per i trasferimenti internazionali; le condizioni concrete dipendono dal servizio Apple, dall'account e dagli accordi applicabili.

Per maggiori informazioni sulla localizzazione dei dati e sulle garanzie utilizzate da Apple, l'utente può consultare l'informativa e i termini applicabili ai servizi Apple indicati nella sezione 5.

## 9. Conservazione dei dati

I dati dell'app vengono conservati sul dispositivo e nel CloudKit privato dell'utente finché l'account e i relativi dati restano presenti oppure finché l'utente non li elimina.

In particolare:

- i dati operativi restano nell'archivio SwiftData e nella copia CloudKit sincronizzata;
- le credenziali restano nel Keychain finché l'utente non elimina l'account o finché non vengono rimosse dall'app o dalle impostazioni Apple;
- il riepilogo di backup sostituisce il file precedente, quindi ne viene mantenuta una sola versione;
- le notifiche locali restano programmate finché sono attive o finché l'account non viene eliminato;
- dopo una richiesta di cancellazione possono essere conservati soltanto eventuali dati strettamente necessari per adempiere a obblighi di legge o difendere un diritto, per il periodo richiesto dalla normativa applicabile. NeoGauge non mantiene nel proprio archivio una copia separata dei dati di pagamento gestiti da Apple.

La rimozione dell'app elimina normalmente il contenitore locale dell'app, ma non garantisce da sola la cancellazione dei dati presenti in iCloud Keychain o nel CloudKit privato. Per una cancellazione coordinata deve essere utilizzata la funzione “Elimina account” prima di disinstallare l'app, oppure deve essere contattato il Titolare.

## 10. Sicurezza

NeoGauge adotta misure coerenti con la natura dell'app, tra cui:

- contenitore privato dell'app protetto dal sistema operativo;
- archiviazione locale mediante SwiftData;
- database CloudKit privato associato all'account iCloud dell'utente;
- Keychain per credenziali e identificativi di autenticazione;
- possibilità di proteggere l'accesso mediante Face ID, senza accesso ai dati biometrici;
- connessioni e servizi gestiti dai framework Apple;
- riduzione e compressione locale delle immagini prima del salvataggio;
- assenza di un database applicativo pubblico o di un backend proprietario.

Nessun sistema può garantire sicurezza assoluta. L'utente deve proteggere il proprio dispositivo, il codice di sblocco e l'account Apple e mantenere aggiornati sistema operativo e app.

## 11. Pubblicità, profilazione e tracciamento

NeoGauge:

- non mostra pubblicità di terze parti;
- non vende dati personali;
- non crea profili pubblicitari;
- non utilizza i dati per seguire l'utente tra app o siti di soggetti diversi;
- non integra SDK di advertising o analytics di terze parti;
- non utilizza processi decisionali automatizzati che producano effetti giuridici o analogamente significativi.

Le statistiche mostrate da NeoGauge riguardano esclusivamente l'utilizzo e i dati delle moto dell'utente e servono a fornire le funzioni richieste nell'app.

## 12. Diritti dell'interessato

Nei casi previsti dal GDPR, l'utente può chiedere al Titolare:

- conferma dell'esistenza del trattamento e accesso ai dati;
- rettifica dei dati inesatti;
- cancellazione dei dati;
- limitazione del trattamento;
- portabilità dei dati forniti, quando applicabile;
- opposizione ai trattamenti basati sul legittimo interesse;
- revoca del consenso per i trattamenti facoltativi, senza pregiudicare il trattamento già effettuato;
- informazioni sulle garanzie relative ai trasferimenti internazionali;
- reclamo al Garante per la protezione dei dati personali o all'autorità di controllo competente.

Le richieste possono essere inviate a **ffc80.lavoro@gmail.com**. Il Titolare può chiedere le informazioni strettamente necessarie per verificare l'identità del richiedente e risponde nei termini previsti dalla normativa.

Per informazioni sui diritti e sui reclami è possibile consultare il sito del [Garante per la protezione dei dati personali](https://www.garanteprivacy.it/).

## 13. Eliminazione dell'account

NeoGauge include una funzione “Elimina account” con conferma esplicita. In base al funzionamento attuale dell'app, questa funzione tenta di eliminare:

- il backup esplicito presente nel CloudKit privato;
- i record SwiftData relativi a profilo, moto, chilometraggio, rifornimenti, percorsi e statistiche, con propagazione tramite CloudKit;
- il backup locale;
- preferenze e impostazioni dell'account conservate in `UserDefaults`;
- notifiche locali programmate;
- credenziali e identificativi conservati nel Keychain locale e sincronizzabile.

Se l'eliminazione del backup CloudKit o dell'archivio principale non riesce, l'app interrompe l'operazione e informa l'utente. Se restano elementi secondari, come file locali o credenziali, l'app segnala che la pulizia è stata soltanto parziale.

NeoGauge non conserva i token necessari per revocare automaticamente l'autorizzazione “Accedi con Apple”. Dopo aver eliminato l'account, l'utente può revocare separatamente l'accesso a NeoGauge dalle impostazioni del proprio account Apple.

Per esercitare i diritti GDPR è possibile contattare **ffc80.lavoro@gmail.com**. Per problemi tecnici relativi alla procedura è possibile contattare **kawasaki.z650rs.italia@gmail.com**.

## 14. Dati dei minori

NeoGauge non è progettata specificamente per bambini. L'età minima prevista per l'utilizzo autonomo dell'app è **14 anni**.

Se il trattamento di un minore si basa sul consenso e la normativa richiede l'autorizzazione di chi esercita la responsabilità genitoriale, l'app deve essere utilizzata soltanto con tale autorizzazione. In Italia, per l'offerta diretta di servizi della società dell'informazione, il limite previsto dall'art. 2-quinquies del Codice Privacy è 14 anni, salvo che si applichi una diversa base giuridica o una diversa normativa.

Chi ritiene che un minore abbia fornito dati senza l'autorizzazione necessaria può scrivere a **ffc80.lavoro@gmail.com** per richiederne la verifica e la cancellazione.

## 15. Modifiche a questa Privacy Policy

Questa informativa può essere aggiornata per riflettere modifiche dell'app, dei servizi Apple o della normativa. La versione aggiornata sarà pubblicata all'indirizzo [https://djconny.github.io/NeoGauge-Privacy/](https://djconny.github.io/NeoGauge-Privacy/), indicando la nuova data di entrata in vigore.

Quando le modifiche sono rilevanti, il Titolare informerà gli utenti con modalità adeguate, ad esempio tramite l'app, la pagina web o l'App Store, prima che le modifiche producano effetti quando richiesto dalla legge.

## 16. Data di entrata in vigore

**1 agosto 2026**

## 17. Contatti

Per domande su questa Privacy Policy, per assistenza sulla cancellazione dell'account o per esercitare i diritti in materia di protezione dei dati:

**Fabio Francesco Conese**, persona fisica  
**Via Carmine 54/B, 28047 Oleggio (NO), Italia**  
Email privacy e amministrativa: **ffc80.lavoro@gmail.com**  
Email per assistenza tecnica: **kawasaki.z650rs.italia@gmail.com**  
PEC: non disponibile
