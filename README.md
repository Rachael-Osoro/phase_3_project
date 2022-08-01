# Are you Vaccinated?
# A PREDICTIVE MODEL OF VACCINATION AGAINST H1N1 INFLUENZA VARIANT.

![](https://github.com/Rachael-Osoro/git_practice/blob/master/Photos/vax.jpg)

## Repo Structure

<a href="https://github.com/Rachael-Osoro/phase_3_project/tree/main/H1N1_data">Dataset</a>

<a href="https://github.com/Rachael-Osoro/phase_3_project/blob/main/H1N1_analysis.ipynb">EDA ipynb</a>

<a href="https://github.com/Rachael-Osoro/phase_3_project/blob/main/models.ipynb">Modelling ipynb</a>

<a href="https://github.com/Rachael-Osoro/phase_3_project/blob/main/H1N1_Analysis_Presentation.pdf">Presentation<a/>
  
<a href="https://github.com/Rachael-Osoro/phase_3_project/blob/main/README.md">Readme Markdown<a/>

## Overview

Vaccines reduce risks of getting a disease by working with your body’s natural defences (immunity) to build protection. Vaccines are also critical in the prevention and control of infectious disease outbreaks such as  <a href = "https://en.wikipedia.org/wiki/Influenza"> Influenza</a>, <a href = "https://en.wikipedia.org/wiki/COVID-19"> COVID-19</a>, etc. In addition, vaccines can provide enough immunization in a community further reducing spread of diseases through “herd immunity”. Eventually leading to disease eradication/ elimination for instance Small Pox. 

![](https://github.com/Rachael-Osoro/git_practice/blob/master/Photos/health-influenza-taxonomy-virus-cell-illustration.jpg)

One of the commonest infection worldwide is the influenza virus aka ‘flu’ which attacks the human respiratory tract, causing symptoms such as fever, headaches, fatigue, coughing, sore throat, nasal congestion, and body aches. It is a seasonal diasease with high incidence in the colder months. According to <a href = "https://www.wiscontext.org/understanding-perennial-menace-influenza-virus"> this report by Samantha Nash </a>, about 8.3% of USA population get influenza annually. During the 2017-18 flu season, the use of the influenza vaccine is estimated to have prevented 5,700 deaths and 91,000 hospitalizations in the U.S. 
A variant of the influenza virus, H1N1, famously known as swine flu caused a pandemic that led to 61 million clinical cases of influenza, 274,000 hospitalizations and 12,500 deaths. A vaccine for the H1N1 flu virus became publicly available in October 2009 which prevented 700,000–1,500,000 clinical cases, 4,000–10,000 hospitalizations, and 200–500 deaths. <a href = "https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3647645/">according to this study </a>.

## Problem Statement

There seems to be an overall hesitancy in vaccine uptake which is major threat to reduction of vaccine preventable diseases. Reasons for hesitancy vary from safety and effectiveness of vaccines, mistrust, socio-economic characteristics, vaccine development, perceived risk of disease, lack of information about vaccine, personal beliefs, perceived benefit etc. To assess seasonal flu and H1N1 vaccine uptake, in late 2009 and early 2010, the United States conducted the National 2009 H1N1 Flu Survey. This phone survey asked respondents whether they had received the H1N1 and seasonal flu vaccines, in conjunction with questions about themselves. The questions covered their social, economic, and demographic background, opinions on risks of illness and vaccine effectiveness, and behaviors towards mitigating transmission. A better understanding of how these characteristics are associated with personal vaccination patterns can provide guidance for future public health efforts. 


## Project Goal
Immunization is a global health and development success story, saving lives every year. Vaccines reduce disease spread, therefore, maximizing immunization coverage for any population is a crucial public health goal for all countries.
The aim of this project is to predict the vaccination status of person based on their response to survey questions. The results will be utilized by public health departments to ramp up campaigns, mass vaccination, conduct health education on those assigned unvaccinated in order to promote vaccination against influenza. The model can be utilized in subsequent pandemics.

## Data & Methods
Each row in the dataset represents one person who responded to the National 2009 H1N1 Flu Survey and there are two target variables. Data is valid, obtained from 
<a href = "https://www.cdc.gov/nchs/index.htm"> National Centre for Health Statistics</a>.

### EDA
There seems to be low uptake of H1N1 vaccine with on about 21% of the respondents being vaccinated. Illustrated in the bar graph below: <a href="https://github.com/Rachael-Osoro/phase_3_project/blob/main/H1N1_analysis.ipynb">more viz and EDA here</a>

![](https://github.com/Rachael-Osoro/git_practice/blob/master/Photos/h1n1.png)
### Final Model
After iterating through logistic regression, decision trees, random forests, XGBoost model and gradient boosting classifiers, tuned Random forests classifier with accuracy of 83.3% and precision 71.6% is the final model.
83.3% of respondents will be predicted into the right class.
#### Confusion Matrix
The model predicts 76% as True negatives, 7.5% True positives, 3% false positives and 14% false negatives.

![](https://github.com/Rachael-Osoro/git_practice/blob/master/Photos/conf_matrix.png)
#### Feature Importance
The major features affecting vaccine uptake:

![](https://github.com/Rachael-Osoro/git_practice/blob/master/Photos/imp_feat.png)

## Recommendations

1.) Model is able to predict of unvaccinated people. The CDC can reach them through text, email etc to nudge the need for vaccination.

2.) Encourage doctors to recommend vaccinations to the general public.

3.) Dispell misinformation about the vaccine, by providing adequate information about vaccine effectiveness.

4.) Educating the public on risk factors of the H1N1, it's spread and preventive measures so that the public has factual reliable information.

# Limitations
Data is not recent hence model may not depict current H1N1 vaccine uptake.
# Dependencies
Anaconda + XGBoost or
Python,
sklearn,
matplotlib &, 
XGBoost.

