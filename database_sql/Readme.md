# Creazione di un database

come prima cosa ho creato un file chiamato  <b>prova.db</b> (che sarebbe il nostro database).


## creazione della tabella 

poi come secondo passaggio ho creato il file <b>crea_tabella.sql</b> ho detto di creare la tabella  dentro al database <b>prova</b> con il comando <b>CREATE TABLE</b>.


Per creare le colonne del databse le ho messe dentro le parentesi e sono:
 


  <b>id</b> (con la chiave primaria ). <b>Nome</b> <b>Cognome</b> <b>Email</b>.








```sql
CREATE TABLE prova (
    ID INTEGER PRIMARY KEY,
    Nome TIPO,
    Cognome TIPO,
    Email TIPO
);

```

per eseguire il codice nel terminale ho scritto:

 <b>sqlite3 prova.db < crea_tabella.sql</b>


## inserimento dei dati

per inserire i dati nel mio databse ho utilizzato il comando <b> INSERT INTO</b> poi ho messo il nome del mio databse <b>prova</b> poi ho messo il nome delle colonne <b>Nome Cognome Email</b> e  tramite <b>VALUES</b> gli ho assegato i valori all' interno  a delle parentesi.
```sql
INSERT INTO  prova (Nome, Cognome, Email) VALUES 
('Andrea', 'Alvigini', 'AndreaAlvigini@example.com'),
('Davide', 'Rivolta', 'DavideRivolta@example.com'),
('Alessandro', 'Degiacobbi', 'AlessandroDegia@example.com'),
('Simone', 'Rizzo', 'SimoneRizzo@example.com'),
('Giorgio', 'Bruzzone', 'GiorgioBruzzone@example.com'),
('Christoper', 'Thompson', 'Christopherthompson@example.com'),
('Greta', 'DiFabio', 'GretaDifabio@example.com'),
('Tiziano', 'Gessa', 'TizianoGessa@example.com'),
('Emanuele', 'Cappanera', 'EmanueleCappanera@example.com'),
('Gianluca', 'Ciceri', 'GianlucaCiceri@example.com');

```

per eseguire questo snippet  ho scritto nel terminale:


<b>sqlite3 prova.db < inserisci_dati.sql </b>.