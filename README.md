# README
Lo script `OWMUtility` permette di scaricare i dati meteo usando le api di openweathermap.

### INSTALLAZIONE:

1. Scaricare l'archivio [OWMUtility.tar](https://github.com/giacfuria/OWMUtility/releases/download/0.1/OWMUtility.tar) e decomprimerlo in una cartella qualsiasi.

2. Inserire nel codice dello script la chiave fornita da openweathermap per l'accesso alle api.

Lo script deve essere chiamato da terminale nei tre modi seguenti:

```
./OWMUtility corrente 
```
  se si vogliono scaricare le condizioni meteo
  attuali per le 50 città contenute nel file `lista_50_citta.txt`. 
```
./OWMUtility previsione
```   
  se si vogliono scaricare le previsioni meteo 
  per i 5 giorni successivi a quello attuale per le 50 città contenute nel 
  file `lista_50_citta.txt`.
```
./OWMUtility immagini
```
  se si vogliono scaricare le icone associate ai weather codes.
  
### NOTE:

1. Lo script, in base al parametro scelto, crea una cartella (`meteo_corrente`, `previsione` o `icone`) nella stessa cartella in cui è stato eseguito. Le cartelle `meteo_corrente` e `previsione` dopo l'esecuzione contengono un file xml (`nome_citta.xml`) per ogni città. La cartella `icone` dei file nella forma `10d.png`.

2. Lo script `OWMUtility` insieme ai file `lista_50_citta.txt` e `file_icone.txt` devono trovarsi nella stessa cartella. Tutti e tre insieme possono essere posizionati in una cartella qualsiasi per funzionare. 

3. Il file `lista_50_citta.txt` contiene le 50 città più popolose in Italia. Possono essere aggiunte altre città in un qualsiasi momento. Attenzione a non inserire duplicati (usare diff).
