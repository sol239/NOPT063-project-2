(ChatGPT)

### **1. Úvod do architektur SW systémů**

* **SW architektura** popisuje **strukturu systému**, jeho komponenty a vztahy mezi nimi.
* Slouží k **řízení složitosti** a zajištění kvalitativních atributů (výkonnost, bezpečnost, modifikovatelnost…).
* Hlavní cíle: **komunikace mezi týmy**, **základ pro rozhodnutí o návrhu**, **základ pro dokumentaci a údržbu**.
* Architektura se tvoří na **vysoké úrovni abstrakce**, nezabývá se detaily implementace.

---

### **2. Architektonické styly**

* **Monolitický styl:** všechny funkce v jedné aplikaci. Jednoduchý, ale hůře škálovatelný a modifikovatelný.
* **Klient-server:** klient žádá služby, server je poskytuje. Odděluje UI a logiku.
* **Vrstevnatá architektura:** systém rozdělen do vrstev (prezentace, logika, data). Každá vrstva komunikuje jen s vrstvou pod ní.
* **Pipes & Filters:** data proudí přes filtry (transformace dat), vhodné pro zpracování toků dat.
* **Event-driven:** komponenty reagují na události. Hodí se pro asynchronní systémy.
* **Microservices:** malé nezávislé služby, komunikují přes API, dobré pro škálovatelnost a modifikovatelnost.

---

### **3. Pohledy na SW architekturu**

* **Logický pohled:** popisuje hlavní komponenty a jejich interakce.
* **Fyzický pohled:** zobrazuje rozmístění SW na HW (servery, sítě).
* **Procesní pohled:** popisuje dynamické chování systému a tok dat mezi procesy.
* **Datový pohled:** zaměřuje se na strukturu a tok dat.
* **Vývojový pohled:** zobrazuje modulární strukturu pro vývoj a údržbu.

---

### **4. Modelování a dokumentace SW architektury**

* **Cíle:** sdílení znalostí, plánování změn, usnadnění údržby.
* **Standardy:** UML (Use Case, Class, Component, Deployment diagrams), ArchiMate, C4 model.
* **Důležité dokumenty:**

  * Diagram komponent
  * Diagram nasazení
  * Diagram toků dat
  * Specifikace rozhraní a kontraktů

---

### **5. Kvalitativní atributy SW architektury**

* **Dostupnost (Availability):** systém je přístupný po určitou dobu, závisí na redundanci a odolnosti vůči chybám.
* **Modifikovatelnost (Modifiability):** snadná změna funkcí nebo komponent.
* **Výkonnost (Performance):** rychlost a efektivita zpracování.
* **Bezpečnost (Security):** ochrana proti neoprávněnému přístupu a útokům.
* **Integrovatelnost (Integrability):** schopnost připojit další systémy nebo moduly.
* **Znovupoužitelnost (Reusability):** komponenty lze použít v různých projektech.
* **Testovatelnost (Testability):** snadná kontrola funkčnosti a kvality systému.
* **Uživatelská přívětivost (Usability):** intuitivní a jednoduché používání systému.

---

### **6. Vybrané architektonické vzory**

* **Model-View-Controller (MVC):** odděluje data (model), prezentaci (view) a logiku (controller).
* **Layered (vrstevnatý):** logika rozdělena do vrstev, každá má jasnou zodpovědnost.
* **Repository:** centrální úložiště dat, ke kterému přistupují různé komponenty.
* **Broker:** komponenty komunikují přes zprostředkovatele (middleware).
* **Peer-to-Peer:** všechny uzly mají stejné postavení, spolupracují přímo.

---

### **7. Datová architektura**

* **Zaměřuje se na správu a tok dat v systému.**
* Obsahuje:

  * Datové modely (ER diagramy, relační, NoSQL)
  * Datové sklady a jezera (data warehouses, data lakes)
  * Datové toky a integrace
  * Strategie správy dat (security, zálohování, kvalita dat)

---
