## 📊 Dashboard Power BI – Analiza Sprzedaży E-Commerce (Sklep Rowerowy)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)

Interaktywny, 3-stronicowy raport Power BI dedykowany analizie sprzedaży, marżowości oraz klientów dla europejskiego e-commerce w branży rowerowej (Sprzedaż, Produkt, Klient). Projekt stanowi kompletne rozwiązanie BI – od surowych danych, przez modelowanie i zaawansowane miary DAX, aż po autorski interfejs w Figmie.


<div align="center">

### Wybierz stronę raportu:

<div align="center">

<a href="#strona-1">
  <img src="https://img.shields.io/badge/📄_Przegląd_Sprzedaży-F2C811?style=for-the-badge&logoColor=black" alt="Strona 1">
</a>
<a href="#strona-2">
  <img src="https://img.shields.io/badge/📄_Analiza_Produktów-2A75D3?style=for-the-badge&logoColor=white" alt="Strona 2">
</a>
<a href="#strona-3">
  <img src="https://img.shields.io/badge/📄_Analiza_Klientów-107C41?style=for-the-badge&logoColor=white" alt="Strona 3">
</a>

</div>

<div align="center">


<div align="left">

### 📚 Spis treści
<div id="1-wstęp"></div>
<details>
<summary><b>1. Problem biznesowy i cele projektu</b> <i>(kliknij, aby rozwinąć)</i></summary>

<br>

Zarząd e-commerce rowerowego potrzebował **spójnego wglądu w realną rentowność produktów i klientów**, ponieważ rozproszone dane utrudniały podejmowanie decyzji o marżach i budżetach marketingowych.

**Cele:**
* Zidentyfikowanie, które linie rowerów i akcesoriów faktycznie generują zysk.
* Śledzenie dynamiki przychodów w czasie i wykrywanie sezonowości.
* Określenie profilu najbardziej wartościowego klienta i geograficznego rozkładu zamówień.
</details>

<div id="2-dane"></div>
<details>
<summary><b> 2. Dane do raprotu</b> <i></i></summary>

<br>

##### a. Źródło danych
<small>
* **Pochodzenie i format danych:** Publiczny zbiór danych z platformy **Kaggle**, plik *.csv**
</small>

##### b. Zakres 
<small>
* **Czas:** Dokładna data (dzień, miesiąc, rok)
* **Demografia:** Wiek (liczbowo oraz grupy wiekowe: *Youth*, *Adults*) i płeć klientów.
* **Geografia:** Kraj (*Country*) i region/stan (*State*).
* **Produkty:** Kategoria (*Product_Category*: rowery/akcesoria), Podkategoria (*Sub_Category*) oraz nazwa modelu (*Product*).
</small>
  
##### c. Miary finansowe
  <small>
* **Wolumen i przychody:** *Order_Quantity* (sztuki), *Unit_Price*, *Revenue* (przychód).
* **Koszty i rentowność:** *Unit_Cost*, *Cost*, *Profit* (zysk)
</details>
  </small>

<div id="3-model danych"></div>
<details>
<summary><b> 3. Model danych </b> <i></i></summary>

<br>

Model danych został zorganizowany wokół centralnej tabeli faktów

* **Tabela Faktów (`Fact_Sales`):** Główna tabela transakcyjna zawierająca kluczowe metryki finansowe (koszty, przychody, wolumen) oraz atrybuty klienta i produktu.
* **Tabela Wymiaru (`Dim_Date`):** Dedykowana tabela kalendarza połączona relacją jednokierunkową **1:* (Jeden do Wiele)** z tabelą faktów, umożliwiająca zaawansowaną analizę czasową (Time Intelligence).
* **Tabela Miar (`tb_measures`):** Osobna tabela techniczna służąca jako spójny kontener na wszystkie utworzone miary DAX, co ułatwia zarządzanie kodem.
</details>









<!-- Sekcja Strony 1 -->
<div id="strona-1" align="center">

### 🚲 Strona 1: Ogólny Przegląd Sprzedaży

<img src="sales-overview.gif" alt="Strona 1 - Sales Overview" width="100%">

<a href="#">
  <img src="https://img.shields.io/badge/⬆_Powrót_do_menu-F2C811?style=for-the-badge&logoColor=black" alt="Powrót">
</a>
</div>

<br>


<!-- Sekcja Strony 2 -->
<div id="strona-2" align="center">

### 🚲 Strona 2:  Analiza Produktów

<img src="product_overview.gif" alt="Strona 2 - Product Overview" width="100%">

<a href="#">
  <img src="https://img.shields.io/badge/⬆_Powrót_do_menu-F2C811?style=for-the-badge&logoColor=black" alt="Powrót">
</a>
</div>

<br>

<!-- Sekcja Strony 3 -->
<div id="strona-3" align="center">

### Strona 3:  Analiza Klientów

<img src="customer_overview.gif" alt="Strona 3 - Customer Overview" width="100%">

<a href="#">
  <img src="https://img.shields.io/badge/⬆_Powrót_do_menu-F2C811?style=for-the-badge&logoColor=black" alt="Powrót">
</a>
</div>

<br>





