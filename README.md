# GWT e MapDB
Un semplice esempio di uso di gwt e mapdb pensato per gli studenti del corso di [Ingegneria del Software](http://sweng.web.cs.unibo.it) del corso di laurea di Informatica per il management dell'Università di Bologna.

L'esempio e basato su questa [guida](https://mincong-h.github.io/2018/01/29/learning-gwt-with-maven/)

### Prerequisiti

Assicurarsi che maven e git siano correttamente installati sul proprio pc.

### Uso

Comdandi da eseguire da terminale per installare ed eseguire il progetto.

```
$ git clone https://github.com/luigi-asprino/gwt_mapdb.git
$ cd gwt_mapdb/
$ mvn war:exploded
$ mvn gwt:run
```

A questo punto l'applicazione sarà disponibile all'indirizzo http://localhost:8888/MyModule.html 

La logica applicativa è molto semplice.
1. Si inserisce il proprio nome.
2. Il client invia al server il nome inserito.
3. Il server controlla nel DB se ha mai ricevuto questo nome.
4. Nel caso in cui abbia ricevuto questo nome risponde dicendo quante volte lo ha ricevuto.




