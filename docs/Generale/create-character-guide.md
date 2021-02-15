# Creazione di un personaggio

## Scegli una classe

Indica la classe scelta nel campo Class&Level

Esempio: Monaco

## Scegli una razza

Indica la razza/sottorazza scelta nel campo race

Esempio: Umano

## Statistiche base

Lancia `4d6` 6 volte. Per ogni risultato, scarta il valore più basso e somma gli altri tre.
Assegna questi numeri alle statistiche base (STR / DEX / COS / INT / WIS / CHA)

Esempio:

```
6 6 5 4 ==> 17 DEX
6 5 4 3 ==> 15 CON
5 5 4 1 ==> 14 STR
4 3 3 2 ==> 10 WIS
4 3 2 1 ==> 9  INT
2 2 1 1 ==> 5  CHA
```

## Scegli il background

Esempio: forestiero

## Applica tratti di razza

Applica i bonus di caratteristica della razza scelta.

Applica la velocità e altri tratti, come per esempio la lingua.

Se competente in tiri salvezza o skill, aggiungi marcatore di proficiency sulle abilità corrispondenti.

Esempio

```
Umano: +1 a tutte le caratteristiche

STR 14 => 15
DEX 17 => 18
CON 15 => 16
INT  9 => 10
WIS 10 => 11
CHA  5 =>  6

Velocità base: 9 metri
Linguaggi: Comune + linguaggio a scelta
```

## Applica caratteristiche del background

Esempio

```
Forestiero

Competenze nelle abilità: Atletica, Sopravvivenza ==> aggiungi proficiency per entrambe
Competenze negli strumenti: scegli uno strumento musicale
Linguaggi: aggiungine uno
Equipaggiamento: aggiungi gli elementi riportati all'equip
Seleziona Tratto Caratteriale, Ideale, Legame e Difetto.
```

## Applica caratteristiche della classe

### Proficiency

In base alla classe scelta e al livello, copiare il valore corretto. Ricorda che, salendo di livello, il valore della proficiency potrebbe variare e quindi potresti dover ricalcolare altri valori.

```
Esempio: Monaco Liv 1

Proficiency: +2
```

### Modificatori statistiche base

Usa la formula `FLOOR((STAT-10)/2)` per calcolare i modificatori.

| Valore | Modificatore | Valore | Modificatore | Valore | Modificatore |
| ------ | ------------ | ------ | ------------ | ------ | ------------ |
| 1 | -5 | 11 | +0 | 21 | +5 |
| 2 | -4 | 12 | +1 | 22 | +6 |
| 3 | -4 | 13 | +1 | 23 | +6 |
| 4 | -3 | 14 | +2 | 24 | +7 |
| 5 | -3 | 15 | +2 | 25 | +7 |
| 6 | -2 | 16 | +3 | 26 | +8 |
| 7 | -2 | 17 | +3 | 27 | +8 |
| 8 | -1 | 18 | +4 | 28 | +9 |
| 9 | -1 | 19 | +4 | 29 | +9 |
| 10 | +0  | 20 | +5 | 30 | +10 |

Esempio:

```
Classe monaco:

STR 15 => +2
DEX 18 => +4
CON 16 => +3
INT 10 => +0
WIS 11 => +0
CHA  6 => -2

Punti vita massimi: 8 + COS = 8 + 3 = 11

Competenze:
- Armatura: nessuna
- Armi: Armi semplici, spade corte
- Strumenti: un tipo di strumenti da artigiano o uno strumento musicale a scelta
- Tiri salvezza: Forza, Debolezza ==> aggiungi proficiency su saving throws
- Abilità: Due a scelta tra Acrobazia, Atletica, Furtività, Intuizione, Religione, Storia ==> Religione, Storia, aggiungi proficiency su skills
```

### Calcolo modificatori tiri salvezza

Per ogni tiro salvezza, se si ha proficiency, la formula da applicare è `FLOOR((STAT-10)/2) + PROFICIENCY`. Altrimenti, `FLOOR((STAT-10)/2)`.

| Caratteristica | Valore | Tiro salvezza |
| -------------- | ------ | ------------- |
| STR | +2 | +4 :material-check-circle:{: .highlight } |
| DEX | +4 | +6 :material-check-circle:{: .highlight } |
| CON | +3 | +3 |
| INT | +0 | +0 |
| WIS | +0 | +0 |
| CHA | -2 | -2 |

\* valore massimo: 5

### Calcolo modificatori skills

Per ogni skill, se si ha proficiency, la formula da applicare è `FLOOR((STAT-10)/2) + PROFICIENCY`.
Se non si ha proficiency, `FLOOR((STAT-10)/2)`.

| Attributo             |                                            | Attributo             |                                            |
| --------------------- | ------------------------------------------ | --------------------- | ------------------------------------------ |
| Acrobatics (Dex)      | +4                                         | Medicine (Wis)        | +0                                         |
| Animal Handling (Wis) | +0                                         | Nature (Int)          | +0                                         |
| Arcana (Int)          | +0                                         | Perception (Wis)      | +0                                         |
| Athletics (Str)       | +4 :material-check-circle:{: .highlight }  | Performance (Cha)     | -2                                         |
| Deception (Cha)       | -2                                         | Persuasion (Cha)      | -2                                         |
| History (Int)         | +0                                         | Religion (Int)        | +0                                         |
| Insight (Wis)         | +2 :material-check-circle:{: .highlight }  | Sleight of Hand (Dex) | +4                                         |
| Intimidation (Cha)    | -2                                         | Stealth (Dex)         | +6 :material-check-circle:{: .highlight }  |
| Investigation (Int)   | +0                                         | Survival (Wis)        | +2 :material-check-circle:{: .highlight }  |

## Passive wisdom

Formula: `10+WIS`

Esempio

```
Passive Wisdom: 10+0 = 10
```

## Armor class

A meno che la classe non indichi altrimenti (e.g.: Monaco `10+DEX+WIS`), la classe armatura dipende da armatura/scudo utilizzati, vedi p. 145 del MdG.

## Initiativa

Formula: `DEX`

Esempio

```
Iniziativa: +5
```

## Caratteristica da incantatore

Caratteristica da incantatore, CD tiro salvezza incantesimi e Bonus di attacco incantesimi sono tutti definiti dalla classe.

Esempio

```
Caratteristica da incantatore=WIS
CD tiro salvezza incantesimi=8+WIS+PROFICIENCY
Bonus di attacco incantesimi=n.a.
```

Completare quindi le informazioni mancanti su background, aspetto o altre caratteristiche definite col master.