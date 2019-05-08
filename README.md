# Sustainability

A Clojure library designed to help you live sustainably.

## Usage

To estimate how much CO2 was produced in a given year per capita

```clj
(co2-by-year-in-finland 1979) ; => 11.4034573078207
(co2-by-year-in-finland 2000) ; => 10.1284741400511
```

To estimate how much a person of a given age creates CO2 emissions compared to average over lifetime.

```clj
(co2-multiplier-by-age-finland 1) ; => 0.1433125171218903
(co2-multiplier-by-age-finland 39) ; => 1.2666295009137765
```

To estimate how many tons of CO2 emissions there were for someone alive during a certain time period

```clj
(co2-over-life-in-finland 1969 2008) ; => 311.03141542755174
(co2-over-life-in-finland 1979 2018) ; => 297.5844637544411
```

To estimate how much it costs to compensate for (your) life so far
```clj
(* (co2-over-life-in-finland 1979 2018) 12.87)) => 3829.9120485196568
```

## License

The code is released to the Public Domain. Use it for much good!

The data included, is covered by their respective licenses detailed below.

## CO2 emissions by age
- [The leverage of demographic dynamics on carbon dioxide emissions: does age structure matter?](https://www.demogr.mpg.de/en/projects_publications/publications_1904/journal_articles/the_leverage_of_demographic_dynamics_on_carbon_dioxide_emissions_does_age_structure_matter_4131.htm)
- Zagheni, E.
- Demography, 48:1, 371-399 (2011)
- DOI:10.1007/s13524-010-0004-1
- See also [CO2 Age Structure](https://www.mpg.de/4635546/CO2_age_structure)
- Distributed under the terms of the Creative Commons Attribution Noncommercial License which permits any noncommercial use, distribution, and reproduction in any medium, provided the original author(s) and source are credited.

## CO2 emissions (metric tons per capita)
- [The World Bank](https://databank.worldbank.org/data/source/world-development-indicators)
- EN.ATM.CO2E.PC
- Carbon dioxide emissions are those stemming from the burning of fossil fuels and the manufacture of cement. They include carbon dioxide produced during consumption of solid, liquid, and gas fuels and gas flaring.
- Carbon Dioxide Information Analysis Center, Environmental Sciences Division, Oak Ridge National Laboratory, Tennessee, United States.
- Licensed CC BY-4.0
