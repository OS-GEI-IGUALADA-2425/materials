# Materials del curs de Sistemes Operatius

|![](figs/logo.png)              |   ![](figs/institute.png)              |
|-----------------|-----------------|
| **Denominació** | Sistemes Operatius |
| **Impartició**  | 1er Semestre del Grau en Enginyeria Informàtica |
| **Professor**   | [Jordi Mateo](mailto:jordi.mateo@udl.cat) |
| **Departament** | [ENGINYERIA INFORMÀTICA I DISSENY DIGITAL]([https://dd](https://deidd.udl.cat/ca/))  |
| **Universitat** | [Universitat de Lleida](https://www.udl.cat) |
| **Escola**      | [Escola Politècnica Superior](https://www.eps.udl.cat) |
| **Guia docent** | [105012](https://guiadocent.udl.cat/html/2024-25_105012) |


## Materials

| Unitat | Diapositives | Apunts | Laboratori | Setmana |
|--------|--------------|--------|------------|---------|
| 0      | [Diapositives](diapositives/SO_tema0.pdf) | [Apunts](apunts/SO_tema0.pdf) | [Laboratori 0](https://os-gei-igualada-2425.github.io/laboratoris/lab0/main.html) | 1 |
| 0      | [Diapositives](diapositives/SO_intro_prog_sistema_1_C.pdf) | |[Laboratori 1](https://os-gei-igualada-2425.github.io/laboratoris/lab1/main.html) | 2 |
| 1      | [Diapositives](diapositives/SO_tema1.pdf) | [Apunts](apunts/SO_tema1.pdf) | | 3 |


## Contingut

- Introducció
- Requisits
- Instal·lació
- Estructura del Repositori
- Contribuir
- Llicència

## Introducció

Benvinguts al repositori de materials del curs. Aquí trobareu totes les diapositives i apunts necessaris per seguir el curs 2024/2025.

## Requisits

Per compilar els materials, necessitareu tenir instal·lat un conjunt d'eines com són:

- [Pandoc](https://pandoc.org/)
- [TeX Live](https://www.tug.org/texlive/)
- [Make](https://www.gnu.org/software/make/)

Per facilitar la compilació dels materials, s'ha proporcionat un fitxer `Makefile` amb les comandes necessàries que utilitzen una imatge Docker amb totes les dependències necessàries. Per tant, únicament cal tenir instal·lat Docker per compilar els materials.

## Instal·lació

Per compilar els materials, seguiu aquests passos:

1. Cloneu el repositori:

    ```bash
    git clone
    ```

2. Utilitzeu el `Makefile` per compilar els materials:

- Si voleu generar les diapositives:

    ```bash
    make diapositives
    ```

- Si voleu generar els apunts:

    ```bash
    make apunts
    ```

## Estructura del Repositori

```text
materials
├── README.md 
├── apunts/ │ 
    ├── tema1.pdf │ 
    ├── tema2.pdf │ 
    └── … 
├── diapositives/ │ 
    ├── tema1.pdf │ 
    ├── tema2.pdf │ 
    └── … 
├── md/
    ├── apunts/
        ├── tema1.md
        ├── tema2.md
        └── …
    ├── diapositives/
        ├── tema1.md
        ├── tema2.md
        └── …
├──Makefile
|──Makefile.diapositives
|──Makefile.apunts
├──Metadata.yaml
├──bibliografia.bib
├──.markdownlint.json
└──LICENSE
```

## Contribuir

1. Feu un fork del repositori.
2. Creeu una branca per la vostra característica (`git checkout -b característica/nova-característica`).
3. Feu commit dels vostres canvis (`git commit -m 'Afegir nova característica'`).
4. Feu push a la branca (`git push origin característica/nova-característica`).
5. Obriu una Pull Request.

## Llicència

Aquest projecte està llicenciat sota la Llicència  GNU General Public License v3.0 - veure el fitxer [LICENSE](LICENSE) per a més detalls.
