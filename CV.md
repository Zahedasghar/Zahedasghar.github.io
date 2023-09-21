---
name: Zahid
surname: Asghar
position: " Professor of Economics"
address: "School of Economics, Quaid-i-Azam University, Islamabad"
# profilepic: "img/zahid.jpg"
# phone: +1 301 696 3368
www: zahidasghar.com
email: "zasghar@qau.edu.pk"
twitter: zahedasghar
github: zahedasghar
# linkedin: zahid-asghar
# googlescholar: ObUvhnsAAAAJ&hl
# orcid: 0000-0002-6177-9308
# extrainfo: "testing extra info"
# quote: "testing a quote"
headcolor: e64173 #009ACD
#urlcolor: e64173
date: "`r format(Sys.time(), '%B %Y')`"
docname: CV
# about me: "Testing About Me"
output: vitae::awesomecv
always_allow_html: yes
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = FALSE, warning = FALSE, message = FALSE)
library(vitae)
library(fontawesome)
library(tidyverse)
```

# \faBriefcase \acvHeaderIconSep Appointments

```{r}
tribble(
  ~ title, ~ year, ~ institution, ~ where,
  #"Quaid-i-Azam University", "2018—", "Professor of Economics", "Frederick, MD", "Assistant Professor of Economics",
  #"Hood College", "2016—2019", "Visiting Assistant Professor of Economics", "Frederick, MD", "Visiting Assistant Professor of Economics",
  #"Hood College", "2016—", "Assistant Professor of Economics", "Frederick, MD", "2019—",
  #"Hood College", "2016—", "Visiting Assistant Professor of Economics", "Frederick, MD", "2016—2019",
  "Professor of Economics", "2018—Present", "School of Economics", "Quaid-i-Azam University, Islamabad",
  "Associate Professor of Statistics ", "2015—2018", "Department of Statistics", "Quaid-i-Azam University, Islamabad",
  "Subject Specialist Econometrics", "2011—2013", "National Institute of Banking and Finance, State Bank of Pakistan", "NIBAF,Islamabad",
  "Consultant ", "2009-10", "Sultan Qaboos University", "Muscat, Oman",
  "Director", "2019—2022", "School of Economics", "QAU,Islamabad",
  "Registrar", "2020-2021", "Quaid-i-Azam University", "Islamabad"
) %>% 
  detailed_entries(with = title,
                   what = institution,
                   #why = detail,
                   when = year,
                   where = where)
```


# \faGraduationCap \acvHeaderIconSep  Education

```{r}
tribble(
  ~ Degree, ~ Year, ~ Institution, ~ Where,
  "Ph.D — Economics", "2007", "Pakistan Institute of Development Economics", "Islamabad",
  "MSc — Statistics", "1993", "Bahauddin Zakaraya University", "Multan, Punjab",
  "BSc - Math,Stat", "1990", "University of the Punjab", "Lahore, Punjab"
) %>% 
  detailed_entries(Degree, Year, Institution, Where)
```

# \faFlask \acvHeaderIconSep Research

## \faExclamationTriangle \acvHeaderIconSep Interests

Applied Economics, Development Economics, Official Statistics, Economy of cities, Econometrics and Data Analytics, 

\medskip

## \faFile \acvHeaderIconSep Peer-Reviewed Journal Articles (more than 40)

```{r}
bibliography_entries("publications.bib") %>%
  arrange(desc(issued))
```

\bigskip


```{r, eval=FALSE}
bibliography_entries("underreview.bib") %>%
  arrange(desc(author$family), issued)
```

\bigskip 


```{r, eval=FALSE}
## \faSpinner \acvHeaderIconSep Works in Progress ( to get like rayan safner, eliminate chunk start and end )

bibliography_entries("workingpapers.bib") %>%
  arrange(desc(author$family), issued)
