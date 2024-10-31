# Drug_Reg_ANVISA
**Project Status**: [Current status: In progress, completed, etc.]

## **ATTENTION**
> Run the script in a **Python** environment, but use responsably. Mistakes can be commited.
  ### Dependencies (libraries used):
    import pandas as pd
    import matplotlib.pyplot as plt
    import plotly.express as px
    from matplotlib.text import Text
    import seaborn as sns

  
## Project Overview

This project aims to explore the Brazilian pharmaceutical market by analyzing data on drug registrations from the Brazilian Health Surveillance Agency (ANVISA).

ANVISA DATABASE: Medicines Registered in Brazil

> _"The open drug registration database is a data intelligence project that extracts information from the Datavisa system to list products that have been registered by Anvisa, including those whose registration is already valid or canceled/expired, as reported on the Agency's consultation portal."_

> URL: https://dados.gov.br/dados/conjuntos-dados/medicamentos-registrados-no-brasil

The dataset includes information about:
- 'PRODUCT_TYPE';
- 'PRODUCT_NAME';
- 'PROCESS_END_DATE';
- 'REGULATORY_CATEGORY';
- 'PRODUCT_REGISTRATION_NUMBER';
- 'REGISTRATION_EXPIRATION_DATE';
- 'PROCESS_NUMBER';
- 'THERAPEUTIC_CLASS';
- 'REGISTRATION_HOLDER_COMPANY';
- 'REGISTRATION_STATUS';
- 'ACTIVE_INGREDIENT'.

## Project guideline

- How can we use data on drug registrations in Brazil over the years to understand the evolution of the pharmaceutical market?
  
- What the frequency of new drug registrations can reveal in the pharmaceutical market?

- Can we analyze the competitive landscape in the pharmaceutical market? Are able to identify market niches?

## Project Deliverables

**Data Cleaning and Preprocessing**

The dataframe consists of 31317 entries, divided into 11 nominal categorical variables.

Analysing tha variables and missing data:
- **PRODUCT_TYPE** > only the name 'medicine';
- **PROCESS_END_DATE** > the missing values demonstrates the 518 were not completed;
- **PRODUCT_REGISTRATION_NUMBER** > a total of 31317 drug resgistration, but remains valid 11732 registers;
- **THERAPEUTIC_CLASS** > currently exists 548 terapeutical classes in use over the country;
- **REGISTRATION_HOLDER_COMPANY** > the company number were reduced from 718 to 359 companies with registered products;
- **ACTIVE_INGREDIENT** > are presented 2544 Active Pharmaceutical Ingredient registered.

The major 'REGULATORY_CATEGORY' are similar, generic and new (reference drugs). Another values will be set as 'Others'. Was founded 94 missing values, 0.8% of 11732 registers, that appear to not interfere in the data evaluation.

**Exploratory Data Analysis**

**Drug Registration by the Time**

Was develped a temporal series analysis beyond 1995. In 1999, a legal milestone was reached for the production of medicines, with the creation of the National Health Surveillance Agency (Anvisa) and the Generic Medicines Law.

Anvisa is a federal agency that acts in the sanitary control of products and services, responsible for registering and supervising the production of medicines, evaluating the technical and administrative documentation related to quality, safety and efficacy. The creation of this agency streamlined the process of registering new drugs.

A generic medicine is a medicine with the same active substance, pharmaceutical form, dosage and therapeutic indication as the **"reference medicine"** (patent holder), but without having a commercial name, only the name of the active pharmaceutical ingredient on its packaging. The **first was registered in 1998**, but after the politics the registration number raised.

While the generic medicine law, in addition to stimulating the production of generic medicines, allowed the production and marketing of medicines with expired patents. However, the greatest growth is related to "similar medicines", which are the generic with the trade name printed on its packaging, which favors its advertising, **which explains the growth above generic drugs in 2001**.

The peak in 2011 appers related to the "No category", thats seem to be an missclassified data. In these data are included as therapeutic class  anti-inflammatory, antihypertensives, bronchodilators, expectorants, antivirals, among others. **Drug classes that should be included in some regulatory category for comercialization**.

**Theapeutical Class Registration**

The evaluation over the time (temporal series) demonstrates the same pattern presented by the Durg Registragion. 

The number 1 are the antibiotics, due bacterial infections are prevalent across a range of age groups. 

Non-steroidal anti-inflammatory drugs (NSAIDs) relieve inflammatory, are most of the are OTC (Over The Counter) that can be sold directly to people without a prescription. Non-opioid analgesics are complementary to NSAIDs.
> If sum both will be the major class.

Antineoplastic and antidepressant drugs appear in the TOP 5 of the list because they treat the most common diseases in Brazil.

**Statistical Analysis**
> Perform statistical analysis to quantify the insights gained from the data and test hypotheses.

**Predictive Modeling**
> Develop machine learning models to predict future market trends.

Report: Summarize the key findings and insights, including recommendations for stakeholders in the pharmaceutical industry.



## Contribution Guidelines

Contributions are welcome! Please refer to the [Contribution Guidelines] for information on how to contribute to this project.

## Acknowledgements

[List any collaborators or individuals who contributed to the project.]

## License

[Specify the license used for the project.]

## Contact

[Provide contact information for the project maintainers.]

## Disclaimer

This project is for research and educational purposes only. The findings should not be considered financial or investment advice.
