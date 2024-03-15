# Progetto01: Sviluppo di una applicazione Net

Questo progetto consiste nello sviluppo di una applicazione in grado di interagire con un servizio REST online, salvare dati in un database e gestire l'accesso ai dati da parte di utenti autenticati.

_Nota 1: è possibile utilizzare una qualsiasi versione recente di Net Core. In generale pe run nuovo progetto è consigliabile scegliere la versione “Long time support” corrente. [Vedi Download .NET (Linux, macOS, and Windows) (microsoft.com)](https://dotnet.microsoft.com/en-us/download))_

_Nota 2: Nel testo che segue ipotizzo che tu abbia scelto di utilizzare le API di AccuWeather per questo eservizio, ma puoi scegliere una API qualsiasi come ad esempio es. quelle di Google Maps, o di Open Street Map … esistono migliaia di servizi online che possono essere utilizzati in modo gratuito. Ti puoi divertire a cercare quello che ti piace ed adattare il progetto in base al servizio che scegli_.

## Istruzioni operative

1.	Create un account su [https://developer.accuweather.com/(]AccuWeather APIs) e ottenere una chiave per l’utilizzo **gratuito** del servizio
2.	Create un repository su GitHub (o GitLab) per ospitare il vostro progetto. Puoi eseguire in fork di questo repository se preferisci.
3.	Creare un’applicazione Net Core (web, desktop o console a vostra scelta) con le funzionaltà descritte nella sezione *requisiti*. **Non è necessario realizzare una applicazione completa. Anche un prototipo parziale può andare bene. La cosa importante è che il progetto possa mostrare le tua capacità come sviluppatore**.
4.	Invia al tuo contatto in Smartpeg un link al repository con il tuo progetto
5.	[Opzionale] pubblica la tua applicazione su un servizio di hosting a tua scelta ed inviaci anche il link ad un versione funzioanate dell'applicazione

## Requisiti 

L’applicazione dovrà avere se seguenti funzionalità: 

**Mostrare i dati meteo di una località scelta dall'utente**: l'applicazione deve leggere i dati forniti da AccuWeather per la località inserita dall'utente e mostrare in forma grafica o testuale la situaizone meteo attuale.

**Persistenza dei dati**: salvare in un database le seguenti informazioni ogni volta che vengono lette dalle API:
- Nome località
- Data e ora
- Temperatura corrente


**Gestione degli utenti e controllo di accesso**
- L’utente “admin” accede con una password predefinita letta dal file di configurazione
- Solo ‘admin” accede ad un pannello per la gestione degli utenti (creazione, cancellazione, cambio password)
- Solo gli utenti registrati possono vedere i dati meteo

### Requisiti aggiuntivi
Se ti piacciono le sfide impegnative, potresti aggiungere anche altre funzionalità come ad esempio:
- esporre una API per leggere i dati meteo salvati nel database
- visualizzare e salvare anche le previsioni del giorno successivo oltre che i dati meteo correnti
- dotare la tua applicaizone di un sistema di log utile per la diagnostica di eventuali problemi 
- produrre statistiche sull'utilizzo dell'applicazione da parte degli utententi
