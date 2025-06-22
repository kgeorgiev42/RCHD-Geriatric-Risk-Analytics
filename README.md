# Harnessing Routine Data and Healthcare Contacts to Predict Risk and Treatment Requirements in Older People

_PhD Thesis Supplementary Codebase_

### _Konstantin Georgiev_

### _BHF Centre for Cardiovascular Science, University of Edinburgh_

---

## Description
This repository contains the supporting codebase for the PhD thesis titled **"Harnessing Routine Data and Healthcare Contacts to Predict Risk and Treatment Requirements in Older People"**. The codebase provides scripts for the analysis of routine healthcare data, focusing on risk prediction, treatment requirements, and care pathway analytics relevant to geriatric care planning. The original work is based on data from NHS Lothian care systems, conducted within [DataLoch](https://dataloch.org/) Secure Data Environments (SDEs).

## Codebase Structure

- **data/**: currently contains the open [COCHRANE REH-COVER](https://rehabilitation.cochrane.org/special-projects/completed-special-projects/REH-COVER) summary data collated from previous systematic review rounds, used for the analysis in Chapter 4. Future data will include synthetic EHRs for Machine Learning and Process Mining pipelines.

- **docs/**: basic documentation, including structured overviews of the analysis code and related work.

- **notebooks/**: Jupyter and R Markdown notebooks and files covering the original data processing pipelines used to conduct the experiments within [DataLoch](https://dataloch.org/) Secure Data Enviroments:
  1) [cv19_statistics](https://github.com/kgeorgiev42/RCHD-Geriatric-Risk-Analytics/blob/main/docs/cv19_statistics.md): relevant to statistical analysis and mapping for COVID-19 care pathways and rehabilitation interventions (covered in Chapters 4, 5 and 6)
  2) [process_mining](https://github.com/kgeorgiev42/RCHD-Geriatric-Risk-Analytics/blob/main/docs/process_mining.md): relevant to Process Mining analytics for comparison of care interactions between COVID-19 pandemic waves (covered in Chapter 6).
  3) [geriatric_ml](https://github.com/kgeorgiev42/RCHD-Geriatric-Risk-Analytics/blob/main/docs/geriatric_ml.md): relevant to Machine Learning analytics for risk and resource predictions in urgently hospitalised older patients (covered in Chapter 8).

---

## Work in Progress
- The codebase is under active development to enable reproduction of these experiments on synthetic (dummy) healthcare data. Some scripts and pipelines are prototypes or in-progress. The `src/` folder will be used to construct data pipelines for Machine Learning and Process Mining analytics related to geriatric care pathways.

---

## Citations
If you use this codebase or its methods, please cite any of the related published work:

- Georgiev, K., Fleuriot, J.D., Papapanagiotou, P. et al. "Comparing Care Pathways Between COVID-19 Pandemic Waves Using Electronic Health Records: A Process Mining Case Study". *J Healthc Inform Res* 9, 41–66 (2025). https://doi.org/10.1007/s41666-024-00181-6
- Georgiev, K., Fleuriot, J.D., Papapanagiotou, P. et al. "Comparing Care Pathways Between COVID-19 Pandemic Waves Using Electronic Health Records: A Process Mining Case Study." *J Healthc Inform Res* 9, 41–66 (2025). https://doi.org/10.1007/s41666-024-00181-6
- Georgiev, K., McPeake, J., Shenkin, S.D. et al. "Understanding hospital activity and outcomes for people with multimorbidity using electronic health records". *Sci Rep* 15, 8522 (2025). https://doi.org/10.1038/s41598-025-92940-7
- Georgiev, K., et al., "Predicting incident dementia in community-dwelling older adults using primary and secondary care data from electronic health records", **Brain Communications*, Volume 7, Issue 1, 2025, fcae469, https://doi.org/10.1093/braincomms/fcae469

## Acknowledgments

This thesis is supported by a PhD Fellowship award from the Sir Jules Thorn Charitable Trust (21/01PhD) as part of the University of Edinburgh’s Precision Medicine PhD programme.

The original data studies were supported by [DataLoch](dataloch.org), which is core-funded by the [Data-Driven Innovation programme](ddi.ac.uk) within the Edinburgh and South East Scotland City Region Deal, and the [Chief Scientist Office](cso.scot.nhs.uk), Scottish Government.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
