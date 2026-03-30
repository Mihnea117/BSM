# Sursa de Alimentare Stabilizata cu Iesiri Multiple (Reglabila si Fixe)

Proiect realizat in cadrul disciplinei **Bazele Sistemelor Mecatronice** (Anul 2 - FIMM, UPB).

## 📌 Descriere Proiect
Obiectivul principal al acestui proiect este proiectarea si simularea unei surse de tensiune capabile sa asigure un nivel constant si precis al alimentarii, eliminand fluctuatiile provenite din reteaua de curent alternativ sau modificarile sarcinii la iesire. Sistemul este conceput pentru utilizarea in laboratoare de electronica si prototipare, oferind flexibilitate prin cele trei ramuri de iesire independente.

## 🚀 Detalii Tehnice si Functionare

### 1. Arhitectura Sistemului
* **Transformare:** Un transformator (TR1) coboara tensiunea de retea la un nivel sigur si utilizabil pentru componentele electronice.
* **Redresare:** O punte redresoare (BR1) converteste tensiunea alternativa in tensiune continua pulsatorie (redresare completa).
* **Filtrare:** Se utilizeaza un inductor (L1) si condensatori de filtrare (C1) pentru a netezi tensiunea si a reduce riplul.
* **Reglare:** Tensiunea filtrata este dirijata catre trei regulatoare de tip liniar pentru a obtine valorile finale stabilizate.

### 2. Specificatii Iesiri
* **Iesire Reglabila (1.25V - 37V):** Implementata cu ajutorul regulatorului **LM317**, permitand ajustarea manuala a tensiunii prin intermediul unui potentiometru (RV1).
* **Iesire Fixa 12V:** Stabilizata prin regulatorul **LM7812**, destinata sistemelor de control si echipamentelor care necesita acest prag standard.
* **Iesire Fixa 5V:** Stabilizata prin regulatorul **LM7805**, utilizata frecvent pentru alimentarea microcontrolerelor, senzorilor si modulelor digitale.

### 3. Monitorizare si Siguranta
* **Semnalizare Vizuala:** Fiecare ramura este echipata cu LED-uri albastre care indica functionarea activa si prezenta tensiunii pe iesire.
* **Masurare:** Schema include voltmetre virtuale pentru monitorizarea in timp real a valorilor livrate pe fiecare port.
* **Protectii Integrate:** Regulatoarele utilizate dispun de protectie interna la supracurent, protectie termica si siguranta in caz de scurtcircuit.

## 🛠 Software Utilizat
* **Proteus Design Suite:** Folosit pentru realizarea schemei electrice detaliate, simularea interactiva si analiza functionala a intregului sistem.

## ✅ Avantajele Solutiei
* **Stabilitate ridicata:** Mentine tensiunea de iesire in limite foarte stranse chiar si la variatii ale tensiunii de intrare.
* **Zgomot redus:** Regulatoarele liniare asigura o ondulatie minima, fiind ideale pentru circuite sensibile.
* **Versatilitate:** Permite alimentarea simultana a mai multor dispozitive cu cerinte de tensiune diferite (5V, 12V si variabil).

---
**Autor:** Neagu Mihnea-Stefan - Grupa 522B.
