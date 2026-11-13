# Osnovi-robotike-22.EAI044

## Opis projekta

Ovaj repozitorijum sadrži implementaciju i simulaciju SCARA robota sa 3 stepena slobode (3-DOF), u okviru predmeta Osnovi robotike.

## DH parametri

Kinematički model SCARA robota definisan je primenom Denavit–Hartenberg (DH) konvencije.

| Zglob (i) |  ai |  αi |      di     | θi    |
| :-------: | :-: | :-: | :---------: | :-:   |
|     1     |  a1 |  0  |      d1     | θ1\*  |
|     2     |  a2 |  0  |      0      | θ2\*  |
|     3     |  0  |  0  |    d3 + d3\*|  0    |

## Struktura projekta

```text
model/           Model robota (URDF)
scara_robot/     Python implementacija
  kinematika/    Kinematika
  simulacija/    Kod vezan za simulaciju
test/            Testiranje implementacije
```

## Podešavanje okruženja

Za upravljanje Python okruženjem koristi se Conda.

Kreiranje okruženja:

```bash
conda env create -f environment.yml
```

Aktiviranje okruženja:

```bash
conda activate scara_robot
```

Instalacija potrebnih Python biblioteka:

```bash
pip install -r requirements.txt
```
