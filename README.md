# AI Case Study of Credo Health Solutions, Inc.

## Introduction
Credo Health Solutions, Inc. ([Credo Health](https://www.credohealth.com/)) is a privately held, venture-capital-backed start-up in the healthcare industry[^1]. It was incorporated in 2021 in Denver, CO, by Carm Huntress[^1],[^2].

Credo Health aims to automate the patient medical record retrieval process for healthcare providers[^3].

Credo Health has gone through two rounds of seed funding for a total of $8.25 million from 8 investors ($3 million in March of 2022 and $5.25 million in January of 2024)[^1],[^2]. The company has grown from 6 employees to 24 employees between March of 2022 and January of 2024[^1],[^2].

Carm Huntress was inspired to create Credo Health by his mother who carried stacks of her patient records with her from medical appointment to medical appointment when she was ill with cancer in the early to mid 1990. To quote Mr. Huntress[^4]:
> Patients today still carry around their paper records like my Mom did. We still fax (yes, fax!) over nine billion pages of medical records annually and spend $126 billion managing those faxes and paper records. Three out of every ten diagnostic tests have to be repeated because caregivers can’t find previous patient records.

> [!Note]
> Since Credo Health is privately held, it was difficult to find independent information about the company. Hence, the following information relating specifically to Credo Health might be biased and incomplete since it was obtained mostly from company sources such as the company's website, blogs or articles written by the company's founder and published in various Internet publications.

## Problem Statement, Company Solution, and Technology

### Problem Statement

Although medical patient records are mostly digitized in Electronic Health Record (EHR) systems, due to a lack of interoperability between these systems, healthcare providers still often exchange patient records via Fax or email[^5]. In addition, the information contained in these often voluminous records is not synthesized before consumption by the receiving provider[^5].

Some of the inefficiences caused by this lack of interoperability are
* Delay in patient care due to incomplete patient medical records[^6].
* Administrative overhead due to "chart chasing"[^3].
* Repeated diagnostic tests because records of previous tests could not be found[^4].
* Incomplete coding of patients' medical conditions which causes loss of revenue and may lead to bad patient care[^7].

More specifically, Credo Health maintains[^8] that on average
* Front desk staff spends
  - 1.5 hours per day chasing charts.
  - $20 on sending a fax.
* Providers
  - Spend 5 hours previewing patient charts per week.
  - Have access to only 10% of the available records prior to a patient's first visit.
* Risk Adjustment
  - Requires to manually review 1000+ records every day.
  - Is missing 25% of reported conditions.

It is estimated that these inefficiencies cost the healthcare industry over $100 billion a year[^5].  

### Company Solution

With its PreDx software application, launched in March/April of 2023[^9], Credo Health aims to address these inefficiences by[^10]
1. Automating the retrieval of patient records.
2. Applying AI to analyze the often voluminous records. More specifically, the application will identify possibly relevant [HCC](#Glossary)s to improve and speed up risk adjustment.
3. Summarizing the patient record to provide a review of a patient's complete clinical picture prior to the patient's appointment. This summary includes medications, recent labs, previous diagnoses, and previous medical procedures.

The target market for PreDx are value-based care providers serving Medicare Advantage patients[^9].

### Technology and Methods

According to the [Credo Health blog](https://www.credohealth.com/blog), PreDx employs the following technologies and methods[^9]:
* Automated, digital retrieval of patient records combined with manual retrieval of records to fill in the gaps.
* Using proprietary AI and ML algorithms, trained on its own data, in combination with in-house clinicians to synthesize the patient records into a summary for the provider.
* The Credo Health Blog contains articles[^7],[^11] referring to how large language models (LLM) can be applied to analyze medical records suggesting that PreDx uses this technology as well.

> [!Note]
> From the author's experience in the healthcare industry (10 years of providing IT support and services for Medicare Advantage clinics), Credo Health probably uses the following technologies in addition to and conjunction with the technologies listed above:
> * [FHIR](#Glossary), [CCDA](#Glossary) and similar protocols and standards in conjunction with Health Information Exchanges (HIE) and Health Information Service Providers (HISP) to retrieve medical records from external parties.
> * Optical Character Recognition (OCR) to process many of the retrieved records into computer readable form.
> * Natural Language Processing (NLP) to understand the meaning behind the retrieved medical records.

## Industry Trends and Advances

The following healthcare industry trends and advances work in Credo Health's favor:
* Adoption of industry standards such as FHIR and CCDA.
* Implementation of Health Information Exchanges and Health Information Service Providers.
* The 21st Century Cures Act which seeks to advance interoperability in the healthcare industry[^12].
* CMS [HCC](#glossary) Model V28 which requires greater specificity when documenting and coding a patient's illness for the purpose of receiving funds for Medicare Advantage patients[^13].
* Continued improvement in AI and ML tools and algorithms.

## Competitors and Competitive Advantage

According to [CB Insights](https://www.cbinsights.com/) the top 5 competitors of Credo Health are[^14]:
* [MDPortals](https://www.mdportals.com/)
* [Apixio](https://www.apixio.com/)
* [Ciox Health](https://www.cioxhealth.com/)
* [DrOwl](https://www.drowl.com/)
* [Ontellus](https://www.ontellus.com/)

The top competitive advantages of the Credo Health solution compared to its competitors are[^10],[^15],[^16],[^17],[^18],[^19]:
* The precentage of patient records retrieved.
* The precentage increase in the Risk Adjustment Factor ([RAF](#Glossary)).
* The increase in [HEDIS/Stars](#Glossary) measures.
* Seemless integration into EHR applications.

## Results

Credo Health is quoting a [Wakely](https://www.wakely.com/) Consulting Group validated case study that found[^10]
* A 98.5% patient record retrieval rate.
* An average of 71+ records retrieved per patient.
* An average increase in HCC value of 0.286 (V28) found per patient.

In addition, Credo Health maintains that[^8]
* Their solution saves a provider on average 1-2 hours on chart retrieval per patient.
* 100% of a patient's health conditions are documented on the patient's first visit.
* The increase in HCC value is fully supported by clinical evidence which the solution references in the patient record.

> [!Note]
> Unfortunately, the author was unable to independently verify these results or determine how these results compare with competitors' results beyond what is described in section [Competitors and Competitive Advantage](#competitors-and-competitive-advantage) above.

## Recommendations

The author recommends to increase the number of sources that are analyzed and summarized prior to a patient's visit. Currently, these sources only seem to include historical patient records and maybe the patient record residing in the provider's EHR system. To create an even more comprehensive, [longitudinal health record](#Glossary) of the patient, other sources to include could be
* Digital images evaluated using AI and ML algorithms.
* Readings from medical devices that are in the patient's possession, such as weight scales, blood pressure cuffs, thermometers, heart rate monitors, blood sugar monitors, etc.
* Logs about the patient's exercise or physical activity.
* [Social determinants of health](#Glossary).

All of this data could be analyzed using AI and ML to not only determine what the current health condition is of a patient, but, also, to determine what their future health conditions might be[^20]. This could provide valuable insights into what preventative measures to implement for that patient. One of the goals would be to prevent diseases, postpone their onset, or their progression, thereby improving patients' quality of life and saving the healthcare system money.

---
---

## Glossary
| Term        | Definition |
|-------------|------------|
| CCDA        | "Consolidate Clinical Document Architecture". It is the most widely used standard in the US to document patient encounters thereby facilitating the exchange of health information.[^21] |
| CMS         | "Center for Medicare and Medicaid Services". Governement agency that manages the Medicare, Medicaid, and the Children's Health Insurance  programs. It also manages the Health Insurance Marketplace.[^22] |
| FHIR        | "Fast Healthcare Interoperability Resource". A standard that defines how healthcare information can be exchanged between different computer systems regardless of how it is stored in each system.[^23] |
| HCC         | "Hierarchical Condition Categories". It is a set of medical codes that are linked to specific diagnoses. They are used to determine the risk adjustment factor for a patient.[^24] HCC is expressed in a value that is less than one for patients that are healthier than average and larger than one for patients that are less healthy than average.[^25] |
| HEDIS       | "Healthcare Effectiveness Data and Information Set". It is a widely used management tool in the healthcare industry. It allows to measure, in a standardized way, the health of a population and the quality of care this population receives, thereby allowing for comparisons between the health and quality of care of different populations. It is based on "scientific evidence, input from key stakeholders and experts in health measurement".[^26] |
|Longitudinal Health Record | "The Longitudinal Record is a single comprehensive patient record comprised of data from numerous data sources across the healthcare continuum."[^27] |
| RAF         | "Risk Adjustment Factor". It is used to determine how to adjust payments to Medicare Advantage Organizations, among others, for the expected healthcare costs of their enrollees. It is based on disease factors and demographics.[^28] |
| Social Determinants of Health | "Social determinants of health (SDOH) are the conditions in the environments where people are born, live, learn, work, play, worship, and age that affect a wide range of health, functioning, and quality-of-life outcomes and risks."[^29] |
| Stars       | The Star rating is published by CMS yearly. It allows Medicare consumers to compare the quality of Medicare health and drug plans.[^30] |

## Footnotes

[^1]: *Credo Health Overview*, Pitchbook Website, https://pitchbook.com/profiles/company/491815-99#overview, accessed on 2/16/2024.
[^2]: Rumage, Jeff (2022, March 7). *Newly Launched Credo Raises $3M to Gather Medical Charts for Providers*, Built in Colorado, https://www.builtincolorado.com/2022/03/07/healthtech-credo-launches-3m-funding.
[^3]: De Lombaerde, Geert (2022, March 7). *Medical Records Startup Takes Aim at Chart Chasing*, Healthcare Innovation, https://www.hcinnovationgroup.com/clinical-it/article/21259264/medical-records-startup-takes-aim-at-chart-chasing.
[^4]: Huntress, Carm (2022). *26 Years Later: Carm Huntress' Inspiration Behind Credo Health*, Credo Helath Blog, https://www.credohealth.com/blog/26-years-later-carm-huntress-inspiration-behind-credo-health.
[^5]: Huntress, Carm (2023, March 3). *Medical Records Are Costing Us $125 Billion Every Year. It’s Time for Something to Change*, Nashville Medical News, https://www.nashvillemedicalnews.com/article/5818/medical-records-are-costing-us-125-billion-every-year-its-time-for-something-to-change.
[^6]: (2022, November 21). *3 Problems Keeping Healthcare Trapped in the 20th Century*,  Credo Health Blog, https://www.credohealth.com/blog/3-problems-keeping-healthcare-trapped-in-the-20th-century.
[^7]: Huntress, Carm (2023, May 3). *How AI can help physicians with pre-encounter medical record analysis*, Medical Economics, https://www.medicaleconomics.com/view/how-ai-can-help-physicians-with-pre-encounter-medical-record-analysis.
[^8]: *There’s nothing riskier than taking on risk without the complete clinical picture.*, Credo Health Website, https://www.credohealth.com/risk-adjustment, accessed 2/19/2024.
[^9]: (2023, March 27). *Credo Unveils PreDx - The First Pre-Encounter Patient Summary Solution Enabling Providers to Excel in VBC*, Credo Health Blog, https://www.credohealth.com/blog/credo-unveils-predx-the-first-pre-encounter-patient-summary-solution-enabling-providers-to-excel-in-value-based-care.
[^10]: *Digitally native. Fully integrated. The first of its kind.*, Credo Health Website, https://www.credohealth.com/product, accessed on 2/19/2024.
[^11]: (2023, May 9). *From ChatGPT to the Complete Digital Medical Record*, Credo Health Blog, https://www.credohealth.com/blog/from-chatgpt-to-the-complete-digital-medical-record.
[^12]: (2023, January). *Interoperability and Methods of Exchange among Hospitals in 2021*, ONC Data Brief, No. 64, https://www.healthit.gov/data/data-briefs/interoperability-and-methods-exchange-among-hospitals-2021.
[^13]: Selvaraj, Jayashree (2024, January 4). *Understanding the Changes in the CMS-HCC Model V28*, AGS Health Blog, https://www.agshealth.com/blog/understanding-the-changes-in-the-cms-hcc-model-v28/#:~:text=HCC%20model%20V28%20will%20require,future%20analysis%20in%20model%20recommendations.
[^14]: *Credo's alternatives and competitors*, CB Information Services (CBInsights) Website, https://www.cbinsights.com/company/credo-5/alternatives-competitors, accessed on 2/16/2024.
[^15]: *Compare Credo vs MDPortals*, CB Information Services (CBInsights) Website, https://www.cbinsights.com/compare/credo-5-vs-mdportals, accessed on 2/19/2024.
[^16]: *Compare Apixio vs Credo*, CB Information Services (CBInsights) Website, https://www.cbinsights.com/compare/apixio-vs-credo-5, accessed on 2/19/2024.
[^17]: *Compare Ciox Health vs Credo*, CB Information Services (CBInsights) Website, https://www.cbinsights.com/compare/ciox-health-vs-credo-5, accessed on 2/19/2024.
[^18]: *Compare Credo vs DrOwl*, CB Information Services (CBInsights) Website, https://www.cbinsights.com/compare/credo-5-vs-drowl, accessd on 2/19/2024.
[^19]: *Compare Credo vs Ontellus*, CB Information Services (CBInsights) Website, https://www.cbinsights.com/compare/credo-5-vs-keais-records-service, accessed on 2/19/2024.
[^20]: Carrasco-Ribelles, Lucia A, et al. (2023, September 2) *Prediction models using artificial intelligence and longitudinal data from electronic health records: a systematic methodological review*, Journal of the American Medical Informatics Association, Volume 30, Issue 12, December 2023, Pages 2072–2082, https://academic.oup.com/jamia/article/30/12/2072/7259105.
[^21]: *What is C-CDA?*, Particle Health, Inc Website, https://www.particlehealth.com/blog/what-is-ccda-consolidated-clinical-document-architecture#:~:text=C%2DCDA%20stands%20for%20Consolidated,Document%20Architecture%20(CDA)%20style., accessed on 2/16/2024.
[^22]: *Centers for Medicare and Medicaid Services (CMS)*, USA Gov Website, https://www.usa.gov/agencies/centers-for-medicare-and-medicaid-services#:~:text=The%20Centers%20for%20Medicare%20and,and%20the%20Health%20Insurance%20Marketplace., accessed on 2/19/2024.
[^23]: *What is FHIR?*, The Office of the National Coordinator for Health Information Technology Website, https://www.healthit.gov/sites/default/files/2019-08/ONCFHIRFSWhatIsFHIR.pdf, accessed on 2/19/2024.
[^24]: *HCC 101: What you need to know about Hierarchical Condition Categories*, Intelligent Medical Objects Ideas Website, https://www.imohealth.com/ideas/article/hcc-101-what-you-need-to-know-about-hierarchical-condition-categories/, accessed 2/19/2024.
[^25]: *An Introduction to Hierarchical Condition Categories (HCC)*, American Society of Anesthesiologists Website, https://www.asahq.org/quality-and-practice-management/managing-your-practice/timely-topics-in-payment-and-practice-management/an-introduction-to-hierarchical-condition-categories-hcc#:~:text=Patients%20that%20are%20healthier%20than,have%20a%20score%20above%201.000.
[^26]: *What is HEDIS®1?*, National Committee for Quality Assurance (NCQA) Website, https://www.ncqa.org/wp-content/themes/ncqa-org/css/images/landing-employer-toolkit/pdf/NCQA-HPA-MeasuringHCQ-HEDIS-WEB.pdf, accessed on 2/19/2024.
[^27]: (2020, May 6), *Longitudinal Record Use Case*, Michigan Health Information Network Website, https://mihin.org/wp-content/uploads/2020/06/MiHIN-Longitudinal-Record-Use-Case-Summary-FINAL-v3-05-06-20.pdf.
[^28]: *Module 1: Risk Adjustment Introduction and Overview*, Department of Health & Human Services Website, https://www.hhs.gov/guidance/sites/default/files/hhs-guidance-documents/2012313873-fg-riskadjustmentmethodology_module1.pdf, accessed on 2/19/2024.
[^29]: *Social Determinants of Health*, National Committee for Quality Assurance (NCQA) Website, https://health.gov/healthypeople/priority-areas/social-determinants-health, accessed on 2/29/2024.
[^30]: (2022, October 6). *2023 Medicare Advantage and Part D Star Ratings Fact Sheet*, Department of Health & Human Services Website, https://www.cms.gov/files/document/2023-medicare-star-ratings-fact-sheet.pdf, accessed on 2/19/2024.