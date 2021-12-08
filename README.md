# :pushpin: Prikaz izveštaja kao odgovor na zahteve koji su postavljeni od strane korisnika

U ovom delu biće prikazani grafički izveštaji koji su kreirani na osnovu zahteva korisnika. Za potrebe ovog procesa korišćeno je prethodno kreirano skladište podataka i alat za pravljenje izveštaja koji predstavlja dodatak za *Visual Studio* pod nazivom SSRS (*SQL Server Reporting Services*).

### Zahtev broj :one:: Koji je dozvoljen broj dana na koji se film određene oznake može iznajmiti?

Zahtev je prikazan korišćenjem tabele koja je grupisana prema oznaci i dozvoljenom broju dana iznajmljivanja određenog filma. Nakon svakog broja dozvoljenog iznajmljivanja filma date oznake postoji zbir svih filmova koje mu pripadaju.

![22](https://user-images.githubusercontent.com/61964257/145212169-9e884dcd-7214-4c78-a967-c48e8b3981da.PNG)


### Zahtev broj :two:: Koliko korisnika je iznajmilo određen film? Koji od tih korisnika su prekoračili rok za vraćanje iznajmljenog filma? Koliki je ukupan profit dobijen od tog filma?

Za potrebe pretrage u izveštaju kreiran je parametar sa opadajućom listom prema kojoj se nakon pretrage filtriraju rezultati. Za korisnike koji nisu prekoračili iznos cene umesto broja 0 stoji “Film je vraćen na vreme!”, dok su oni korisnici koji su film vratili na vreme označeni crvenom bojom. Na samom kraju je izračunato koliko korisnika je iznajmilo ozančen film/filmove, kao i ukupan profit od tog filma ili od svih označenih filmova.

![23](https://user-images.githubusercontent.com/61964257/145212174-8b0f08da-a255-4379-bd2c-7f9eaf4d2bff.PNG)
![24](https://user-images.githubusercontent.com/61964257/145212175-c6685bfd-8b00-40cb-b0f1-4c15a6abc072.PNG)


### Zahtev broj :three:: Kolika je ukupna zarada od iznajmljenih filmova koju su zaposleni Jon Stephens i Mike Hillyer dobili po mesecima 2005. godine?

Zahtev je kreiran korišćenjem *Line with Markers Chart-a* u kom su za ketegoriju odabrani nazivi meseca, a za vrednost obeležje *amount* sabrano uz pomoć funkcije *Sum*.

![25](https://user-images.githubusercontent.com/61964257/145212179-0cc1434f-ff9a-4281-adee-1a319ef53afc.PNG)


### Zahtev broj :four:: Koja kategorija filma je donela najviše prihoda?

Zahtev je prikazan korišćenjem *Bullet Graph Gauge-a* koji prikazuje ukupnu zaradu svake od kategorija. Dodat je i *switch* uslov koji ukoliko je ukupan profit manji od 1600 indikator je crvene boje, ukoliko je profit manji od 1400 indikator je zelene boje i ukoliko je profit manji od 1200 indikator je žute boje. Rezultati istraživanja pokazuju da je *SPORTS* kategorija koja je donela najviše prihoda.

![26](https://user-images.githubusercontent.com/61964257/145212180-c3fd5bd4-4eca-4b37-a0bd-433512b2a8d6.PNG)


### Zahtev broj :five:: Koji je film koji je najčešće puta iznajmljen i koliko puta je taj film iznajmljen?

Zahtev je prikazan korišćenjem *Column Chart-a* u kom je za kategoriju odabrano obeležje *film_title*, a za vrednost serije obeležje *CountRental*. Rezultati pokazuju da je film koji je najviše puta iznajmljen *ROCKETEER MOTHER* sa 16 iznajmljivanja.

![27](https://user-images.githubusercontent.com/61964257/145212184-693bc084-262e-44d9-81d1-133fd4608c42.PNG)


### Zahtev broj :six:: Koja prodavnica je zaradila veći profit od prekoračenog roka iznajmljenih filmova?

Zahtev je prikazan korišćenjem *Pie Chart-a*, a prekoračeni iznosi su grupisani prema obeležju *store_location*. Rezultati pokazuju da je veći profit zaradila prodavnica 47 *MySakila Drive Lethbridge Canada*.

![28](https://user-images.githubusercontent.com/61964257/145212187-ae9d91f6-fcef-43a7-a160-ad888af76963.PNG)
