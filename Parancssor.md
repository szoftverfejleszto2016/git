Git a parancssorból
===================

Git telepítése
--------------

A Git-et Windowshoz a <https://git-scm.com/> címről töltheted le.

A telepítő több eszközt is telepít. Mi ezek közül a Git Bash-t fogjuk használni.
Ez egy Linux terminál, ebbe fogjuk gépelni a parancsokat.

Ha nincs a gépedre telepítve a Git, töltsd le és telepítsd!

Utána indítsd el a Git Bash programot! Az első használatnál meg kell adni a
felhasználónevet és az e-mail címet a következő parancsokkal:

**git config --global user.name** *felhasználóneved*

**git config --global user.email** *e-mail címed*

Klónozás
--------

1.  Jelentkezz be online a GitHub-ra!

2.  Válaszd ki a korábban készített *proba1* repository-t! Kattints a *Clone or
    download* gombra, majd az az ábrán jelzett helyre! ez a vágólapra másolja a
    repository címét.

![](media/f9cc1c4d114a51a1498e36992439e73c.png)

1.  Töröld le a számítógépedről a múltkor klónozott *proba1* mappát. Ezt most
    újra el fogjuk készíteni.

2.  Ezután válts át arra a mappára, amelybe a klónozást szeretnéd! A parancsot
    úgy írtam be, hogy a fájlkezelőből áthúztam a mappát a cd parancsba:

![](media/b769eeaa9c0d8a131803c73330d37e30.png)

1.  Írd be a **git clone** parancsot, és illeszd be a 2-es pontban kimásolt
    címet (Shift+Ins, vagy jobb kattintás és Paste):

![](media/03eebeb2fad2e48737f6c771cc364c5e.png)

1.  Nézd meg a fájlokat (a fájlkezelőben is)! Figyeld meg, hogy van egy rejtett
    *.git* mappa. Ebben tárolja a Git az objektumokat. Soha ne módosítsd ennek a
    mappának a tartalmát!

![](media/bd440700c5becb07f923189c301c2a2c.png)

Új repository
-------------

1.  Válts az egy szinttel feljebb lévő mappába! Hozz létre egy weblap2 mappát,
    majd tedd aktuálissá!

![](media/323ec2a2842f77b6af03ba3cb734ab77.png)

1.  Másold a fájlkezelővel az új weblap2 mappába a kapott fájlokat, majd listázd
    ki őket a dir paranccsal!

![](media/ff38f4e6e954906a59d69c7f8d927e7b.png)

1.  Készíts repository-t a mappából a **git init** paranccsal:

![](media/b601940b32b953b8a9b9a83e00c42002.png)

1.  Add ki a **git status** parancsot:

![](media/98a692208114115c17d2d4f0e758e14a.png)

1.  A Git-ben jelezni kell, hogy mely fájlokat szeretnénk követni. Add hozzá a
    követendő fájlokhoz az aktuális mappa teljes tartalmát! Ezt nevezik
    (staging-nek.) Utána nézd meg újra a státuszt!

![](media/5b89e4edafef5850ee3900333ee0a03a.png)

1.  Készíts pillanatfelvételt a jelenlegi állapotról (commit)! Az üzenet legyen
    alapállapot!

![](media/2919e156660bbb143608dddcbf53e9d6.png)

1.  Utána nézd meg újra a státuszt!

![](media/173c7909b00dee3bc2137a57a1d6bb69.png)

1.  Ezzel a helyi repository-ba mentettük a módosításokat. Nyisd meg a GitHub
    oldalad (jelentkezz be), és készíts egy új, üres repository-t weblap2 néven!

2.  A létrehozás után megjlenő oldalon másold a vágólapra az új repository
    címét:

![](media/ee7a2dffeb3d8346fd1f6307ebc681b8.png)

1.  Utána a bash-ben add meg a távoli repository-t a következő paranccsal (a
    címet az előző lépésben másoltuk a vágólapra)! Ettől kezdve a távoli
    repository-ra az origin névvel hivatkozhatsz. (Más nevet is lehet használni,
    de ezt szokták.)

![](media/ed60ce259c011531a8d94709f9c8055b.png)

