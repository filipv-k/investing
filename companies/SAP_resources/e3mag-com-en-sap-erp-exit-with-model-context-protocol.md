[Skip to main content](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#brx-content) [Skip to footer](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#brx-footer)

[Editor-in-Chief Blog](https://e3mag.com/en/category/editor-in-chief-blog/)

# SAP ERP Exit with the Model Context Protocol

To understand the immense importance of MCP, one must consider the structural integration challenges of modern ERP landscapes. Until now, integrating AI with existing S/4 systems has been a tedious and proprietary nightmare.

Peter M. Färbinger, E3 Magazine

August 13, 2026

[![](https://e3mag.com/wp-content/uploads/2024/02/Banner_Content_Sidebar_300x250_ENG_1.jpg)](https://e3mag.com/en/en-newsletter-registration/)

Content:

[Media Discontinuities and APIs as Showstoppers](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#media-discontinuities-and-apis-as-showstoppers)

[New SAP ERP Architecture by MCP](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#new-sap-erp-architecture-by-mcp)

[Roland Berger Consulting: MCP Helps AI](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#roland-berger-consulting-mcp-helps-ai)

[MCP Openness vs. SAP Licensing Law](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#mcp-openness-vs-sap-licensing-law)

[API, BTP, and BDC Exits with the MCP Server](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#api,-btp,-and-bdc-exits-with-the-mcp-server)

[Pitfall: SAP ERP Audits](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#pitfall-sap-erp-audits)

[Seamless ERP with MCP Server](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#seamless-erp-with-mcp-server)

[Observability for LLMs via MCP](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#observability-for-llms-via-mcp)

[Conclusion: I can't do without my MCP server](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#conclusion-i-can't-do-without-my-mcp-server)

[To the comments (0)](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#kommentare)

![](https://e3mag.com/wp-content/uploads/2026/02/Chefredakteur-neu.jpeg)![](https://e3mag.com/wp-content/uploads/2023/12/pmf_RGB_400x400_2-150x150.png)

![avatar](https://e3mag.com/wp-content/uploads/2023/12/pmf_RGB_400x400_2.png)

## Media Discontinuities and APIs as Showstoppers

In the days before SAP BTP, ABAP developers (Business Technology Platform), had to program custom, isolated interfaces for every single AI application and every data source, which inevitably led to an uncontrollable explosion of interfaces—the infamous NxM integration problem with spiraling complexity, inconsistent security policies, and skyrocketing maintenance costs.

To this end, MCP has established a radically open, structural solution that is rightly celebrated in the global tech community as the „USB-C for AI apps.“ It standardizes the integration and tool layer and provides a unified definition of how language model-based applications (LLM clients) can securely, transparently, and dynamically access external systems, data sources, and computing cores—without having to program a separate integration for every third-party system.

## New SAP ERP Architecture by MCP

For an existing SAP customer, an MCP server fundamentally pushes the boundaries of system architecture by acting as a standardized translator and cognitive interface in front of the ERP backend.

Instead of hard-coding complex interfaces into the logic of AI agents, the ERP system makes its capabilities and data available in a controlled manner via an MCP server as predefined tools and consolidated interfaces. The higher-level AI application acts as an MCP host, recognizes the tools exposed via the server—such as retrieving a purchase order status, querying supplier ratings, or checking material inventory—and calls them up autonomously and contextually as needed for specific processes.

## Roland Berger Consulting: MCP Helps AI

The invaluable advantage of this approach is that the AI does not need to learn from a private corporate database through expensive, risky, and privacy-sensitive model training, but instead is supplied with precise, filtered live operational data in real time via the MCP server.

From the perspective of system security and data protection, this is an invaluable milestone: As an analysis by Roland Berger shows, MCP enables autonomous AI agents to request only the specific data that is absolutely necessary for the current task, which drastically minimizes the attack surface and makes compliance with strict governance requirements auditable and scalable in the first place. In addition, token consumption drops dramatically, since there is no need to funnel unnecessary mountains of data through the language models’ context windows.

## MCP Openness vs. SAP Licensing Law

However, this open architecture conflicts with the economic interests of the Walldorf-based software monopoly SAP, a fact that is painfully evident in the controversial new SAP API Policy issued in April 2026. Under the official pretext of protecting system stability and cybersecurity from uncontrolled access, SAP has significantly tightened the screws on third-party providers and existing customers.

In its notorious Section 2.2.2, the guideline explicitly prohibits any use of APIs to interact with autonomous or generative AI systems that independently plan, select, or execute sequences of API calls, unless this is done via a path approved and certified by SAP. In addition, systematic bulk data extractions to external data warehouses or data lakes such as Microsoft Fabric are prohibited.

Particularly controversial is the classification of the popular ODP-RFC interface for data integration as „prohibited use“ for third-party applications, effective as of February 2024. This poses an existential risk for existing SAP customers: SAP is attempting to establish itself as the exclusive, toll-charging gatekeeper for the company’s own data intelligence. Anyone who wants to enhance their S/4 data with superior, third-party algorithms in the dawning age of AI will be systematically blocked and forced to license the expensive and proprietary ecosystem of the Business Technology Platform (SAP BTP) and the Business Data Cloud (SAP BDC).

![](https://e3mag.com/wp-content/uploads/2026/08/e3nl26kw33_grafik-1200x670.png)

## API, BTP, and BDC Exits with the MCP Server

In this context, ERP decision-makers face the pressing question of whether SAP’s restrictive API policy can be circumvented through the skillful use of MCP servers. The answer requires a nuanced analysis of the technical and contractual realities.

From a technical standpoint, an MCP server is indeed a powerful tool for empowerment. By encapsulating standardized OData interfaces as remote MCP tools, existing customers can connect their SAP process data directly to external, superior AI platforms such as Microsoft Copilot Studio or Snowflake Cortex Agents—all while completely bypassing the often functionally immature SAP assistant Joule and avoiding costly BTP workarounds.

But the legal and business reality catches up with existing SAP customers relentlessly at this point: As integration expert Marian Zeis warns in his analyses, there is no simple, binary compliance approval from SAP. An autonomous third-party AI agent that accesses SAP data via a customer’s own MCP gateway and performs actions there unambiguously triggers the restrictive AI clauses of the API policy from a legal standpoint.

## Pitfall: SAP ERP Audits

SAP reserves the right to monitor MCP, BTP, and API access through automated audits and metering tools, and will attempt to monetize any external data flow under the controversial Digital Access licensing model as indirect use subject to high usage fees. While an MCP server thus breaks the technical vendor lock-in and prevents customers from being forced to purchase inferior SAP AI products, it does not relieve them of the contractual obligation to secure data extraction and indirect use under licensing law in order to avoid back payments in the next audit.

## Seamless ERP with MCP Server

Despite these commercial threats from SAP, a highly dynamic, self-sufficient ecosystem is developing around the Model Context Protocol, driven by SAP partners and the open-source community. SAP itself has certainly taken note of this strategic move and has made local MCP servers generally available for its own development frameworks—such as CAP, UI5, and Fiori—to provide developers with contextual AI assistance directly at the code level.

In addition, a planned MCP gateway within the SAP Integration Suite’s API management is being proposed to connect legacy systems—however, this is not yet widely implemented and is primarily intended to restrict access exclusively to Joule agents. The actual, immediately usable innovation is therefore coming from established third-party providers.

## Observability for LLMs via MCP

With the Trento MCP Server, European open-source pioneer SUSE offers a highly secure solution that makes real-time observability data from the SAP infrastructure available to any LLM without requiring confidential operational data to leave the company. Theobald Software provides specialized MCP servers that establish a reliable and secure direct connection between external AI agents and SAP table structures, which is essential for data consistency in the ERP environment. Archiving specialist KGS also uses the protocol to leverage audit-compliant document archives as semantically rich context providers for AI systems. In the open-source developer community, it is primarily thought leaders such as Marian Zeis and Alice Vinogradova who are paving the way with open-source ABAP-MCP servers to seamlessly integrate S/4 HANA and classic ECC 6.0 systems with modern AI platforms.

## **Conclusion: I can't do without my MCP server**

The conclusion for existing SAP customers is this: Artificial intelligence—and, in particular, the era of Agentic AI—absolutely requires the Model Context Protocol as a universal connection interface in order to have any reason to exist in a business-critical ERP environment.

An ERP system like SAP S/4 HANA is and remains the indispensable, stable anchor for data quality, industry knowledge, and process logic in every company. However, this valuable knowledge remains isolated and rigid unless it is brought to life by the flexible, cognitive capabilities of modern AI models. Conversely, pure language models—without the precise, structured business context of an ERP system—are prone to dangerous hallucinations and are completely blind to day-to-day operations.

MCP is the crucial link that seamlessly, securely, and vendor-independently merges the two worlds. For ERP decision-makers, the path to artificial intelligence must therefore never lead through SAP’s exclusive, overpriced cloud solutions. Anyone who wants to preserve their business freedom must opt for an open, composable ERP concept (Composable ERP), in which the SAP system remains the transactional backend, while AI orchestration is managed via standardized MCP interfaces and vendor-neutral integration platforms.

![avatar](https://e3mag.com/wp-content/uploads/2023/12/pmf_RGB_400x400_2.png)

Peter M. Färbinger, E3 Magazine

Peter M. Färbinger, Publisher and Editor-in-Chief of E3 Magazine DE, US, ES, and FR (e3mag.com), B4Bmedia.net AG, Freilassing (DE), email: pmf@b4bmedia.net, and phone: +49(0)8654/77130-21

[All articles of the author](https://e3mag.com/en/author/peter-m-faerbinger-e-3-magazin/)

#### Write a comment [(Cancel Reply)](https://e3mag.com/en/sap-erp-exit-mit-model-context-protocol/\#respond)

## [Study: State of FinOps 26](https://e3mag.com/en/studie-state-of-finops-26/)

[![](https://e3mag.com/wp-content/uploads/2026/07/2607_sz_deutsche_telekom_bundesministerium.jpg)](https://e3mag.com/en/the-backbone-of-digital-government-a-sovereign-ai-platform-for-the-federal-government/)

## [The Backbone of Digital Government: A Sovereign AI Platform for the Federal Government](https://e3mag.com/en/the-backbone-of-digital-government-a-sovereign-ai-platform-for-the-federal-government/)

## [Integrated HR and ERP Systems: Data-Driven Control Centers](https://e3mag.com/en/integrierte-hr-und-erp-systeme-datengetriebene-steuerungszentren/)

We've detected you might be speaking a different language. Do you want to change to:

![de_DE](https://e3mag.com/wp-content/plugins/translatepress-multilingual/assets/images/flags/de_DE.png) DE

![de_DE](https://e3mag.com/wp-content/plugins/translatepress-multilingual/assets/images/flags/de_DE.png) DE

![en_US](https://e3mag.com/wp-content/plugins/translatepress-multilingual/assets/images/flags/en_US.png) EN

![es_ES](https://e3mag.com/wp-content/plugins/translatepress-multilingual/assets/images/flags/es_ES.png) ES

![fr_FR](https://e3mag.com/wp-content/plugins/translatepress-multilingual/assets/images/flags/fr_FR.png) FR

[Change Language](https://e3mag.com/)

[Close and do not switch language](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/#)

We've detected you might be speaking a different language. Do you want to change to:

![de_DE](https://e3mag.com/wp-content/plugins/translatepress-multilingual/assets/images/flags/de_DE.png) DE

![de_DE](https://e3mag.com/wp-content/plugins/translatepress-multilingual/assets/images/flags/de_DE.png) DE

![en_US](https://e3mag.com/wp-content/plugins/translatepress-multilingual/assets/images/flags/en_US.png) EN


![es_ES](https://e3mag.com/wp-content/plugins/translatepress-multilingual/assets/images/flags/es_ES.png) ES


![fr_FR](https://e3mag.com/wp-content/plugins/translatepress-multilingual/assets/images/flags/fr_FR.png) FR


[Change Language](https://e3mag.com/)

[![](https://e3mag.com/wp-content/uploads/2025/06/ccs_logo_26.png)](https://e3mag.com/en/cc-summit-en/)

Working on the SAP basis is crucial for successful S/4 conversion.

This gives the Competence Center strategic importance for existing SAP customers. Regardless of the S/4 Hana operating model, topics such as **Automation**, **Monitoring**, **Security**, **Application Lifecycle Management** and **Data Management** the basis for S/4 operations.

For the fourth time, E3 magazine is organizing a summit for the SAP community in Salzburg to provide comprehensive information on all aspects of S/4 Hana groundwork.

### Venue

**FourSide Hotel Salzburg**,

Trademark Collection by Wyndham

Am Messezentrum 2, 5020 Salzburg, Austria

+43-662-4355460

### Event date

Wednesday, June 10, and

Thursday, June 11, 2026

**AI experience workshop only** on June 11, 2026 (limited places)

**Bonus:** Access to all lectures on June 11, 2026

### Regular ticket

Lectures, evening event and, depending on availability, the AI workshop on June 11, 2026

Places at the AI experience workshop are limited and registration is required.

### Subscribers to the E3 Magazine Ticket

reduced with promocode CCAbo26

### Students\*

reduced with promocode CCStud26.

Please send proof of studies by e-mail to office@b4bmedia.net.

\*The first 10 tickets are free of charge for students. Try your luck! 🍀

**EUR 305 excl. VAT.**

**EUR 590 excl. VAT**

**EUR 390 excl. VAT**

**EUR 290 excl. VAT**

### **Registration form**

Which services would you like to book?**\***Select...AI experience workshop onlyRegular ticket

This field is required.

Would you like to take part in the AI experience workshop? (Subject to availability - limited places)Select...YesNo

This field is required.

Participation in the evening event**\***Select ...YesNo

This field is mandatory.

Salutation**\***Select ...Ms.Mr.not specified

This field is required.

Academic degreeSelect ...Dr.Prof.Prof. Dr.Mag.

This field is required.

First name participant**\***

This field is mandatory.

Name of participant**\***

This field is mandatory.

Company**\***

This field is mandatory.

Job title**\***

This field is required.

Department**\***Select ...MarketingFinances/ControllingManagementInsurance/ClaimsIT/EDPOperations/BusinessHuman ResourcesProduction/Planning/QMOther

This field is required.

Branch**\***Select ...Construction industryConstruction industry, plant engineering and shipbuildingChemistry & PharmaServices (IT)Service industryEnergy & SupplyFinancial sectorHealthcareTradeReal EstateConsumer goodsMachine, device and component constructionMedia industryMetal, machinery, and plant engineeringMetal processingPublic administrationOther

This field is required.

E-mail address participant**\***

This field is mandatory.

The following query on the age group is purely for statistical purposes. We kindly ask you to provide this information voluntarily.

Age groupSelect ...18-3030-4546-6060+Not specified

This field is required.

[Add line](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/# "Add line")[Remove line](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/# "Remove line")

* * *

Billing address:

Salutation**\***Select ...Ms.Mr.not specified

This field is required.

Academic degreeSelect ...Dr.Prof.Prof. Dr.Mag.

This field is required.

First name customer**\***

This field is mandatory.

Last name customer**\***

This field is mandatory.

Company**\***

This field is mandatory.

Street**\***

This field is mandatory.

House number**\***

This field is mandatory.

ZIP Code**\***

This field is mandatory.

Location**\***

This field is mandatory.

E-mail address of purchaser**\***

This field is mandatory.

If you enter your e-mail address here, your invoice will only be sent by e-mail to the specified address after the event.

E-mail address for invoicing via PDF:

This field is mandatory.

VAT ID**\***

This field is mandatory.

According to tax law, company names in invoices must be correct. The data you enter will be used for invoicing.

Department / Contact person

This field is mandatory.

PO number

This field is mandatory.

Promo code

This field is required.

Would you like to share any other important information with us?

This field is required.

I accept the terms and conditions, expressly consent to the processing of my data in accordance with the GDPR, and authorize its use for the purpose of contacting me. // Privacy Policy – Cookie Policy**\***

This field is mandatory.

This field is mandatory.

In accordance with the GDPR, I consent to receiving further information about the CC Summit from E3 Magazine and partners.**\***

This field is mandatory.

This field is mandatory.

Note: In the event of photo, TV, and video recordings by the publisher B4Bmedia.net AG (E3 Magazine) or by authorized third parties (e.g., participants in E3 events), visitors/participants agree to the possible recording of images of themselves and the associated use of such images (social media, YouTube, web, etc.).

reCAPTCHA

Recaptcha requires verification.

I'm not a robot

reCAPTCHA

This field is required.

Submit

[![](https://e3mag.com/wp-content/uploads/2025/03/steampunk_brown_2026.png)](https://e3mag.com/en/steampunk-summit-en/)

### Venue

Hotel Hilton Heidelberg

Kurfürstenanlage 1

D-69115 Heidelberg

### Event date

Wednesday, April 22 and

Thursday, April 23, 2026

### Tickets

**AI only** **Experience workshop** on April 23, 2026

**Bonus**: Access to all lectures on April 23, 2026

**Regular ticket**

April 22, 2026: Lectures and evening event

April 23, 2026: Lectures and AI workshop

**EUR 305 excl. VAT**

**EUR 590 excl. VAT**

**Subscribers to the E3 magazine**

reduced with promocode STAbo26

**EUR 390 excl. VAT**

**Students\***

reduced with promocode STStud26.

Please send proof of studies by e-mail to office@b4bmedia.net.

**EUR 290 excl. VAT**

\*The first 10 tickets are free of charge for students. Try your luck! 🍀

The event is organized by the E3 magazine of the publishing house B4Bmedia.net AG. The presentations will be accompanied by an exhibition of selected SAP partners. The ticket price includes attendance at all presentations of the Steampunk and BTP Summit 2026, a visit to the exhibition area, participation in the evening event and catering during the official program. The lecture program and the list of exhibitors and sponsors (SAP partners) will be published on this website in due course.

### **Registration form**

Which services would you like to book?**\***Select...Regular ticketAI experience workshop only

This field is required.

Participation in the evening event**\***Select ...YesNo

This field is mandatory.

Salutation**\***Select ...Ms.Mr.not specified

This field is required.

Academic degreeSelect ...Dr.Prof.Prof. Dr.Mag.

This field is required.

First name participant**\***

This field is mandatory.

Name of participant**\***

This field is mandatory.

Company**\***

This field is mandatory.

Job title**\***

This field is required.

Department**\***Select ...MarketingFinances/ControllingManagementInsurance/ClaimsIT/EDPOperations/BusinessHuman ResourcesProduction/Planning/QMOther

This field is required.

Branch**\***Select ...Construction industryConstruction industry, plant engineering and shipbuildingChemistry & PharmaServices (IT)Service industryEnergy & SupplyFinancial sectorHealthcareTradeReal EstateConsumer goodsMachine, device and component constructionMedia industryMetal, mechanical and plant engineeringMetal processingPublic administrationOther

This field is required.

E-mail address participant**\***

This field is mandatory.

The following query on the age group is purely for statistical purposes. We kindly ask you to provide this information voluntarily.

Age groupSelect ...18-3030-4546-6060+Not specified

This field is required.

[Add line](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/# "Add line")[Remove line](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/# "Remove line")

* * *

Billing address:

Salutation**\***Select ...Ms.Mr.not specified

This field is required.

Academic degreeSelect ...Dr.Prof.Prof. Dr.Mag.

This field is required.

First name customer**\***

This field is mandatory.

Last name customer**\***

This field is mandatory.

Company**\***

This field is mandatory.

Street**\***

This field is mandatory.

House number**\***

This field is mandatory.

ZIP Code**\***

This field is mandatory.

Location**\***

This field is mandatory.

E-mail address of purchaser**\***

This field is mandatory.

If you enter your e-mail address here, your invoice will only be sent by e-mail to the specified address after the event.

E-mail address for invoicing via PDF:

This field is mandatory.

VAT ID**\***

This field is mandatory.

According to tax law, company names in invoices must be correct. The data you enter will be used for invoicing.

Department / Contact person

This field is mandatory.

PO number

This field is mandatory.

Promo code

This field is required.

Would you like to share any other important information with us?

This field is required.

I accept the terms and conditions, expressly consent to the processing of my data in accordance with the GDPR, and authorize its use for the purpose of contacting me. // Privacy Policy – Cookie Policy**\***

This field is mandatory.

This field is mandatory.

In accordance with the GDPR, I agree to receive further information about the Steampunk Summit from E3 Magazine and partners.**\***

This field is mandatory.

This field is mandatory.

Note: In the event of photo, TV, and video recordings by the publisher B4Bmedia.net AG (E3 Magazine) or by authorized third parties (e.g., participants in E3 events), visitors/participants agree to the possible recording of images of themselves and the associated use of such images (social media, YouTube, web, etc.).

Submit

![](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/)

![](https://e3mag.com/en/sap-erp-exit-with-model-context-protocol/)

reCAPTCHA