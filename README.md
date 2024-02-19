# AI Case Study of Credo Health Solutions, Inc.

## Introduction
Credo Health Solutions, Inc. ([Credo Health](https://www.credohealth.com/)) is a privately held, venture-capital-backed start-up in the healthcare industry[^1]. It was incorporated in 2021 in Denver, CO, by Carm Huntress[^1] [^2].

Credo Health aims to automate the patient medical record retrieval process for healthcare providers[^3].

Credo Health has gone through two rounds of seed funding for a total of $8.25 million from 8 investors ($3 million in March of 2022 and $5.25 million in January of 2024)[^1] [^2]. The company has grown from 6 employees to 24 employees between March of 2022 and January of 2024[^1] [^2].

Carm Huntress was inspired by his mother who carried stacks of her patient records with her from medical appointment to medical appointment when she was ill with cancer in the early to mid 1990. To quote Mr. Huntress[^4]:
> Patients today still carry around their paper records like my Mom did. We still fax (yes, fax!) over nine billion pages of medical records annually and spend $126 billion managing those faxes and paper records. Three out of every ten diagnostic tests have to be repeated because caregivers can’t find previous patient records.

> [!Note]
> Since Credo Health is privately held, it was difficult to find independent information on the company. Hence, the following information might be biased and incomplete since it was obtained mostly from company sources such as the company's website, blogs or articles written by the company's founder and published in various Internet publications.

## Problem Statement, Company Solution, and Technology

### Problem Statement

Although medical patient records are mostly digitized in Electronic Health Record (EHR) systems, in many instances, healthcare providers still exchange these records via Fax or email[^5]. In addition, the information contained in these often voluminous records is not synthesized before consumption by the receiving provider[^5].

Some of the inefficiences caused by this lack of interoperability are
* Delay in patient care due to incomplete patient medical records[^6].
* Administrative overhead due to "chart chasing"[^3].
* Repeated diagnostic tests because records of previous tests could not be found[^4].
* Incomplete coding of patients medical conditions which causes loss of revenue and may lead to bad patient care[^7].

It is estimated that these inefficiencies cost the healthcare industry over $100 billion a year[^5].  

### Company Solution

With its PreDx software application, launched in March/April of 2023[^8], Credo Health aims to address these inefficiences by
1. Automating the retrieval of patient records.
2. Applying AI to synthesize the often voluminous records into a user-friendly summary.
3. Making all the data available to the provider before a patient's appointment.

The target market for PreDx are value-based care providers serving Medicare Advantage patients[^8].

### Technology and Methods

According to the [Credo Health blog](https://www.credohealth.com/blog), PreDx employs the following technologies and methods[^8]:
* Automated, digital retrieval of patient records combined with manual retrieval of records to fill in the gaps.
* Using proprietary AI and ML algorithms, trained on its own data, in combination with in-house clinicians to synthesize the patient records into a summary for the provider.
* The Credo Health Blog contains articles[^7] [^9] referring to how large language models (LLM) can be applied to analyze medical records suggesting that PreDx uses this technology as well.

> [!Note]
> From my own experience in the healthcare industry (10 years of providing IT support and services for Medicare Advantage clinics), Credo Health probably uses the following more specific technologies:
> * FHIR, CCDA and similar protocols and standards in conjunction with Health Information Exchanges (HIE) and Health Information Service Providers (HISP) to retrieve medical records from external parties.
> * Optical Character Recognition (OCR) to process many of the retrieved records into computer readable form.
> * Natural Language Processing (NLP) to understand the meaning behind the retrieved medical records.

## Competitors and Competive Advantage

According to [CB Insights](https://www.cbinsights.com/) the top 5 competitors of Credo Health are[^10]:
* [MDPortals](https://www.mdportals.com/)
* [Apixio](https://www.apixio.com/)
* [Ciox Health](https://www.cioxhealth.com/)
* [DrOwl](https://www.drowl.com/)
* [Ontellus](https://www.ontellus.com/)

The top competitive advantages of the Credo Health solution compared to its competitors are are:
* The precentage of patient records retrieved.
* The precentage increase in the Risk Adjustment Factor (RAF).
* The increase in HEDIS/Stars measures.

## Landscape

* What field is the company in?

* What have been the major trends and innovations of this field over the last 5&ndash;10 years?

* What are the other major companies in this field?

## Results

* What has been the business impact of this company so far?

* What are some of the core metrics that companies in this field use to measure success? How is your company performing based on these metrics?

* How is your company performing relative to competitors in the same field?

## Recommendations

* If you were to advise the company, what products or services would you suggest they offer? (This could be something that a competitor offers, or use your imagination!)

* Why do you think that offering this product or service would benefit the company?

* What technologies would this additional product or service utilize?

* Why are these technologies appropriate for your solution?

## Glossary
| Term        | Definition                                                                        |
|-------------|-----------------------------------------------------------------------------------|
| HEDIS       | HEDIS stands for "Healthcare Effectiveness Data and Information Set". It is a widely used management tool in the healthcare industry. It allows to measure the health of a population and the quality of care this population receives in a standardized way thereby allowing for comparisons between the health and quality of care different populations receive. It is based on "scientific evidence, input from key stakeholders and experts in health measurement".[^11] | 

## Footnotes

[^1]: https://pitchbook.com/profiles/company/491815-99#overview, accessed on 2/16/2024.
[^2]: Rumage, Jeff (2022, March 7). *Newly Launched Credo Raises $3M to Gather Medical Charts for Providers* Built in Colorado. https://www.builtincolorado.com/2022/03/07/healthtech-credo-launches-3m-funding.
[^3]: De Lombaerde, Geert (2022, March 7). *Medical Records Startup Takes Aim at Chart Chasing*, Healthcare Innovation, https://www.hcinnovationgroup.com/clinical-it/article/21259264/medical-records-startup-takes-aim-at-chart-chasing.
[^4]: Huntress, Carm (2022). *26 Years Later: Carm Huntress' Inspiration Behind Credo Health*, Credo Helath Blog, https://www.credohealth.com/blog/26-years-later-carm-huntress-inspiration-behind-credo-health.
[^5]: Huntress, Carm (2023, March 3). *Medical Records Are Costing Us $125 Billion Every Year. It’s Time for Something to Change*, Nashville Medical News, https://www.nashvillemedicalnews.com/article/5818/medical-records-are-costing-us-125-billion-every-year-its-time-for-something-to-change.
[^6]: (2022, November 21). *3 Problems Keeping Healthcare Trapped in the 20th Century*,  Credo Health Blog, https://www.credohealth.com/blog/3-problems-keeping-healthcare-trapped-in-the-20th-century.
[^7]: Huntress, Carm (2023, May 3). *How AI can help physicians with pre-encounter medical record analysis*, Medical Economics, https://www.medicaleconomics.com/view/how-ai-can-help-physicians-with-pre-encounter-medical-record-analysis.
[^8]: (2023, March 27). *Credo Unveils PreDx - The First Pre-Encounter Patient Summary Solution Enabling Providers to Excel in VBC*, Credo Health Blog, https://www.credohealth.com/blog/credo-unveils-predx-the-first-pre-encounter-patient-summary-solution-enabling-providers-to-excel-in-value-based-care
[^9]: (2023, May 9). *From ChatGPT to the Complete Digital Medical Record*, Credo Health Blog, https://www.credohealth.com/blog/from-chatgpt-to-the-complete-digital-medical-record.
[^10]: https://www.cbinsights.com/company/credo-5/alternatives-competitors, accessed on 2/16/2024.
[^11]: https://www.ncqa.org/wp-content/themes/ncqa-org/css/images/landing-employer-toolkit/pdf/NCQA-HPA-MeasuringHCQ-HEDIS-WEB.pdf, accessed on 2/19/2024.
