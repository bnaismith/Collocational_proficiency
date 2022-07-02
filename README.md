# Examiner judgments of collocational proficiency in L2 English learners’ writing <br/><br/>

### Ben Naismith

<br/>

**Recommended citation:**

Naismith, B. (2022). Examiner judgments of collocational proficiency in L2 English learners’ writing. [Unpublished doctoral dissertation]. University of Pittsburgh. http://d-scholarship.pitt.edu/42374/  

***

### Abstract
This study investigates how aspects of collocational proficiency affect the ratings that expert examiners give to second language (L2) English learner essays. Lexical proficiency is a multi-faceted phenomenon and certain aspects of it are particularly impactful on human judgements, including lexical sophistication and accuracy. However, the importance of proficiency with formulaic sequences (FSs), like collocations, has received less attention than proficiency with single words, despite FSs’ essential role in language production. In addition, previous comparison studies have used a small number of raters with varying levels of assessment expertise, assessing texts of varying length and topic.  

In addressing these issues, this study uses a predominantly quantitative, experimental approach comprised of two stages. First, a small set of three texts of different proficiency levels were created based on model IELTS Task 2 essays, controlling for topic and length. From these texts, a set of 30 versions were produced, manipulating specific collocational features related to sophistication and accuracy. Second, IELTS examiners (_n_ = 47) rated the texts and provided rationales for their choices. From these data, many-faceted Rasch models were used to obtain expected scores, and linear regression models were used to determine which aspects of collocational proficiency best predicted the experts’ ratings.  

The findings reveal that increases in lexical sophistication significantly and positively impacted the experts’ ratings. Post-hoc analyses demonstrated that the categories of high sophistication and mid sophistication differed significantly from low sophistication. However, mid sophistication was not significantly different from high sophistication. When these ‘advanced’ words were used as part of collocations, they then provided a small but significant additional boost to ratings. Notably, there was no significant effect for increased collocational accuracy. In conjunction, these findings indicate that 1) sophistication is perhaps best viewed on a spectrum rather than categorically, 2) there is an additional increase to ratings if learners use advanced lexis as part of collocations, and 3) there is a potential baseline in terms of gravity and frequency of collocation errors below which ratings are not significantly affected. The implications for these findings are therefore discussed in relation to written language assessment and L2 vocabulary pedagogy.

**Key words:** Collocation; Proficiency; Sophistication; Accuracy; Assessment

***

### Contents

This public GitHub repository contains some of the code for the dissertation cited above. All of the code is written using Python 3.8 or R 3.6.2 and is presented in Jupyter notebooks. There are 14 notebooks which address different aspects of the project, divided into three stages: _Creating instruments_, _Processing data_, and _Analyzing data_. In many cases, the notebooks follow a sequential order, loading pickle (`.pkl`) and csv files from previous notebooks. These `.pkl` and `.csv` files are contained in the `docs` folder.

<br/>  

_Creating instruments_

Notebook                                | Description
:---                                    | :---
`01_normalizing_B1_original_text.ipynb` | Creating a length-normalized B1 text from the original public IELTS Task 2 B1 text. Focus on measures of lexical and grammatical sophistication, diversity, complexity, and accuracy.
`02_normalizing_B2_original_text.ipynb` | Creating a length-normalized B2 text from the original public IELTS Task 2 B2 text. Focus on measures of lexical and grammatical sophistication, diversity, complexity, and accuracy.
`03_normalizing_C1_original_text.ipynb` | Creating a length-normalized C1 text from the original public IELTS Task 2 C1 text. Focus on measures of lexical and grammatical sophistication, diversity, complexity, and accuracy.
`4_identifying_collocations.ipynb`      | Exploring frequency statistics from COCA to identify potential collocations to change in the original and normalized text versions
`05_creating_base_texts`                | Creating the three base texts (B1, B2, C1) from the normalized texts. The base texts are very similar to the normalized texts, but with slightly modified collocations to ensure a more even distribution across levels.
`06_processing_base_texts`              | Processing the base texts by calculating measures related to lexical diversity and sophistication, grammatical complexity, and other collocational proficiency metrics. These are the same indices calculated during the text normalization process from notebooks 01, 02, 03.
`07_creating_B1_text_versions.ipynb`    | Creating a set of 10 texts from the B1 base text by carefully manipulating collocational sophistication and accuracy
`08_creating_B2_text_versions.ipynb`    | Creating a set of 10 texts from the B2 base text by carefully manipulating collocational sophistication and accuracy
`09_creating_C1_text_versions.ipynb`    | Creating a set of 10 texts from the C1 base text by carefully manipulating collocational sophistication and accuracy

<br/>  

_Processing data_

Notebook                                       | Description
:---                                           | :---
`10_processing_quantitative_survey_data.ipynb` | Cleaning the quantitative data from the Qualtrics survey for future statistical analysis
`11_processing_qualitative_survey_data.ipynb`  | Cleaning the qualitative data from the Qualtrics survey for future statistical analysis
`12_integrating_data_from_FACETS.ipynb`        | Combining MFRM model output from FACETS (see 'Important notes' #2) with the other survey data

<br/>  

_Analyzing data_   

Notebook                          | Description
:---                              | :---
`13_analyzing_control_data.ipynb` | Producing the descriptive statistics for the control data to check that after manipulations, the original, normalized, and base texts all received comparable ratings from the human raters
`14_analyzing_survey_data.ipynb`  | Producing the descriptive and inferential statistics for the main survey data and creating accompanying visualizations

<br/>  

### Important notes
1. The frequency information from COCA referenced here is not freely available but can be purchased at https://corpus.byu.edu/. Without this data you will be able to see samples of the output of the Jupyter notebooks but will not be able to run them completely.
2. The many facets Rasch models (MFRM) were created using the freely available [Facets software](https://www.winsteps.com).

<br/>  

### Copyright
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/" target="_blank"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png"/></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/" target="_blank">Creative Commons Attribution 4.0 International License</a>.
