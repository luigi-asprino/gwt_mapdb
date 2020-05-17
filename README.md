# GWT e MapDB
Un semplice esempio di uso di gwt e mapdb pensato per gli studenti del corso di [Ingegneria del Software](http://sweng.web.cs.unibo.it) del corso di Laurea di Informatica per il Management dell'Università di Bologna.

L'esempio e basato su questa [guida](https://mincong-h.github.io/2018/01/29/learning-gwt-with-maven/).

### Prerequisiti

Assicurarsi che maven e git siano correttamente installati sul proprio pc.
Assicurarsi che maven usi java8, eseguendo il comando ``mvn --version'' e controllando che  il risultato sia simile al seguente.

```
mvn --version
...
Java version: 1.8.0_144, vendor: Oracle Corporation
Java home: /Library/Java/JavaVirtualMachines/jdk1.8.0_144.jdk/Contents/Home/jre
...
```

[Impostare JAVA_HOME in windows](https://confluence.atlassian.com/conf59/setting-the-java_home-variable-in-windows-792499849.html)


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


### Testing

E' possibile testare il software usando maven eseguendo da terminale il seguente comando.

```
mvn clean verify
```