```

# \faUniversity \acvHeaderIconSep Teaching

## About me
I am applied econometrician and statistician with special interests in development economics, making sense of data through Data visualization and  have conducted a large number of trainings on data analytics using Excel, STATA, R and EVIEWS. I have expertise in using R , STATA and Excel , and comfortable in using Datawrapper, Tableau, SPSS and EVIEWS for data anlysis. I am actively engaged in playing with data particularly _PovCalnetR_, _PDHS_, _PSLM_, _WDI using R_ among many other survey data sets. I have published in gender, food security and other socio-economic issues both in national and international peer reviewed journals. I am keen in having better awareness of development indicators in the society and to contribute to an evidence based decision making in socio-economic policy. I have strengths both in Statistics and Economics

I have taught a wide variety of courses. At School of Economics, I regularly teach econometrics (every semester), Economy of Pakistan, and Urban Economics (1-2 each semester) , Applied Economics and Inferential Statistics. 

```{r, eval=FALSE}
## Hood College
#without chunk it can be displayed
- ECMG 212 — Statistics for Economics & Management (S2017)
- ECON 205 — Principles of Macroeconomics (F2018)
- ECON 304 — International Political Economy (F2017) 
- ECON 306 — Microeconomic Analysis (F2016; S2017; F2017; S2018; F2018; S2019; F2019; S2020; F2020; S2021;  [F2021](https://microf21.classes.ryansafner.com))
- ECON 315 — Economics of the Law ([S2021](https://laws21.classes.ryansafner.com)) [**Developed course**]
- ECON 316 — Game Theory (S2019; [F2021](https://gamef21.classes.ryansafner.com))
- ECON 317 — Economics of Development (F0291; [F2021](https://devf21.classes.ryansafner.com))
- ECON 324 — International Trade (F2016; F2018; [F2020](https://tradef20.classes.ryansafner.com))
- ECON 326 — Industrial Organization (S2017; [S2020](https://ios20.classes.ryansafner.com))
- ECON 410 — Public Economics (S2018; [S2020](https://publics20.classes.ryansafner.com))
- ECON 452 — History of Economic Thought ([F2020](https://thoughtf20.classes.ryansafner.com))
- ECON 480 — Econometrics (F2016; F2017; F2018; F2019; F2020; [F2021](https://metricsf21.classes.ryansafner.com))
- MGMT 399 — Internship for Business (S2018)

## Wake Forest University

- ECN 150 — Introduction to Economics (Fall 2015; Spring 2016)
- ECN 271 — Special Topics: Austrian Economics (Spring 2016)

## George Mason University

- ECON 385 —  International Economic Policy (Summer 2013, Fall 2013, Spring 2014)
- ECON 403 — Austrian Economics (Summer 2015)
- ICES — High School Economics Workshops (Summer 2012, cotaught with Paul Mueller)
```

# Professional Engagements

-    Senate Member, Pakistan Institute of Development Economics 2008-2011 
 
 -    Member Research Advisory Council on ‘Research for Social 
  Transformation and Advancement’ (RASTA) under PSDP of the Ministry 
  of Planning, Development and Special Initiatives, the Government of
  Pakistan, 2020-21 to-date 
 -    Member Technical Committee Price Indices , Pakistan Bureau of 
  Statistics 2013 to-date 
  
 -    LEAD fellow Cohort-19  
  
 -    Member Technical Committee SDGs , Pakistan Bureau of Statistics 
  
 -    Member Technical National Account Committee, Pakistan Bureau of
  Statistics 
  
 -    Member, Board of Studies and Faculty at various academic institutions 
 - Editor (Pakistan Economic Review) and member of editorial boards and a reviewer



# \faBriefcase \acvHeaderIconSep Research Projects and Consultancy

-  *Workshop on Applied Economics with R*, Pakistan Institute of Development Economics, Spring Semester 2023 
-  *R for data analytics* Online course 5 weeks Feb-Mar:2023

-	Data Analysis of Tax on Services Sector 2012-2022 of Punjab 
	
-	Data Analyst for Earning Projection Survey of Free-Lancing jobs
	under IGNITE, Ministry of Finance 2021, Pakistan   
	
-	Data consultant for Ignite: National Technology Fund, Ministry of
	Finance 2019-20 
	
-	Assessing Data requirements for SDGs through key informant
	interviews and surveys in progress under NRPU of the HEC (Current)
-	Data were extracted from PSLM and HIES from 1998-2015-16 Surveys 
	
-	Member of the team as a data analyst for a research project for
	financing agriculturists through a third party instead of  Arhtis
	at NIBAF, State Bank of Pakistan 2011-13 
	
-	Consultant for a project on Biases in Consumer Price Index (PIDE)
	2007 
	
# \faComments \acvHeaderIconSep Trainings
 -    *Revenue Forecasting for KP Revenue Authority* , 26-30 September, 2022 USAID/SDPI
 -    *Econometrics Using STATA Under TVET Support Program in Pakistan*, 2-13 March, 2015
 -    *Applied Econometrics, NIBAF, State Bank of Pakistan* 14-18 December, 2017, Islamabad 
 -    **Data Management and Analysis Using STATA**, _International Rescue Committee_, 25-27 April, 2017 Islamabad 

 -    Workshop conducted for Mid-Career Management Course on “Data
	Visualization” Information Services Academy, Islamabad, December,
	2020 
	
 -    Resource Person for  ‘Data Visualization and its importance for
	Journalists and media’, Information Services Academy, Islamabad, 
	3rd January, 2020 
	
 -    Resource Person for Workshop on Applied Economics Using Softwares, School of
	Economics, QAU, 22-26 July,2019

 -    Resource Person for Workshop on Analysing Data Using Stata, Pakistan Institute of     Development Economics, Islamabad, 5-February,2019 
 -    Data Visualization for Policy Making Using Excel for Faculty Development Program,
	HEC, 2-Sessions, 20th January,2019 
 -    Resource Person for Workshop on Applied Econometrics, School of Economics, QAU, 
	4-6 Jan,2019 
 -    National Invited Speaker for “ Making Sense of Data Through Visualization,
	University of Malakand, Nov-2018 
 -    National Invited Speaker for “Data Visualization”, Women University, Multan
	11-May, 2018 
 -    Data, Data Visualization, and Data Driven Decision Making for Faculty Development
 -    Program, HEC, 2-Sessions, 20th January,2017 
 -    Teaching Basic Statistics for Teachers Workshop at PIDE (Conducted 2 Sessions on
 -    Data Visualization and Exploration August, 2016) 
 -    MS Excel-Advanced Young Professional Induction Program Batch 5, NIBAF, State Bank 
	of Pakistan (20-22 June, 2016) 
 -    Visualization and Exploration of Data Using R for PIDE research staff and students
	(8-9 May, 2016).
	*Business Intelligence through Financial Modeling-Scenario-Building* for Senior
 -    Middle Management of SBP-BSC, NIBAF, Islamabad (4 hours), 2016 (2nd Iteration).
	*Business Intelligence through Financial Modeling-Scenario-Building* for Senior
 -    Middle Management of SBP-BSC, NIBAF, Islamabad (4 hours), 2016 
	
 -    *Use of Statistical Package for Social Sciences (SPSS) In Agricultural Statistics of Pakistan* Ministry of Food Security and Research, PARC, Islamabad Feb.24,2016 
	
 -    *MS Excel Advanced for SBP-BSC officers* at NIBAF Islamabad (Feb.22-23, 2016) 
	
 -    *Statistical Methods Using STATA* for Strengthening of Crops Estimation System in Pakistan by Capacity Building of the Officers.  Ministry of Food Security and
  Research, Islamabad, October 20,2015 
  
 -    *Applied Research Methods for Economics & Finance*, Department of Economics and
	Finance, PIDE, Islamabad September 7-11,2015 
	
 -    *Processing and Analysis of Data (Methodology and Software)* June10-12, 2015 
	*MS Office-Advanced (Excel, Word & PowerPoint) Young Professional Induction Program*. NIBAF, State Bank of Pakistan (22-25 April, 2015) 
	
 -    *Inflation, Measurement Issues and its Impact on Common Man* for Research Officers (Economist Group) M/O Planning, Development and Reform at PPMI, Islamabad (22 Oct, 2014) 
 -    *Data Analysis Using Excel-Advanced for Research Staff and Faculty*, Pakistan
	Institute of Development Economics, Islamabad (9-10 June, 2014)
 -    *Advanced Applied Econometrics Using STATA/ EVIEWS* for State Bank of Pakistan
 Officers at LRC, Karachi (24 June-5 July 2013)
 -    *Issues in Pakistan Economy*, State Bank Officers Training, NIBAF, 6th July, 2013 Islamabad
 -    *Advanced Econometrics Using STATA and EVIEWS* for State Bank of Pakistan Officers (Research, Statistics and Data Ware House wing) at LRC, Karachi (Feb-Mar 2013)
 -    *Applied Econometrics* for State Bank of Pakistan officers (Monetary and Economic Policy Division) at LRC, Karachi (2012)
 -    *Managerial Economics: International Business Administration & IT Course for Central Asian Republics* NIBAF, State Bank of Pakistan, (2012)
 -    *National Accounts*, State Bank Officers Training Scheme (2012)
	*Biostatistics and Genetic Epidemiology*, Quaid-i-Azam University, Islamabad. Served as Focal Person from Aug 02-11 (2016).
 -    *Two weeks training course on Statistics*, Planning Commission of Pakistan, Pakistan (2005)
 -    *Resource Person for Higher Education Commission Faculty Development Program* 2017 to-date


##  PhD thesis 

  Supervised: 5 
  
  Under-progress: 3

  Mphil thesis (Supervised): 40 + 

    

## References: 

  Upon request 
  
# \faCogs \acvHeaderIconSep Skills

```{r, results = "asis", eval = F}
library(fontawesome)
stars<-as.character(fontawesome::fa("star"))
tribble(
  ~"", ~"",
  "R", stars,
  "Stata", stars
) %>%
  knitr::kable(booktabs = T, align = 'lr', escape = F, format = "latex")
```

- **Languages**:
  - English \faStar \faStar \faStar 
  - Urdu \faStar \faStar \faStar \faStarO
  - Punjabi \faStar \faStar \faStar \faStarO
- **Software**:
  - R :     \faStar \faStar \faStar  \faStarHalfEmpty
  - Stata:  \faStar \faStar  \faStar          \faStarHalfEmpty
  - EVIEW:  \faStar \faStar
  - MsExcel:\faStar \faStar