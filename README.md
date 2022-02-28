# Covid in HK
Full case details for reported Covid-19 cases in Hong Kong, shared by the Communicable Diseases Branch of the Center for Health Protection (CHP) of the Department of Health (DH).

## Data

- `daily/YYYY-MM-DD.csv`: Full Case Details for DD/MM/YYYY
- `all.csv`: All Full Case Details from 07/02/2022 to Last Report Date

## Structure

Each `csv` file contains the following information:
| Column      	| Case #           	| Report Date                     	| Gender                  	| Age                         	| Status                               	| Symptom Onset Date                                      	| Residence                                              	| Travel History                                                  	| Classification                               	| Full Vaccination Status                                                                                          	| HK Resident                                               	|
|-------------	|------------------	|---------------------------------	|-------------------------	|-----------------------------	|--------------------------------------	|---------------------------------------------------------	|--------------------------------------------------------	|-----------------------------------------------------------------	|----------------------------------------------	|------------------------------------------------------------------------------------------------------------------	|-----------------------------------------------------------	|
| Description 	| The case number. 	| The date the case was reported. 	| The gender of the case. 	| The age of the case.        	| The most recently known case status. 	| For symptomatic cases, the date of onset of symptoms.   	| The case's last-known residence prior to confirmation. 	| Recent travel history of the case.                              	| The most recently known case classification. 	| Whether the case was fully vaccinated.                                                                           	| Whether the case was a Hong Kong resident or a foreigner. 	|
| Format      	| Number           	| Date (`D/M/YYYY`)               	| `M`/`F`                 	| Number, or empty if Pending 	| `Confirmed`/`Asymptomatic`/`Pending` 	| Date (`D/M/YYYY`), or empty if pending or asymptomatic. 	| Text, or `Pending` if pending.                         	| Text (`Place/Place2`), or `None` if no recorded travel history. 	| `Local`/`Imported`                           	| `Y` if vaccinated with two doses, `N` if unvaccinated or vaccinated with a single dose, or `Pending` if pending. 	| `Y`/`N`, or `Pending` if pending.                         	|

A few points to note:
- Dates in the files are _not_ zero-padded (`7/2/2022`, not `07/02/2022`)
- All data is subject to changes according to epidemiological investigations

## Disclaimer

This data was provided by the Hong Kong Special Administrative Region (HKSAR) of the People's Republic of China, and all relevant laws apply. This data is not owned or created by the creator of this repository, and the repository holds no rights over it.

**THE INFORMATION OR MATERIAL PROVIDED IS FOR REFERENCE ONLY. WHILST WE ENDEAVOUR TO ENSURE THAT THE INFORMATION OR MATERIAL IS ACCURATE, NO EXPRESS OR IMPLIED WARRANTY IS GIVEN BY US AS TO ITS ACCURACY AND WE SHALL NOT BE HELD RESPONSIBLE FOR ANY ERROR OR OMISSION.**

**WE SHALL NOT BE LIABLE FOR ANY DAMAGES (INCLUDING BUT NOT LIMITED TO DAMAGES FOR LOSS OF BUSINESS OR LOSS OF PROFITS) ARISING IN CONTRACT, TORT OR OTHERWISE FROM (I) THE USE OF OR INABILITY TO USE THIS DATA, OR (II) FROM ANY ACTION TAKEN OR DECISION MADE ON THE BASIS OF THIS DATA.**
