Bevezetés
=========

Alapfogalmak
------------

**Version control** (Verziókövetés): Változások követése, előző változatok
megőrzése, szükség esetén visszatérés egy korábbi változathoz.

Egy program írása közben különböző változatokat mentünk. Mindegyik az előző
továbbfejlesztése, bővítése. Néha nem válik be a módosítás, ilyenkor vissza kell
térni egy korábbi változathoz.

![](media/e84495ce9af5ef7d48bb24d602fde8d0.png)

Munka közben a lemezre gyakran mentünk, de csak azokat a változatokat kell
megőrizni, amelyek egy-egy komolyabb módosítást tartalmaznak.

![](media/2a99d5ba6344b7e4e81d7a3e8395745b.png)

A szoftverek általában sok fájlból állnak, és mindegyiket követni kell.

**Repository** (raktár): A projekthez tartozó fájlok tarolására szolgál.
Általában egy mappa, amelyben almappák is lehetnek.

Ha kézzel végezzük a verziókövetést, a mappánk így nézhet ki:

![](media/4cf658c1f087e46def1a62b663d1a4fd.png)

Több fájl esetén az egész mappából készíthetünk több változatot.

**Commit**: Egy pillanatfelvétel a fájlokról. (RevXX, filefixup-XX)

Igeként *to commit*: egy pillanatfelvételt készíteni és elmenteni.

**Branch**: Elágazás. Több változatot fejlesztünk.

Például:

![](media/95d356fac33156422cff6dbd6242e9ba.png)

Git
---

A legelterjedtebb verziókezelő rendszer (version control system). Linus Torvalds
vezetéséve készítették a Linux kernel fejlesztéséhez.

**Distributed repository**: Mindenkinek saját, helyi másolata van a
repository-ról, és abban dolgozik. (Internet nélkül is tud dolgozni.) A
módosításokat időnként át kell másolni a többiek példányaiba is.

![](media/71c3b058736c744bec5438a024fe64b7.png)

**Branching**: A fejlesztők külön ágakon dolgoznak, amelyeket később
összefésülnek.

![](media/d93d30541d37f86b7ad38b5a1d88af5a.png)

**Staging area**: Itt adjuk meg, hogy az új és a módosított fájlok közül mit
szeretnénk commit-olni a repository-ba.

GitHub
------

Egy olyan szolgáltatás (<https://github.com/>), ahol tárolhatjuk, kezelhetjük és
megoszthatjuk a Git repository-kat.

A szolgáltatás igénybevételéhez regisztrálni kell név, e-mail cím és jelszó
megadásával.

Kétféle terv (plan) közül választhatunk:

-   *free*: ingyenes, de csak nyilvános (public) projektjeink lehetnek. Mi ezt
    fogjuk használni.

-   *fizetős*: fizetős, de lehetnek privát projektjeink is.

Feladat
-------

Regisztrálj a gitHub szolgáltatásra, majd jelentkezz be!

GitHub Desktop
--------------

Asztali program, amely grafikus felületen kezeli a helyi Git repository-kat és a
GitHub-on lévőket is.

![](media/c53e08195965ab21a3e67eb972d07398.png)

Feladat
-------

Töltsd le a GitHub Desktop programot (https://desktop.github.com/), és
telepítsd!
