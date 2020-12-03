# 2020_cournot_producer
Power systems data (2018-2019) from ENTSO-e and OMIE (Spain) used in the numerical case study of the [manuscript] currently under review. The dataset includes wind and solar power production forecasts of Spain (ES european bidding zone) and inverse demand function parameters computed from real data of the spanish day ahead market OMIE. The parameters alpha and beta are computed assuming a linear invese demand function. More details in the [manuscript].

## Dataset Content 
This section describes in more detail the data series of the only data file in the repository: dataset_spain_2018_2019.csv

### Time

timestamp: UTC timestamp.

hour: series with value equal to the hour of the day.

### Processed series from OMIE data

Raw data source: [OMIE] 

In the case study we assume a Cournot producer whose production influence the price she obtains. A linear inverse demand function of the form price = alpha - beta * energy_production is assumed. The parameter of this model are considered unknown prior to the market bid. For each hour of the training dataset a different linear model is fit to obtain the corresponding parameters for that hour.

alpha: constant term of the linear model (euros).

beta: slope of the intverse demand function (euros / MWh).

### Forecasts from ENTSO-e

Data source: [ENTSO-e Transparency Platform]

The forecasts below are issued before 18.00 Brussels time day D-1 according to the Manual of Procedure of the [ENTSO-e Transparency Platform].

wind_on_dahead_utc: (MWh) On shore wind production forecast for the european bidding zone ES. 

solar_dahead_utc: (MWh) Solar production forecast for the european bidding zone ES.


## Useful related websites

[OMIE]

[ENTSO-e Transparency Platform]


## How to cite the paper?

If you want to cite this [paper] you can use the following text:
```
M.A. Muñoz, S. Pineda, J.M. Morales, "A bilevel framework for decision-making under uncertainty with contextual information," arXiv preprint arXiv:2008.01500, 2020.
```
or the .bib version:

```
@misc{Munoz2020bilevel,
      title={A bilevel framework for decision-making under uncertainty with contextual information}, 
      author={M.A. Mu\~noz and S. Pineda and J.M. Morales},
      year={2020},
      eprint={2008.01500},
      archivePrefix={arXiv},
      primaryClass={math.OC}
}
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
    
[paper]: https://arxiv.org/abs/2008.01500
[manuscript]: https://arxiv.org/abs/2008.01500
[OMIE]: https://www.omie.es/
[ENTSO-e Transparency Platform]: https://transparency.entsoe.eu/
