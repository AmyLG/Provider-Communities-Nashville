# Provider-Communities-Nashville
Driving into Nashville's complex healthcare referral system based of 2017 Medicare data

### Team
Team lead: Courtney Everest (ce initials for notebooks) <br />
Alexa Zylstra (az initials for notebooks) <br />
Armelle Le Guelte (alg initials for notebooks)
And the entire Data Science Bootcamp Cohort 4

### Duration
2 weeks

### Project overview
This project leverages the 2017 Hop Teaming dataset of Medicare referral claims to examine how Medicare patients move through the middle Tennessee healthcare system. By looking at referrals from individual healthcare providers to Nashville general acute care hospitals, we explore the communities of healthcare specialists that practice in the middle Tennessee area and offer insights into their Medicare patient referral practices.

### Data
* The 2017 Hop Teaming dataset can be acquired for no charge from https://careset.com/datasets-3/
* The NPPES Data Dissemination from https://download.cms.gov/nppes/NPI_Files.html
* The taxonomy code to classification crosswalk from the National Uniform Claim Committee: https://www.nucc.org/index.php/code-sets-mainmenu-41/provider-taxonomy-mainmenu-40/csv-mainmenu-57
* The Zip code to CBSA crosswalk from here: https://www.huduser.gov/portal/datasets/usps_crosswalk.html

### Objectives
* To build a profile of providers referring patients to the major hospitals in Nashville. Are certain specialties more likely to refer to a particular hospital over the others?
* To determine which professionals Vanderbilt Hospital should reach out to in the Nashville area to expand their own patient volume.
* To look for "communities" of providers in the Nashville/Davidson County CBSA. We used the Louvain community detection algorithm from Neo4j: https://neo4j.com/docs/graph-data-science/current/algorithms/louvain/.

### Presentation
https://sites.google.com/view/nashvilleprovidersds4/home

### Findings
We took the dataset of just over 6K unique Nashville providers and general acute care hospitals and ran the Louvain community detection algorithm. We determined that each community of providers revolves primarily around one hospital. We used the zip code of the provider office locations and generated a heatmap of the communities of Medicare recipients each hospital serves. The analysis revealed that providers-hospital communities are dominated by three major hospital systems and fall into geographic clusters but the zip codes are served at different intensities. <br />
We found that HCA dominates the market in terms of Medicare patient referral volume from some of the largest specialties and subspecialties in middle TN. There is a couple of specific sub-specialties where Vanderbilt could grow their Medicare referrals substantially. There are a number of medical conditions that are increasingly prevalent in the primary demographic of Medicare recipients. Based on market insights, we have identified a growth opportunity for VUMC in pulmonary and cardiac subspecialties.
