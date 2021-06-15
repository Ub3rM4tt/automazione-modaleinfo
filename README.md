# automazione-modaleinfo
Tool per automatizzare la creazione della modaleInfo.jsp

Per automatizzare la creazione della modale info è possibile usare il tool presente nel file AutomazioneModaleInfo.html, presente nella stessa cartella di questa guida. Occorrerà semplicemente aprire il file html con Chrome.
Nella versione attuale si deve sempre partire da un testo contenente le informazioni relative al branch e alle issue, seguendo questa formattazione:

Branch_VerificheAdCEdilizia
•	#678 VERIFICHE ADC EDILIZIA – Aggiunta segnalazione Anomalia nella funzione di Validazione Edilizia 
•	#656 VERIFICHE ADC EDILIZIA – Implementati Download Dati, Scarica Report Excel e Scarica Report Pdf 
•	#674 VERIFICHE ADC EDILIZIA – Implementato Verbale Checklist Verifica ADC Edilizia 
•	#654 VERIFICHE ADC EDILIZIA – Implementati Parametri di Filtro 
•	#655 VERIFICHE ADC EDILIZIA – Implementato Esito Ricerca 

Aperto il tool, Il testo dovrà essere inserito nella textArea in alto.
Cliccando su “Converti”, nella textArea in basso comparirà il codice da inserire direttamente nella modaleinfo.jsp.

N.B. Il testo convertito riguarderà le table che andranno aggiunte subito sotto al tag legend Presente nella modale info.
<legend class="fsDetLabel">Dettaglio modifiche</legend>

REGOLE GENERALI:
•	Se sono presenti più branch, vanno separati tra loro dal carattere pipe “|”.
•	Se si fa riferimento a più issue su una stessa riga allora queste vanno separate da una virgola ed uno spazio, senza aggiungere il cancelletto alle issue successive alla prima:
o	Es:	 #554, 555 Esempio issue multiple – seguire questa formattazione.
•	Al momento vengono gestiti i caratteri speciali di lista (•), i trattini di Microsoft Word (–).
