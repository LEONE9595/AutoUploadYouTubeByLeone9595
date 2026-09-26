=====================================================================
          🚀 AutoUpload YouTube v1.0.1.Beta - LEONE9595 🚀
=====================================================================
Sito Web        : https://leone9595.altervista.org/
Canale YouTube  : https://www.youtube.com/user/LEONE9595
Credits         : Fat da Leonardo P co 'l cor ❤️
=====================================================================

Benvenuto! Questo pacchetto ti permette di caricare e programmare 
automaticamente i tuoi video su YouTube senza bisogno di installare 
Python o altre componenti sul tuo computer.

---------------------------------------------------------------------
📁 STRUTTURA DELLE CARTELLE
---------------------------------------------------------------------

 - avvio.bat           : Clicca qui per avviare il programma.
 - setup_runtime.bat   : Da usare SOLTANTO se devi reinstallare o 
                         ripristinare l'ambiente Python portatile.
 - video/              : Inserisci qui i file video da caricare (.mp4, .mkv, .mov, .avi).
 - video/caricati/     : Qui verranno spostati automaticamente i video completati.
 - system/             : Contiene i file di configurazione, credenziali e lingue.
 - system/languages/   : File di lingua JSON (Italiano, English, Trentino, ecc.).
 - runtime/            : Contiene Python portatile e lo script di esecuzione.


---------------------------------------------------------------------
📌 GUIDA RAPIDA AL PRIMO UTILIZZO
---------------------------------------------------------------------

1. PREPARAZIONE DELLE CREDENZIALI GOOGLE (Se non incluse):
   - Assicurati che nella cartella "system/" sia presente il file 
     "client_secret.json" scaricato dalla tua Google Cloud Console.

2. NOMI DEI FILE VIDEO:
   - Nomina i tuoi file video seguendo questo formato per impostare 
     la modalità e le kill:
     
     Formato : MODALITA_KILL.mp4
     Esempi  : Conquest_52-10.mp4
               TDM_30-5.mp4
               Obliteration_15-2.mp4

     * Se il nome del file non contiene "_", la modalità predefinita 
       sarà "Conquest" e le kill "0-0".

3. INSERIMENTO VIDEO:
   - Copia i tuoi file video dentro la cartella "video/".

4. AVVIO DEL CARICAMENTO:
   - Fai doppio clic sul file "avvio.bat".
   - Seleziona la lingua desiderata dal menu iniziale.
   - Se è il primo avvio, si aprirà una pagina del browser per 
     autorizzare l'accesso al tuo canale YouTube.
   - Mettiti comodo e guarda la magia! ✨


---------------------------------------------------------------------
📝 LOG E REPORT
---------------------------------------------------------------------

Ad ogni caricamento completato:
 - Viene generato/aggiornato il report "file caricati report.txt" nella 
   cartella principale con tutti i link YouTube e le date di pubblicazione.
 - I contatori di ogni modalità vengono aggiornati automaticamente in 
   "system/contatori.json".
 - Il video caricato viene spostato in "video/caricati/".


---------------------------------------------------------------------
⚙️ PERSONALIZZAZIONE TESTI
---------------------------------------------------------------------

Puoi personalizzare i modelli dei titoli e delle descrizioni modificando 
i file:
 - system/titolo_base.txt
 - system/descrizione_base.txt

Parametri disponibili da usare tra parentesi graffe:
 - {modalita} : La modalità di gioco estratta dal nome file.
 - {numero}   : Il numero progressivo automatico.
 - {kill}     : Il punteggio/kill estratto dal nome file.


---------------------------------------------------------------------
❓ RISOLUZIONE PROBLEMI
---------------------------------------------------------------------

- "Impossibile trovare Python portatile":
  Verifica che la cartella "runtime/python/" sia presente. Se hai appena 
  estratto il file .ZIP, assicurati di aver estratto TUTTO il contenuto 
  e non solo il file .bat.

- "Errore di autenticazione":
  Elimina il file "system/token.json" e riavvia "avvio.bat" per fare 
  nuovamente il login sul tuo account YouTube.

=====================================================================
                    LEONE9595 OUT! 🚀
=====================================================================
