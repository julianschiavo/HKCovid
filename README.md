# Covid in HK
Full case details for reported Covid-19 cases in Hong Kong, shared by the Communicable Diseases Branch of the Center for Health Protection (CHP) of the Department of Health (DH).

## [Statistics](STATISTICS.md)

**[Data](#data)**

**[Structure](#structure)**

**[Dates & Upcoming Data](#timeframes)**

<br>

## Data

- `daily/YYYY-MM-DD.csv`: Full Case Details for DD/MM/YYYY
- `all.csv`: All Full Case Details from 01/01/2022 to Last Report Date

<br>

## Structure

Each `csv` file contains the following information:
| Column             	| Description                                               	| Format                                                                                                                                                              	|
|--------------------	|-----------------------------------------------------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Case #             	| The case number.                                          	| Number                                                                                                                                                              	|
| Report Date        	| The date the case was reported.                           	| Date (`D/M/YYYY`)                                                                                                                                                   	|
| Classification     	| The most recently known case classification.              	| `Local`/`Local-Linked`/`Imported`/`Import-Related`, or empty if Pending/Unknown                                                                                     	|
| Status             	| The most recently known case status.                      	| `Confirmed`/`Asymptomatic`/`Pending`/`Re-Positive`, or empty if Unknown                                                                                             	|
| Gender             	| The gender of the case.                                   	| `M`/`F`, or empty if Unknown                                                                                                                                        	|
| Age                	| The age of the case.                                      	| Number (or `<Number> months`), or empty if Unknown                                                                                                                  	|
| Symptom Onset Date 	| For symptomatic cases, the date of onset of symptoms.     	| Date (`D/M/YYYY`), or empty if Unknown/Pending/Asymptomatic.                                                                                                        	|
| Vaccination Status 	| Whether the case is vaccinated.                           	| `Full` if vaccinated with two doses, `Some` if vaccinated with at least one dose, `None` if unvaccinated or vaccinated with a single dose, or `Pending` if pending. 	|
| Residence          	| The case's last-known residence prior to confirmation.    	| Text, or `Pending` if pending.                                                                                                                                      	|
| Travel History     	| Recent travel history of the case.                        	| Text (`Place/Place2`), `None` if no recorded travel history, or `Unknown` if unknown.                                                                               	|
| HK Resident        	| Whether the case was a Hong Kong resident or a foreigner. 	| `Y`/`N`, or `Pending` if pending.                                                                                                                                   	|

A few points to note:
- Dates in the files are _not_ zero-padded (`7/2/2022`, not `07/02/2022`)
- All data is subject to changes according to epidemiological investigations

<br>

## Timeframes

### Last Report Date: 11/02/2022

This is the date of the most recently reported cases for which information is available, which tends to be up to 21 days following the reporting date of the case. Case information for previous days is not typically updated.

### Upcoming Data

| Request Date 	| Expected Date 	| Case Dates                                                             	|
|--------------	|---------------	|------------------------------------------------------------------------	|
| 17/02/2022   	| 09/03/2022    	| 12/02/2022, 13/02/2022, 14/02/2022, 15/02/2022, 16/02/2022, 17/02/2022 	|
| 18/02/2022   	| 10/03/2022    	| 18/02/2022                                                             	|
| 19/02/2022   	| 11/03/2022    	| 19/02/2022                                                             	|
| 20/02/2022   	| 11/03/2022    	| 20/02/2022                                                             	|
| 22/02/2022   	| 14/03/2022    	| 21/02/2022, 22/02/2022                                                 	|
| 24/02/2022   	| ~16/03/2022   	| 23/02/2022, 24/02/2022                                                 	|
| 25/02/2022   	| ~17/03/2022   	| 25/02/2022                                                             	|
| 28/02/2022   	| ~20/03/2022   	| 26/02/2022, 27/02/2022, 28/02/2022                                     	|
| 01/03/2022   	| ~21/03/2022   	| 01/03/2022                                                            	|

<br>

## Disclaimer

This data was provided by the Hong Kong Special Administrative Region (HKSAR) of the People's Republic of China, and all relevant laws apply. This data is not owned or created by the creator of this repository, and the repository holds no rights over it.

**THE INFORMATION OR MATERIAL PROVIDED IS FOR REFERENCE ONLY. WHILST WE ENDEAVOUR TO ENSURE THAT THE INFORMATION OR MATERIAL IS ACCURATE, NO EXPRESS OR IMPLIED WARRANTY IS GIVEN BY US AS TO ITS ACCURACY AND WE SHALL NOT BE HELD RESPONSIBLE FOR ANY ERROR OR OMISSION.**

**WE SHALL NOT BE LIABLE FOR ANY DAMAGES (INCLUDING BUT NOT LIMITED TO DAMAGES FOR LOSS OF BUSINESS OR LOSS OF PROFITS) ARISING IN CONTRACT, TORT OR OTHERWISE FROM (I) THE USE OF OR INABILITY TO USE THIS DATA, OR (II) FROM ANY ACTION TAKEN OR DECISION MADE ON THE BASIS OF THIS DATA.**
