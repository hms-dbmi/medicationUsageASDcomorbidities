# medicationUsageASDcomorbidities
Jupyter Notebooks for conducting analysis on medication usage in the treatment of co-occurring conditions in Autism Spectrum Disorder on a claims database.

## Prerequisites
The following libraries must be installed:
```bash
library("devtools")
library("SqlServerJtds")
library("SqlTools")
library("FactToCube")
library("ggplot2")
library("plotly")
library("ggalluvial")
library("stringr")
library("UpSetR")
library("RColorBrewer")
library("networkD3")
library("webshot)
```

## Authorizations
- To have access to the claims database, approval is required. 

## How to
The jupyter notebook 1.ASDcohortSelection comprises all the code used for obtain our sample cohort of patients diagnosed with ASD. It comprises the SQL code queries. 

The jupyter notebook 2.ASDcohortDemographics comprises all the SQL code to describe the demographics of the ASD cohort selection in terms of gender distribution, age at first diagnosis, and regional distribution across the U.S.

The jupyter notebook 3.DrugFrequencyAuthomatic comprises the SQL and R code to evaluate each of the target study drugs in the ASD cohort, and the analysis and visualization of the drug use overtime through Sankey and UpSetR diagrams.

The jupyter notebook 4.ComorbidityAnalysisByMedicationAuthomatic.ipynb comprises all the SQL code required to estimate the number of patients having each comorbidity in each of the medication groups, considering a medication group all the patients taking only that specific drug. It also contains the R code for the posterior representation in a heatmap plot.

## Publication
This code supports the analysis presented in: "Medication Use in the Management of Comorbidities among Individuals with Autism Spectrum Disorder from a Large Nationwide Insurance Database (2014 – 2019)" https://jamanetwork.com/journals/jamapediatrics/fullarticle/2780352 

### Citation: 
Feroe, A.G., Uppal, N., Gutiérrez-Sacristán, A., Mousavi, S., Greenspun, P., Surati, R., Kohane, I.S. and Avillach, P., 2021. Medication use in the management of comorbidities among individuals with autism spectrum disorder from a large nationwide insurance database. JAMA pediatrics, 175(9), pp.957-965.

## License
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