1.  Végül másold a helyi repository-t a távoliba (közben be kell jelentkezned a
    GitHub-ra):

![](media/f93cb2185a62403807be57b82a720ea8.png)

1.  Frissítsd a GitHub oldalt, és ellenőrizd a távoli repository-t!

Elágazás
--------

1.  Kezdj egy új ágat zöld néven, és válts át rá! Utána listázd az ágakat!

![](media/223b4a4d8450bfef7bf5d20387b4ec0c.png)

1.  Nyisd meg a helyi repository mappáját (*weblap2*) a Visual Studio Code-ban!  
    

    ![](media/00863a1a4c33f0b9a3d1915cac703777.png)

2.  A Visual Studio Code-ban nyisd meg a *stilusok.css* fájlt, és állítsd át az
    oldal háttérszínét zöldre!

![](media/fe4f8337a148f8314e8541a040d4f4f7.png)

1.  Mentsd a módosítást, majd nézd meg az eredményt a böngészőben!

2.  Nézd meg a státuszt, add hozzá a stage-hez a fájlokat, majd commit-old őket
    a helyi repository-ba!

![](media/db9e3b264e94f49ffba5cb5aeb42f8b9.png)

1.  Utána töltsd fel az új zöld ágat a GitHub repository-ba az alábbi
    paranccsal! Utána ellenőrizd az új ágat a GitHub-on!

![](media/31cb2a9b224b2ccf30967f20b2d9d369.png)

1.  Módosítsd a Visual Studio Code-ban a weblap betűtípusát Cambria, … -ra, és
    mentsd a módosítást! Nézd meg az eredményt a böngészőben!

2.  Commit-old a változásokat a helyi repository zöld ágába! Most egyszerre
    végezd el a stage-elést és a commit-olást:

![](media/ab58b021d04957af68128359ec3a24bf.png)

1.  Ellenőrizd az eddigi commit-okat:

![](media/e340adb3c9d62a283323fe7f2541a62d.png)

1.  Utána töltsd fel a módosításokat a GitHub repository-ba is!

![](media/f87efa6a9a41951461363237be757d0a.png)

1.  Próbaképpen válts vissza a master ágra, és frissítsd a böngészőben az
    oldalt! Utána válts vissza a zöld ágra, és nézd meg így is az oldalt! Mit
    tapasztalsz?

![](media/50b6ce6eebc9c6581417dad0b1d884ce.png)

Módosítások letöltése
---------------------

1.  Válts a böngészőben a GitHub oldalra, és a zöld ághoz adj hozzá egy
    README.md fájlt!

2.  Töltsd le a módosításokat a helyi repository-ba, és listázd ki a tartalmát:

![](media/efe357fc710b18001414feaf4dd0d626.png)

Ágak egyesítése
---------------

1.  Helyben úgy egyesíthetnéd az ágakat, hogy átváltasz a master ágra (**git
    checkout master**), majd kiadod a **git merge zöld** parancsot. Most azonban
    a GitHub-on szeretnénk az egyesítést elvégezni, ezért válts a GitHub
    oldaladra, és a weblap2 projektben válaszd a *Pull request* fület!

2.  Kattints a *New pull request* gombra, válaszd ki a zöld ágat, majd kattints
    a *Create pull request* gombra!

![](media/bd663df9802c883af6c1cfd6eb3b10f6.png)

1.  Írj egy üzenetet, majd itt is kattints a *Create pull request* gombra,

![](media/50229e02d4b04ae4370f5888f0b571d0.png)

1.  Erősítsd meg a műveletet a *Merge pull request*, majd a *Confirm merge* gomb
    megnyomásával!

![](media/9d8aa511766f78c2c631429b80d7e975.png)

1.  Végül töröld a zöld ágat a GitHub-ról a *Delete branch* gombbal!

2.  Válts a bash-re, válts vissza a master ágra, és töltsd le a master ág
    módosításait! Ellenőrizd az oldalt a böngészőben!

![](media/f472dfe36d1ff8b755ead78c3f226cff.png)

1.  Töröld a helyi zöld ágat is!  
    

    ![](media/9f7d8017feb76768553602e180fd753b.png)
