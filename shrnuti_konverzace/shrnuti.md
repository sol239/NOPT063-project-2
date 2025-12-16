(ChatGPT)

## 1️⃣ Úvod do architektury SW systémů

* Softwarová architektura popisuje **vysokou strukturu systému**, komponenty a jejich interakce.
* Cílem je **zajištění kvality, flexibility a udržovatelnosti** systému.
* Klíčové role architektury: plánování, dokumentace, rozhodování.
* Zdroje: [SEI – Software Architecture](https://resources.sei.cmu.edu/library/subject-areas/software-architecture/)

---

## 2️⃣ Architektonické styly

* **Vrstvená (Layered)** – logické vrstvy, separace zodpovědností.
* **Client–Server** – centralizovaná logika, komunikace přes síť.
* **Monolit** – jeden celek, jednoduchý na začátku, horší škálovatelnost.
* **Microservices** – malé nezávislé služby, škálovatelnost.
* **SOA** – služby s Enterprise Service Bus, integrace podnikových systémů.
* **Event‑Driven** – komunikace přes události, real‑time systémy.
* **Pipe‑and‑Filter** – datové toky a sekvence zpracování.
* **P2P** – decentralizované sítě.
* **Hexagonální / Clean Architecture** – oddělení jádra od adaptérů.
* Zdroje: [Software Architecture Guild](https://software-architecture-guild.com/guide/architecture/fundamentals/architecture-styles/)

---

## 3️⃣ Pohledy na SW architekturu

* Pohledy umožňují různým stakeholderům **vidět systém podle svých potřeb**.
* **4+1 Views** (Philippe Kruchten):

  1. Logický – co systém dělá
  2. Procesní – chování za běhu
  3. Vývojový – modulární struktura kódu
  4. Fyzický – nasazení a infrastruktura
  5. Scénáře / Use Cases – případy použití
* Alternativy: C4 model, ISO/IEC 42010.
* Zdroje: [Wikipedia – 4+1 view model](https://en.wikipedia.org/wiki/4%2B1_architectural_view_model)

---

## 4️⃣ Modelování a dokumentace SW architektury

* **Modelování** – vytváření diagramů a modelů pro pochopení systému.
* **Dokumentace** – soubor artefaktů: struktura, rozhodnutí, pohledy.
* Standardy: UML, C4, ArchiMate.
* ADR (Architecture Decision Records) – zaznamenání důležitých rozhodnutí.
* Doporučení: udržovat dokumentaci živou, používat nástroje (PlantUML, Structurizr, Archi).
* Zdroje: [Software System Design – Modeling & Documentation](https://softwaresystemdesign.com/software-architecture-design/modeling-and-documentation/architecture-documentation-best-practices/)

---

## 5️⃣ Kvalitativní atributy SW architektury

* **Dostupnost, Modifikovatelnost, Výkonnost, Bezpečnost, Integrovatelnost, Znovupoužitelnost, Testovatelnost, Uživatelská přívětivost**.
* Slouží k definici *nefunkčních požadavků* a ovlivňují architektonická rozhodnutí.
* Zdroje: [Wikipedia – FURPS model](https://en.wikipedia.org/wiki/FURPS)

---

## 6️⃣ Vybrané architektonické vzory

* **Vrstvená, Client–Server, Event‑Driven, Microservices, Hexagonální, Microkernel, Space-Based, CQRS, P2P, Strangler, MVC**
* Vzory řeší opakující se architektonické problémy a podporují škálovatelnost, modularitu a udržovatelnost.
* Zdroje: [GeeksforGeeks – Software Architecture Patterns](https://www.geeksforgeeks.org/software-engineering/types-of-software-architecture-patterns/)

---

## 7️⃣ Datová architektura

* Popisuje **strukturu, toky, úložiště a správu dat** napříč systémy a organizací.
* Klíčové komponenty: datové modely (konceptuální, logické, fyzické), datové toky, úložiště, governance, přístup.
* Důležitá pro: kvalitu, bezpečnost, analytiku, AI/ML, integraci a rozhodování.
* Zdroje: [SAP – What is Data Architecture](https://www.sap.com/cz/resources/what-is-data-architecture)

---
