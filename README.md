# HUMN250-TeenageDecisions
---
# For reference on dataset card metadata, see the spec: https://github.com/huggingface/hub-docs/blob/main/datasetcard.md?plain=1
# Doc / guide: https://huggingface.co/docs/hub/datasets-cards
{{ card_data }}
---

# Dataset Card for {{ pretty_name | default("Teenage Online Decisions", true) }}

<!-- Provide a quick summary of the dataset. -->

{{ dataset_summary | default("This dataset is comprised of synthetic data from teenagers actions on social media for a given post. Actions include sharing, commenting, and liking a post.", true) }}

## Dataset Details

### Dataset Description

<!-- Provide a longer summary of what this dataset is. -->

{{ dataset_description | default("This dataset is formed from actions teenagers make when introduced to different online posts. Posts are all text-based and include emojis and hashtags. The number of teenagers within the range of 1000 who liked, commented, and shared the post are recorded next to the post itself. This dataset contains 131 entries of synthesized data from ChatGPT 3.5. The data is unfiltered, but checked for repetition and spelling.", true) }}

- **Curated by:** {{ curators | default("Noah Medrano", true)}}
- **Funded by [optional]:** {{ funded_by | default("Noah Medrano", true)}}
- **Language(s) (NLP):** {{ language | default("en", true)}}
- **License:** {{ license | default("unlicensed", true)}}

### Dataset Sources [optional]

<!-- Provide the basic links for the dataset. -->

- **Repository:** {{ repo | default("https://github.com/nlmed/HUMN250-TeenageDecisions/", true)}}
- **Paper [optional]:** {{ paper | default("No Information: No Paper. Some questions I would ask if there were no sources: Where was the source for data? In what forms were the data presented? Who created the source, and are they credible sources to gather information from? I would direct these questions to the creator of the data-set repository on the site where I found it.", true)}}

## Uses

<!-- Address questions around how the dataset is intended to be used. -->

### Direct Use

<!-- This section describes suitable use cases for the dataset. -->

{{ direct_use | default("This dataset is used to understand the content that best aligns with the ideas, humor, and personalities of teenagers online in the year 2024. This dataset is best suited for programs to show similar-age individuals content that is relevant to them. This may be used in AI domains that learn about the teenage culture to improve current systems geared towards them and their needs. Machine-learning algorithms for understanding what types of posts a teenage user would like to see may be in the scope of this dataset. Other AI applications like assisting in formulating ideas for advertisements for younger-aged individuals may also be in the scope of this dataset.", true)}}

### Out-of-Scope Use

<!-- This section addresses misuse, malicious use, and uses that the dataset will not work well for. -->

{{ out_of_scope_use | default("This dataset is not to be used in instances of phishing, scamming, or any technological form of malice towards other individuals that would result in potential physical or mental harm. This data will not work for understanding other ages such as middle age adults or children. This dataset will not work for determining what is best for specific demographics within teenagers, such as race or sex.", true)}}

## Dataset Structure

<!-- This section provides a description of the dataset fields, and additional information about the dataset structure such as criteria used to create the splits, relationships between data points, etc. -->

