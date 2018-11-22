Ho creato lo script "OWMUtility" per scaricare i dati meteo usando le api di openweathermap.

INSTALLAZIONE:

(1) Scaricare l'archivio https://github.com/giacfuria/OWMUtility/releases/download/0.1/OWMUtility.tar e decomprimerlo in una cartella qualsiasi.

(2) Inserire nel codice dello script la chiave fornita da openweathermap per l'accesso alle api.

Lo script deve essere chiamato da terminale nei due modi seguenti:

- $./OWMUtility corrente 
  
  se si vogliono scaricare le condizioni meteo
  attuali per le 50 città contenute nel file "lista_50_citta.txt".

- $./OWMUtility previsione
   
  se si vogliono scaricare le previsioni meteo
  Per i 5 giorni successivi a quello attuale per le 50 città contenute nel 
  file "lista_50_citta.txt".

NOTE:

(1) Lo script, in base al parametro scelto, crea una cartella (meteo_corrente o previsione) nella stessa cartella in cui è posizionato. Questa contiene un file xml (nome_citta.xml) per ogni città.

(2) Lo script "OWMUtility" e il file "lista_50_citta.txt" devono trovarsi nella stessa cartella. Entrambi possono essere posizionati in una cartella qualsiasi per funzionare. 

(3) Il file "lista_50_citta.txt" contiene le 50 città più popolose in Italia. Possono essere aggiunte altre città in un qualsiasi momento.
