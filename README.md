# 2020_cournot_producer
Power systems data (2018-2019) from ENTSO-e and OMIE (Spain) used in the numerical case study of the [paper] published on IEEE Transactions on Power Systems. The data includes wind and solar power production forecasts of Spain (ES bidding zone) and inverse demand function data obtained from spanish marked data of OMIE.

## Dataset Content 
This section describes in detail the data series of the only data file in the repository: dataset_wind_europe_2015_2019.csv

### Time

TimeUTC: UTC time

hour of day (hourXX): dummy variable equal 1 when TimeUTC.hour == hourXX (24 series).

### Data from OMIE

Data source: [OMIE] 

alpha: (euros).

beta: (euros).

### Data from Entsoe

Data source: [ENTSO-e Transparency Platform]

Warning! The day ahead data may not follow the Manual of Procedure of the Transparency Platform and may be uploaded after the 18.00 Brussels time deadline of day D-1. The data is sometimes updated afterwards, even months later.

XX_won_real: (MWh) actual onshore wind production of bidding zone XX. 

XX_won_da: (MWh) day ahead (before 18.00 Brussels time day D-1) onshore wind production of bidding zone XX. 

XX_woff_real: (MWh) actual offshore wind production of bidding zone XX.

XX_woff_da: (MWh) day ahead (before 18.00 Brussels time day D-1) offshore wind production of bidding zone XX.

DK1_SchedGen: (MWh) Scheduled generation for DK1. 

DK1_SolarDahead: (MWh) Solar production forecasted for DK1. (before 18.00 Brussels time day D-1)

DK1_TotalLoadDahead: (MWh) Total Load forecasted for DK1. (before 18.00 Brussels time day D-1)

### Other data

DK1_FM3_output: (MWh) Output of the first step optimization problem tailored to forecasting as described in the [paper].

## Useful related websites

[OMIE]

[ENTSO-e Transparency Platform]



## How to cite the paper?

If you want to cite this [paper] you can use the following text:
```
Pending.
```
or the .bib version:

```
Pending
```

## Developed by 

 * [Miguel Angel Muñoz Diaz](https://www.researchgate.net/profile/Miguel_Munoz_Diaz) - miguelangeljmd@uma.es
 * [Juan Miguel Morales](https://www.researchgate.net/profile/Juan_Morales25) - juan.morales@uma.es
 * [Salvador Pineda](https://www.researchgate.net/profile/Salvador_Pineda) - spinedamorente@gmail.com
 * [OASYS group](http://oasys.uma.es) -  groupoasys@gmail.com

## Do you want to contribute?
 
Any feedback is welcome so feel free to ask or comment anything you want via a Pull Request in this repo.
 
## License
 
Please, see the LICENSE file.
    
[paper]: Pending
[Energinet]: https://www.omie.es/
[ENTSO-e Transparency Platform]: https://transparency.entsoe.eu/
