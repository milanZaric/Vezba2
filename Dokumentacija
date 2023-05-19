# Vezba2 

# Opis baze u kratkim crtama. Baza je komplet izradjena na MacOS operativnom sistemu (Ventura verzija) u terminalu i pri izradi
  je koriscen alat home brew. Sve ostalo je standarno i bez ikakvog GUI-a. Baza sadrzi 2 tabele koju su vezane preko primarnih
  kljuceva koji su u bazi. Primarni kljuc u tabeli Prodavac je ID a u tabeli Prodaja je Prodavac ID.

# Svrha baze je iscitavanje podataka iz obe baze, pa je zato bilo potrebno za spajanjem tabela, i zato mozemo reci da je baza 
  relaciona.

# Opis tabela. Prva tabela je Prodavac i sastoji se od atributa kao sto su ID, Ime, Prezime, Automobil i boja, dok se u tabeli 
  Prodaja nalaze ID, Datum, Cena, Kolicina i Prodavac ID. 
  
# Pristup i instalacija. Pristupa se preko terminala a bazu je moguce ucitati i iz nekih popularnih GUI resenja(programa). Ova baza je 
  radjena totalno iz terminala. Tako da cu opisati kako u par koraka da se istoj pristupi na isti nacin. Prvo je potrebno 
  skinuti bazu sa ovog repozitoriju na Vas racunar. Sledeci korak je da se otvori terminal ili CMD ako je na primer windows 
  masina upitanju. Sa daljim objasnjenjem cu nastaviti sa primerom MacOS-a ali je postupak jako slican i na drugim operativnim
  sistemima. Na MacOS mozemo pokrenuti Spotlight precicu preko command + space dugmeta ili u gornjem desnom uglu na lupicu. U baru
  koji iskoci mozemo ukucati terminal i potvrditi. Kada smo usli u terminal mozemo instalirati home brew ukoliko nije instaliran.
  Komanda koju prvo treba da kucate u terminal je /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  potom za proveru da li je sve instalirano mozete ukucati brew doctor. Kada je home brew instaliran mozemo nastaviti sa ucitavanjem baze.
  Posle toga treba instalirati mysql sto je krajnje jednostavno pomocu home brew alata. Komanda je: brew install mysql, nakon cega je
  potrebno pokrenuti mysql server, komanda je: brew services start mysql, mozemo i ovo proveriti da li je sve proslo kako treba sa 
  komandom brew services list, i na kraju mozemo startovati mysql sa komadom: mysql -u root (default-no je da sifre nema, sto znaci samo
  stisnite enter za potvrdu). Posto su koraci svi uradjeni kako treba samo preostaje da se pozicioniramo gde je ova baza skinuta. Recicemo
  da je dafault lokacija downloads, tako da je komanda cd ~/Downloads, sada kada smo u Downloadsu mozemo da primenimo zavrsnu komandu a to
  je mysql -u root < ~/Downloads/BiznisBaza.sql.


# Neke osnovne komande kada smo vec u bazi i neki laksi upiti za izvlacenje nekih podataka.

======= Izlistavanje cele tabele Prodavac
        SELECT * FROM Prodavac;
======= Izlistavanje cele tabele Prodaja
        SELECT * FROM Prodaja;
======= Izlistavanje imena iz tabele Prodavac
        SELECT Ime FROM Prodavac;
======= Izlistavanje kolicine iz tabele Prodaja
        SELECT Kolicina FROM Prodaja;

Slozeniji upit, koja osoba ima koju kolicinu automobila naprimer i koje boje
        SELECT Ime, Prezime, Datum, Cena, Kolicina, Boja, Automobil
        FROM Prodaja 
        INNER JOIN Prodavac ON Prodaja.ProdavacID = Prodavac.ID
        WHERE Ime = 'Milan' and Prezime = 'Zaric';
        
        
### Sa ovim dokumentacija je finisirana, za sva dodatna pitanja stojim na raspolaganju.
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        

