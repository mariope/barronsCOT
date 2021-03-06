# barronsCOT v0.1.0

[![Build Status](https://travis-ci.org/mariope/barronsCOT.png?branch=master)](https://travis-ci.org/mariope/barronsCOT)

Retrieve and analyze Barron's Commitments of Trader data.

## Getting Started

Barron's commitments of traders (COT) is a weekly data seed from Barron's web page
[Barron's COT ](http://www.barrons.com/public/page/9_0210-traderscommitments.html)

**barronsCOT** package reads the COT table from Barron's web page, store the data and plot graphics to analyze it.

- Retrieve COT weekly data
- Clean and store data
- Show several graphics representation

### Prerequisities

If you install from devtools you do not need to do anything else.

```
> devtools::install_github("mariope/barronsCOT")
```

#### Loading the library

When you load the library, you obtain three data frames: 

- **COTsp** for S&P 500 COT

- **COTspm** for S&P 500 (E-mini) COT

- **COTgold** for Gold COT.

```
library(barronsCOT)
```

## Running barronsCOT

The functions available are:

### getBarronsCOT()

Retrieve COT weekly data fron Barron's web page.
This function hasn't parameters.

```
> getBarronsCOT()
```
The output is a text saying if the data frames have been updated like this:

```
# [1] "Values added with date:  February 14, 2017"
```

or

```
# [1] "February 14, 2017 Values are already embedded"
```

### plotCOT()

Show several graphics representation.
This function need a COT data frame. Default COTsp.

```
> plotCOT(COTsp)
> plotCOT(COTspm)
> plotCOT(COTgold)
```

## Built With

* R v3.2.2
* R Studio - version 0.99.903

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

I use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/mariope/barronsCOT/tags). 

## Authors

* **Mario Pisa** - *Initial work* - [barronsCOT](https://github.com/mariope/barronsCOT)

## License

This project is licensed under the GPL-3 License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* To Open Source community.
