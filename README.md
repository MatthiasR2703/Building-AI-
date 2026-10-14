# KommunalFund AI

Building AI course project

## Summary

KommunalFund AI is an AI-based recommendation system that helps municipalities identify suitable public funding programmes for local projects. It matches project descriptions with relevant funding opportunities and ranks them according to their likely suitability.

## Background

Municipalities in Germany can access a large number of funding programmes offered by the federal government, the Länder and the European Union. These programmes can support projects in areas such as digitalisation, climate protection, infrastructure, mobility, education or urban development.

The problem is that finding the right programme can be difficult and time-consuming. Funding opportunities are published by many different institutions, use different terminology and often contain complex eligibility requirements.

Smaller municipalities in particular may not have specialised staff who continuously monitor funding programmes. As a result, suitable funding opportunities may be discovered too late or not at all.

My motivation for this project comes from practical experience in municipal administration. During my work in local government, identifying suitable funding programmes and evaluating whether they fit a planned project was a recurring task.

KommunalFund AI aims to make this process faster and more accessible.

The project would address problems such as:

* large numbers of funding programmes from different institutions
* complex and inconsistent programme descriptions
* limited administrative resources in smaller municipalities
* difficulties matching municipal projects with funding criteria
* deadlines that may be overlooked

## How is it used?

A municipal employee enters a short description of a planned project.

For example:

> "The municipality wants to renovate a public primary school, improve its energy efficiency, install solar panels and replace the heating system."

The system analyses the project description and compares it with available funding programmes.

The user would then receive a ranked list of potentially suitable programmes.

An example result could look like this:

1. Energy-efficient renovation of public buildings – high match
2. Municipal climate protection programme – high match
3. Renewable energy investment programme – medium match
4. General infrastructure programme – low match

For each recommendation, the system could also display:

* funding authority
* eligible applicants
* funding rate
* maximum funding amount
* application deadline
* relevant programme requirements
* a short explanation of why the programme matches the project

The system would not make the final decision. Municipal employees would still verify the original funding guidelines before submitting an application.

## Data sources and AI methods

The system would mainly use publicly available information from official funding institutions.

Possible data sources include:

* funding databases of the German federal government
* funding programmes of the German Länder
* EU funding programmes
* development banks such as KfW
* state development banks
* official programme guidelines and funding documents

Each funding programme could be represented through features such as:

* programme description
* target group
* eligible project types
* geographical area
* funding amount
* funding percentage
* application deadline
* keywords and thematic categories

Natural Language Processing could be used to analyse both municipal project descriptions and programme descriptions.

A simple first version could use a bag-of-words or TF-IDF representation and calculate the similarity between the project description and funding programme descriptions.

More advanced versions could use semantic text embeddings to identify programmes even when different terminology is used.

The system could combine AI methods with rule-based filtering.

For example:

1. Remove programmes for which municipalities are not eligible.
2. Remove programmes outside the relevant geographical region.
3. Remove programmes whose deadlines have passed.
4. Calculate the semantic similarity between the project description and the remaining programmes.
5. Rank the programmes according to their relevance.

This combination of rules and machine learning could improve both accuracy and transparency.

## Challenges

KommunalFund AI would have several limitations.

The most important challenge is data quality. Funding programmes change frequently and deadlines, requirements and funding amounts may be updated.

Another challenge is that programme guidelines can contain complex legal and administrative requirements that cannot always be captured reliably by an automated system.

A high similarity score does not necessarily mean that a project is actually eligible for funding.

For this reason, the system should never replace professional or legal assessment. It should function as a decision-support and research tool.

Further challenges include:

* incomplete or outdated programme information
* different terminology used by funding institutions
* interpretation of complex eligibility rules
* regional differences between funding programmes
* potential errors in automatically generated recommendations

Transparency would therefore be important. The system should explain why a programme was recommended and always provide a link to the official programme documentation.

## What next?

A first prototype could focus on one German federal state and a limited number of funding programmes.

For example, the system could initially analyse funding programmes available to municipalities in Hesse.

After evaluating the quality of the recommendations, additional programme databases could be added.

Future versions could include:

* automatic monitoring of new funding programmes
* notifications when suitable programmes become available
* deadline monitoring
* automatic extraction of eligibility criteria from programme documents
* comparison of several funding options
* personalised profiles for municipalities
* integration with municipal project management systems
* automatic generation of funding programme shortlists

A more advanced system could also learn from previous successful applications. If municipalities voluntarily shared anonymised information about funded projects, the model could identify patterns between projects and successful funding programmes.

The long-term goal would be a digital assistant that helps municipalities identify funding opportunities earlier and use public funding more efficiently.

## Acknowledgments

This project idea was developed as part of the Building AI course by the University of Helsinki and Reaktor.

The concept is inspired by practical experience in municipal administration and by the difficulties municipalities face when identifying suitable public funding programmes.

Any future implementation would use only data and documents that may legally be processed and reused. Official funding programme information would always be linked to its original source.
