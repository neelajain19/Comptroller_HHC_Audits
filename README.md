# Comptroller_HHC_Audits

## Project Background:

As part of my investigative health class, I am looking into a troubling pattern of medical biopsies conducted on schizophrenia patients at NYC Health & Hospital South Brooklyn Health (formerly known as Coney Island Hospital.) My reporting partner and I are looking into whether the biopsies are part of a medical research program or being conducted on an improper basis.  One of our sources, an emergency psychiatrist wondered if the procedures were coded erroneously as a way to take advantage of Medicaid reimbursement.  (The majority of patients on whom the biopsies were conducted on were insured via Medicaid.) My conversation with her prompted me to begin looking further into improper billing purposes at NYC Health & Hospitals.

## Scrape Process:

I identified several [NYC Health & Hospital audit reports](https://comptroller.nyc.gov/reports/?fwp_agency=health-and-hospitals-corporation) completed by the New York City Comptroller’s Office and 
[scraped](https://github.com/neelajain19/Comptroller_HHC_Audits/blob/21c3732478f6c58d154cb7e5bf570c2cd5de393d/01%20-%20Scraping.ipynb) the 
[PDFs](https://github.com/neelajain19/Comptroller_HHC_Audits/tree/71ef59bb8c90058f78f3e35a3b0a2d426f9d0b9a/Comptroller_Reports).

## Text Analysis Process:

Then as part of my text analysis I looked for the following keywords in the 20 or so audit reports to determine if HHC has a history of improper billing practices and, in particular, related to Medicaid:

Keywords:

Coney Island Hospital
Brooklyn Health South
improper billing practices
Medicaid reimbursement
Managed Care Organization
CSC billing policies
Fee for Service 
(FFS)
Anthony Rajkumar 
William Brown 
Svetlana Lipyanskaya 

I saved the results dataframe to a CSV file.  I then converted the CSV file to an Excel file and also added a tab with the pivot table that I mention below.

## Text Analysis Findings:  

Based on the results produced by my key word text analysis, I thought the best way to filter the results and identify the key PDFs that I need to sort through was by creating a pivot table that would show the PDFs with the most frequent references to key words.  

After creating the pivot table, I noticed that the highest number (175) of mentions to non-unique keywords (total of 708) pertained to “William” in the context of my keyword search for “William Brown”, who was a former Chief Executive Officer of Coney Island Hospital. When I checked the “Search Term with 15 Words Context”  for these mentions in the results, the majority (if not all) were in the context of the mention of “William C. Thompson, Jr. Comptroller” on the first page of all the audit reports.  The low similar score (33.3) for all these identifications was also reflective of that.  Therefore, I deduced that the keyword identification of this term did not yield information of value.  

I then thought it would be best to next look at the results for keyword searches for “Coney Island Hospital” and “Brooklyn Health South” as those are more specific terms than other keywords such as  “Medicaid Reimbursement” and “Fee for Service.”  Again, I decided to focus on the PDFs with most mentions of the hospital names based on my pivot table.  For “Coney Island Hospital” the two PDFs with the most references were 142A with 60 mentions and 111A with 50 mentions.  After briefly skimming these PDFs I quickly realized that while these PDFs focused on audits specific to Coney Island Hospital which is helpful, the audit topic was not particularly relevant to my investigative story.  (The PDFs were focused, respectively, on Coney Island Hospital’s compliance with HHC timekeeping and payroll standards as well as whether the hospital had appropriate controls in place for inventory of its non-controlled drugs.) In the case of identification of the keyword “Brooklyn Health South,” the two PDFs with the most mentions were 094A with 7 mentions  and 142A with 6 mentions.  I already knew that PDF 142A did not have relevant information to my story based on my above prior review of it so I did not review it again.  When I checked the context of the keyword identification for PDF 094A in the “Search Term” column I quickly realized that most of the references were in the context of lists of hospitals and naming the borough they were located in. Also considering that there were so few mentions of the hospital name, I also decided the PDF was not worth diving deeper into.

I then decided to take a look at some of the PDFs that had the most mentions of more general keywords such as “Medicaid reimbursement,” “Managed Care Organization” and “improper billing practices”.  I also wanted to focus on PDFs that had a significant number of mentions, not just in the single digits. This led me to hone in the following PDFs:

080A which had 78 mentions of “Medicaid”, 18 mentions of “improper” and 24 mentions of “fees”
152F which had 52 mentions of “Medicaid” and 48 mentions of “Managed”
067A which had 85 mentions of “fee”

Considering the number of keyword references in PDF 080A, I was hopeful this PDF would have information relevant to my investigative story concerning improper billing practices in relation to Medicaid.  However, this PDF was an audit of how well HHS adhered to provisions in a Memo of Understanding (MOU) detailing the conditions under which HHC would send payments to the CIty for Emergency Medical Services transports. The audit found that HHC did not comply with the conditions of the MOU, improperly overbilled the City and also was delayed in sending payments to the City.  Although the content of this audit is not directly related to improper billing practices specific to Medicaid in the context of Coney Island Hospital and South Brooklyn Health, it does supply evidence that HHC generally billing practices and financial controls have been lax and that the Office of the Comptroller requested improvements.

The next PDF I looked at was 152F which has several mentions of “Medicaid” and “Managed” in the context of ‘Managed Care.’ This PDF was particularly useful as it was a follow-up audit to determine if HHC has made improvements to its payment and collection practices as they relate to Medicaid Managed Care (MMC) and Health Maintenance Organizations (HMOs). One of the prior audit findings was that HHC only received payments from 72 billable accounts (only 14.5%) due to weaknesses in their billing and collections system.  One of the major factors contributing to this was a lack of training by HHC staff on billing practices as well as an inability to access basic billing and collection information. The audit found that HHC worked to potentially correct this issue by updating its contracting process with providers.

The last PDF I looked at was 067A, which, although it had 85 mentions of “fees”, did not contain any applicable information as it was an audit report on Harlem Hospital’s affiliation contract with Columbia University.  (On second thought, “fee” is an extremely general term to look for even in the context of the larger term “fee for service” so I likely should have not included it as part of my keywords

## Text Analysis Conclusion:

Analysis of the PDFs based on the number of keyword references found that HHC has a history of improper billing practices that were identified by the Office of the Comtroller. Although many of these PDFs are several years old (in some cases 15 years old), they do provide evidence that there is potential for the biopsy procedures to have been erroneously coded and billed for Medicaid reimbursement purposes.  It’s interesting that there are no more recent HHC audit reports on the Comptroller’s website.  Therefore, now that I know this keyword identification process yielded fruitful, though old results, I will inquire with the Office of the Comptroller regarding more recent audit reports or perhaps even submit a FOIA.
