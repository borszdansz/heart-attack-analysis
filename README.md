# Szívroham kockázati elemzés

A projekt célja egy adatelemzés volt szabadon választható témában. A választás a szívinfarktus gyakorisága volt különböző változók szerint. 
## Csapat

Borszéki Dániel - első éves matematika alapszakos hallgató

## Mit csinál a notebook?
* A notebook elsőnek telepíti a szükséges programcsomagokat, majd importálja ezeket.
* A data/ mappából betölti az adatokat, mely egy .csv fájlban (táblázat) van elmentve, majd megjeleníti az első néhány sort.
* A változók sorszáma, neve és típusát megjeleníti, majd alapvető statisztikai jellemzőkkel (számuk, medián, minimum érték, stb.) jellemzi őket.
* Hiányzó értékeket ellenőrzi, ha talál, akkor annak a változónak hiányzik előfordulása(i).
* Matematikai statisztikai vizualizációk követik ezeket:
  * Elsőnek az életkor eloszlása az adatok között
  * Majd az életkor és a szívroham közötti kapcsolat
  * A nem szerinti eloszlás
  * Az enzimek emelkedése és a szívroham kapcsolata
  * A pulzusszám és szívroham kapcsolata <<-- itt le kellet vágni a kiugró értékeket, mert nem lett volna látványos velük.
  * Végül egy korrelációs mátrix, melyben a különböző változók egymáshoz képesti viszonyait tekinthetjük meg.
  * Majd kiértékelés
   
## Az adatokról
Az adatok a [Kaggle](https://www.kaggle.com/datasets/fatemehmohammadinia/heart-attack-dataset-tarik-a-rashid?resource=download) nevű weboldalon találtam. Az iraqi Erbil városi Zheen kórházban jegyezték fel ezeket az adatokat 2019 január és május között.
### A változók:
**Kor** (age): Életkor\
**Nem** (gender):  0: Nő ; 1: Férfi\
**Pulzus** (heart rate): Percenkénti szívverés. Egészséges tartomány nyugalomban 60-100.\
**Szisztolés vérnyomásérték** (systolic blood pressure): A szív összehúzódásakor keletkező maximális nyomás. Ha krónikusan magas, az szívinfarktushoz vezethet.\
**Diasztolés vérnyomásérték** (diastolic blood pressure): A szív pihenési fázisában mért nyomás. Ha tartósan alacsony, az szívinfarktushoz vezethet.\
**Vércukorszint** (blood sugar): A vér glükóz tartalma. A egészséges szint 110mg/dl körül mozog.\
**Kreatin-kináz** (ck-mb): A szívizomban fordul elő. Megemelkedett szintje a szivinfarktus korai diagnosztikai jele\
**Troponin** (troponin): Megemelkedett szintje infarktust jelezhet. Más klinikai képpel is jelentkezhet, ezért van szükség más enzim, pl *Kreatin kináz* mérésére.

## Futtatás (CMD-ben)
1. "pip install -r requirements.txt" Telepítjük a szükséges programcsomagokat. ("pip install pandas numpy matplotlib" is működik)
2. "jupyter notebook" Notebook futtatása, itt a projekt mappába kell navigálni.




## A program telepítése és futtatása

