## Általános információ


## 7 feszültséget kell mérni
- 3db fázisfeszültség (fönt)
	- U_L1 = 234 V
	- U_L2 = 234 V
	- U_L3 = 235 V
- A villanymotor teste és a fázis között: 230V kell, hogy legyen (pl a csavarnál lehet érinteni)
		- U_L1-PE = 233 V
- 3db vonali feszültség: közel a motor kapcsaihoz, pl a mágneskapcsoló kimenő oldalánál 
	- U_L1-2 = 406 V
	- U_L2-3 = 405 V
	- U_L1-3 = 401 V 
### Fogyasztás méréshez
* A háromfázisú digitális fogyasztásmérő nulla sarka a feszültségmérés miatt kell, 2.5-ös vezetékek vannak hozzá.
* Három led villog az egy-egy fázis fogyasztását mutatva, ha az egyik nem villog, ott nincs feszültség: sánta üzem. Baj.
* Fogyasztásméréshez a 4. led: 
	- 800imp/kWh
	- 1.25Wh elfogyasztott energiamennyiség
	- (ennél a motornál kb 1-2 perc míg felvillan)
- t=111sec

### Amper mérés
- I_1 = 0,288 A
- I_2 = 0,314 A
- I_3 = 0,297 A

### Számítások

- S1 = I_L1 · U_L1 = 0,288 A · 234 V = 67.3VA
- S2 = I_L2 · U_L2 = 0,314 A · 234 V = 72,77 VA
- S3 = I_L3 · U_L3 = 0,297 A · 235 V = 69,79 VA

- 800imp/kWh --> 800imp/1000Wh
- 1 imp = 1000 / 800 = 1,25
- P = 3600 / 111min · 1,25 = 40.54 kW
- cos φ = P / S  = 40,54 kW / 209,95 VA = 0,19
- (ez nem kell: S = S1 + S2 + S3 = 202,585)

## Egyéb információk

- Ha a nulla és védővezeték között 1V-nál nagyobb feszültséget mérünk bármikor, nagy a baj, veszélyes!
- Ha üresjáraton forog a motor, a cos φ-je rossz, ha terhelem akkor jobb: ezért nem szabad túlméretezni a motort.
- A kismegszakítókat a P-hez kell méretezni (a hatásos, tengelyről levehető teljesítményt adják meg a motoroknál)
- Mérésnél, ha 1 vezetéket fogok át (lakatfogó, Amper mérés) akkor valós értéket mér, ha 3 fázist akkor 0-t. Ha kettő fázist fogok át, a különbözetét mutatja (a 3. vezeték értékét)