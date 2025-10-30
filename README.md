# 💧 DETECTOR DE UMEZEALĂ (DEW DETECTOR) - PROIECT TCAD

## 🚀 Prezentare Generală

Acest depozit conține materialele complete pentru proiectul de **Tehnici CAD (TCAD)**, realizat la **Universitatea Națională de Știință și Tehnologie Politehnica București (UNSTPB)**.

Proiectul constă în designul unui **Detector Simplu și Economic de Rouă (Umezeală Condensată)**, alimentat la **5V c.c.**, destinat protejării dispozitivelor electronice sensibile, precum videorecordere (VTR), camere, copiatoare sau calculatoare.

Circuitul a fost proiectat și simulat folosind suita software **OrCAD 17.2 Lite**.

---

## 🔬 Principiul de Funcționare

Circuitul utilizează elementul senzor de rouă **HDP-07** (fabricat de Hokuriku).

1.  **Senzorul HDP-07** funcționează pe baza unui polimer conductiv a cărui rezistență se modifică drastic la contactul cu umezeala (între **90% și 95%** umiditate relativă).
2.  **Stare Normală:** În repaus, senzorul are o rezistență foarte mică, menținând tranzistorul **T1 (2N2222)** în stare de blocare.
3.  **Detecție:** Când umezeala crește, rezistența senzorului crește, permițând polarizarea tranzistorului T1.
4.  **Ieșire:** T1 intră în conducție și activează **Optocuplorul PC817** (**OPTO ISOLATOR-A**), emițând un semnal de detecție. Optocuplorul asigură izolare galvanică și o ieșire de tip colector deschis.
5.  **Ajustare:** Pragul de sensibilitate este ajustabil cu ajutorul **Potențiometrului P1 (220K)**.

---

## 🧱 Specificații PCB

Placa de circuit imprimat (PCB) respectă următoarele specificații de proiectare:

| Parametru | Valoare | Note |
| :--- | :--- | :--- |
| **Dimensiune PCB** | Pătrată, latura de **60mm** | Dimensiunea laturii |
| **Număr Straturi** | Două straturi electrice (TOP și BOTTOM) | Toate componentele sunt pe stratul TOP. |
| **Lățime Trasee Semnal** | **0.3mm** | |
| **Lățime Trasee Alimentare** | **1.1mm** | |
| **Spațiere Minimă** | **0.25mm** | În toate cazurile |
| **Regulator Tensiune** | **IC1: LM7805/TO** | Stabilește tensiunea de lucru la 5V. |
| **Alimentare Externă** | 9V - 12V DC (Max. 35V) | Intrare prin conectorul J1 (CON2) |

---

## 📁 Conținutul Depozitului

* **`01_Documentatie/`**: Raportul proiectului, schema electrică și lista de materiale (BOM).
* **`02_Proiect_PCB/`**: Fișierele native **OrCAD Capture** și **PCB Editor** pentru modificări ulterioare.
* **`03_Fisiere_pentru_Fabricatie/`**: Fișierele finale (Gerber, Drill Chart) necesare pentru comanda PCB-ului la un producător.
* **`04_Foi_de_Catalog/`**: Datasheet-uri pentru referință tehnică.

---

## 🏫 Informații proiect
Proiect realizat de **Dragotoniu Ionuț-Constantin**

Facultatea de Electronică, Telecomunicații și Tehnologia Informației – UPB

An universitar 2025–2026
