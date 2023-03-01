# nemetigek
Ezzel a kis programmal gyakorolhatjuk a német igék múltbeli képzését.

## Szükséges dolgok
A következők szükségesek a program működtetéséhez:
- internetkapcsolat,
- egy JavaScriptet támogató böngésző (a legtöbb mai böngésző, mint például a Chrome, Firefox, Edge, Safari, Brave, Opera támogatja ezt),
- egy CSV-fájl, amelyben a szavak vannak (egy ilyen fájlt könnyen létrehozhatunk egy Excel-táblázatból; fontos, hogy pontosvesszővel elválasztott legyen és UTF-8 kódolású).

## Telepítés
A program telepítése nagyon egyszerű, de fontos, hogy a fájlokat **letöltsük** és ne a felhőből próbáljuk meg elérni:
1. **Töltsük le** a *Releases* oldalon a **HTML-fájlt** és mentsük el (mindegy, hogy hová).
2. **Töltsünk le** egy **CSV-fájlt**, amit valószínűleg a tanárunktól kaphatunk (mindegy, hogy hová mentjük).
3. **Nyissuk meg** a **HTML-fájlt** a kedvenc böngészőnkben.

## Működés
1. Miután megnyitottuk a HTML-fájlt, kattintsunk a **Fájl kiválasztása** (előfordulhat, hogy a különböző böngészőkben más neve van a gombnak) gombra és válasszuk ki a CSV-fájlunkat.
2. Ezután félkövéren megjelenik egy véletlenszerűen kiválaszott szó. Töltsük ki a mezőket (ügyeljünk a kis- és nagybetűkre, mert a rendszer ezeket megkülönbözteti). Ha egy szó nem rendhagyó, akkor az E/3 mezőt hagyjuk üresen.
3. Az **Ellenőrzés** gombra kattintva láthatjuk, hogy helyesek voltak-e válaszaink és ha nem, akkor mellettük zölddel a helyes válaszokat. Alul nyomon követhetjük eddigi teljesítményünket.
4. A **Tovább** gombra kattintva új szót kérhetünk.
5. Ha minden szóval **végeztünk**, egy felugró üzenet tájékoztat minket erről. Az *OK* (megint, ez az egyes böngészőkben eltérhet) gombra kattintva megtekinthetjük eredményünket.
6. Ha újra akarjuk kezdeni, vagy más szavakkal folytatnánk, frissítsük le az oldalt és ismételjük meg a fenti lépéseket.

## CSV-fájl készítése
Excelből ilyet nagyon könnyen készíthetünk a *Mentés másként* fül alatt a *.csv (pontosvesszővel elválasztott UTF-8) opciót választva fájlkiterjesztésként. (Fontos, hogy UTF-8 kódolású legyen, mert más esetben egyes karakterek nem jól jelenhetnek meg.)
A mintatablazat.csv fájl mintául szolgál, nyugodtan töltsük le, vizsgáljuk meg, valami olyasminek kell lennie az általunk készítettnek.
Csak néhány kritériuma van a CSV-fájlnak/táblázatnak:
- Az első sort figyelmen kívül hagyja a program, így az bármi lehet
- Az első oszlopban az ige szótári alakja kell, a másodikban az E/3, ha van, a harmadikban a präteritum, a negyedikben a perfekt, az ötödikben a magyar megfelelője. Fontos, hogy ne rövidítsünk, mert a rövidítést nem tudja feloldani a program, tehát *csak* a rövidített lesz a jó megoldás.
- (A CSV-fájl utolsó sorát a program figyelmen kívül hagyja, mert ez általában egy üres sor. Ha Excelből készítettük a fájlt, akkor ezzel nem kell foglalkozni.)

---

Ez a projekt a Papa Parse nevű könyvtárat használja, amely a MIT lincensz alatt érhető el.