{{ dataset_structure | default("Each row in the dataset refers to a singular post and contains the following:
  Post: The body and main content of the post.
  Likes: The number of teenagers who liked the post.
  Shares: The number of teenagers who shared the post with another individual.
  Comments: The number of teenagers who left a comment on the post.
  
  The data in this set is not split.", true)}}

## Dataset Creation

### Curation Rationale

<!-- Motivation for the creation of this dataset. -->

{{ curation_rationale_section | default("The motivation for collecting and organizing this data is to further understand the teenage mind when interacting with both the digital world and others when online. Often, individuals will make different decisions online than in person, which may result in cyberbullying or acts of violence. Understanding these trends and motives behind decisions would help to form a better system of online use for teenagers.", true)}}

### Source Data

<!-- This section describes the source data (e.g. news text and headlines, social media posts, translated sentences, ...). -->

#### Data Collection and Processing

<!-- This section describes the data collection and processing process such as data selection criteria, filtering and normalization methods, tools and libraries used, etc. -->

{{ data_collection_and_processing_section | default("Data was collected directly from AI, when given criteria about posts and the distribution of likes, shares, and comments on the post. Criteria for data were that it was relevant to the teenage experience, intriguing to read, and clear and concise. The topics for posts include school, work, fashion, makeup, and pop culture.", true)}}

#### Who are the source data producers?

<!-- This section describes the people or systems who originally created the data. It should also include self-reported demographic or identity information for the source data creators if this information is available. -->

{{ source_data_producers_section | default("This dataset comprises of synthetic data gathered from ChatGPT 3.5. The posts come from a formula to discuss school, work, fashion, makeup, and pop culture. Posts are to be engaging and relevant to average teenagers in 2024. Data was taken directly and put into a readable format in .CSV.", true)}}

### Annotations [optional]

<!-- If the dataset contains annotations which are not part of the initial data collection, use this section to describe them. -->

#### Annotation process

<!-- This section describes the annotation process such as annotation tools used in the process, the amount of data annotated, annotation guidelines provided to the annotators, interannotator statistics, annotation validation, etc. -->

{{ annotation_process_section | default("No Information: No annotations were made to this data. This is something that should be done though to keep in line with data audits. I would ask questions to see how and why some data was annotated. This would further help me understand the legitimacy of the data, and it would give me more viewpoints to look at when analyzing the data.", true)}}

#### Who are the annotators?

<!-- This section describes the people or systems who created the annotations. -->

{{ who_are_annotators_section | default("No Information: No authors, with no annotations. I would likely ask about the credibility of these annotators, and question their claims, as I would question the data. This would allow me to both analyze who is reviewing the data and the validity of the data presented in the dataset.", true)}}

#### Personal and Sensitive Information

<!-- State whether the dataset contains data that might be considered personal, sensitive, or private (e.g., data that reveals addresses, uniquely identifiable names or aliases, racial or ethnic origins, sexual orientations, religious beliefs, political opinions, financial or health data, etc.). If efforts were made to anonymize the data, describe the anonymization process. -->

{{ personal_and_sensitive_information | default("All data within this dataset is synthetic, and is not from real social media sources. There is no recording of authors of posts, nor personal information about the teenagers within the data. No identifying information about race, sex, or sexual orientation is mentioned in the data to prevent biases. All fields are anonymous.", true)}}

## Bias, Risks, and Limitations

<!-- This section is meant to convey both technical and sociotechnical limitations. -->

{{ bias_risks_limitations | default("There are several limitations within the data here including lack of information regarding students, specific comments, and sample size. Students do not have relevant information such as demographical data to help support why they may have liked or disliked a post. Although comments do mean teens engaged with the post, it is not known if there was positive or negative engagement. Negative comments would mean that the teenager did not like the content, but the data will not reflect such actions. There is also a limited sample size of 131, which may not be reflective of all individuals.", true)}}

### Recommendations

<!-- This section is meant to convey recommendations with respect to the bias, risk, and technical limitations. -->

{{ bias_recommendations | default("Users should be made aware of the risks, biases and limitations of the dataset. More information needed for further recommendations.", true)}}

## Citation [optional]

<!-- If there is a paper or blog post introducing the dataset, the APA and Bibtex information for that should go in this section. -->

**BibTeX:**

{{ citation_bibtex | default("No Information: There is no citation for this. Questions I would ask: In what field of work was this introduced? Is it different from the applications that the data is currently being used for? If the introduction of this dataset comes from academia, are there any challenges to the claims that this dataset supports? Do the questions stem from the data itself, or the applications of it? How do we ensure that this data is still relevant to this day? These questions would likely be questions I would try to answer by doing further research, or by looking in the text itself.", true)}}

