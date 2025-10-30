# 💧 Detector de Umezeală (Sondă de Rouă) - Proiect TCAD ETTI-UNSTPB

## 🌟 Prezentare Generală

[cite_start]Acest depozit conține toate fișierele necesare (schemă electrică, layout PCB, fișiere de fabricație și documentație) pentru un **Detector de Umezeală/Rouă** simplu și economic, dezvoltat ca proiect pentru disciplina Tehnici CAD la Facultatea de Electronică, Telecomunicații și Tehnologia Informației (ETTI) [cite: 4] [cite_start]din cadrul Universității Naționale de Știință și Tehnologie Politehnica București (UNSTPB)[cite: 1].

### Caracteristici Cheie
* **Tensiune de Alimentare:** 5V c.c. (Circuitul acceptă intrare externă de 9V - 18V) [cite_start][cite: 33, 41].
* [cite_start]**Senzor:** Element senzor de rouă **HDP-07** (Hokuriku)[cite: 16, 35].
* [cite_start]**Principiul de Detecție:** Bazat pe modificarea rezistenței unui polimer conductiv la umiditate ridicată (90-95% umiditate relativă), care activează tranzistorul T1 (2N2222)[cite: 17, 18, 45].
* [cite_start]**Ieșire:** Optocuplă **PC817** (izolare galvanică, ieșire colector deschis)[cite: 20, 42, 43].
* [cite_start]**Proiectat pentru:** Detectarea umezelii condensate în echipamente electronice sensibile (camere, copiatoare, VTR-uri)[cite: 15, 21].
* [cite_start]**Ajustare:** Pragul de sensibilitate este ajustabil cu potențiometrul P1 (220K)[cite: 47].

## 🛠️ Structura Proiectului

* [cite_start]**`Proiect PCB/`**: Conține fișierele sursă realizate în programul **OrCAD 17.2 Lite** [cite: 230] (Schema și Layout).
* [cite_start]**`Fisiere pentru Fabricatie/`**: Conține fișierele **Gerber** necesare pentru a trimite PCB-ul la producție (Layer Copper TOP [cite: 218][cite_start], BOTTOM[cite: 219], Soldermask, Silkscreen etc.).
* [cite_start]**`Documentatie/`**: Include **Schema Electrică**, **Bill of Materials (BOM)**[cite: 151], și documentația completă a proiectului.
* **`Foi de catalog/`**: Specificațiile tehnice (Datasheets) pentru componentele critice.

## ⚙️ Specificații PCB

Placa este proiectată conform următoarelor reguli:
* [cite_start]**Straturi (Layers):** Două straturi electrice (TOP și BOTTOM)[cite: 23].
* [cite_start]**Dimensiuni PCB:** Placă pătrată cu latura de **60mm**[cite: 25].
* [cite_start]**Lățime Trasee:** * Semnal: **0.3mm** [cite: 24]
* [cite_start]Alimentare: **1.1mm** [cite: 24]
* [cite_start]**Spațiere (Spacing):** **0.25mm** în toate cazurile[cite: 24].
* [cite_start]**Prindere:** Trei găuri de prindere plasate în colțuri (la 1.5M distanță de colț)[cite: 25].

## 🔗 Componente Cheie (Conform BOM)

| Referință | Denumire | Valoare / Model | Capsulă |
| :---: | :---: | :---: | :---: |
| **IC1** | Regulator de Tensiune | LM78L05/TO | [cite_start]TO220AB [cite: 161] |
| **T1** | Tranzistor NPN | 2N2222 | [cite_start]TO92 [cite: 161] |
| **P1** | Potențiometru | 220K | [cite_start]TRIM_BI_23AL (SMD) [cite: 161, 154] |
| **PC817/ISO1** | Optocuplor | PC817/ISO1 | [cite_start]DIP4_3 [cite: 161] |
| **HDP-07** | Senzor de Rouă | SENSOR | [cite_start]JUMPER2 [cite: 161] |
