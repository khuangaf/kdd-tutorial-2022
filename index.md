#### The Battlefront of Combating Misinformation and Coping with Media Bias

## Schedule
August 14, 2022 (Tutorial time TBD)

## Abstract

The growth of online platforms has greatly facilitated the way people communicate with each other and stay informed about trending events. However, it has also spawned unprecedented levels of inaccurate or misleading information, as traditional journalism gate-keeping fails to keep up with the pace of media dissemination. These undesirable phenomena have caused societies to be torn over irrational beliefs, money lost from impulsive stock market moves, and deaths occurred that could have been avoided during the COVID-19 pandemic, due to the infodemic that came forth with it, etc. Even people who do not believe the misinformation may still be plagued by the pollution of unhealthy content surrounding them, an unpleasant situation known as information disorder. Thus, it is of pertinent interest for our community to better understand, and to develop effective mechanisms for remedying, misinformation and biased reporting.

## Target Audience and Prerequisites
Based on the level of interest in this topic, we expect around 150 participants. While no specific background knowledge is assumed of the audience, it would be best for the attendees to know basic deep learning, pre-trained word embeddings (e.g., Word2Vec) and language models (e.g.,BERT).

## Outline
### Background and Motivation
We begin motivating the tutorial topic with a selection of real-world examples of fake news and their harmful impacts to society, followed by a pedagogical exercise of how humans tend to approach the problem of fake news detection, characterization, and correction. We will point out conceptual distinctions amongst various types of fake news, including serious fabrication in news journalism about misattributed or nonexisting events, over-sensationalized clickbaits, hoaxes which are false with the intention to be picked up by traditional news websites and satire which mimic genuine news but contain irony and absurdity. For example, in general, news articles more likely involve serious fabrications, while social media posts involve more humour such as satire and hoaxes. We will also describe the cognitive, social and affective factors that lead people to form or endorse misinformed views (e.g., intuitive thinking, illusory truths, source cues, emotions, etc.), and the psychological barriers to knowledge revision after misinformation has been corrected, including correction not integrated, selective retrieval, and continued influence theories. 

### Fake News Detection (60min)

Bearing in mind the different categories and psychological drivers of misinformation, we introduce detection based on:


* **stylistic** approaches that focus on lexical features, readability, and syntactic clues.
* **fact-checking** approaches that compare check-worthy content with background knowledge, such as external knowledge bases (FreeBase, WikiBase, etc) and previously fact-checked claims.
* **semantic-consistency** approaches that extract features related to single-document discourse-level coherence and cross-document event-centric coherence in text. Extending to cross-media domain, the common strategy is to check text-image consistency and text-video consistency
* **propagation patterns** that capture confounding factors from the dynamics of how a news topic spreads and the social network interactions . 


We will discuss the merits and the limitations of these different lines of fake news detection approaches. For example, fact-checking approaches may not fare well for early rumours or breaking news not yet groundable to an established background knowledge, in which case, the credibility of the news source can offer complementary assistance. Stylistic approaches may be simple but yet effective for detecting low-quality human-written fake news, but not so good for machine-generated misinformation, which is stylistically consistent regardless of the underlying motives.
We then cover recent approaches that leverage a combination of these elements for greater representation power and robustness. Importantly, we also cover works that explore the diachronic bias of fake news detection and portability across data in different time and language settings.


#### Special Note on Neural Fake News Generation & Detection:
Advancements in natural language generation spawn the rise of news generation models which represent a double-edged sword. On one hand, malicious actors may irresponsibility take advantage of the technology to influence opinions and gain revenue. But, on the other hand, it can also be used as
a source of machine-synthesized  training data for detector models to overcome data scarcity since real-world fake news tends to be eventually removed by platforms, as well as a tool for threat modeling to develop proactive defenses against potential threats. We review how popular detectors perform on fake news created from large-scale language and vision generator model. We also review progress in generating fake news that better aligns with the key topic and facts, and work towards applying topic/fact-constrained fake news generation to construct silver-standard data annotations for finer-grained fake news detection.

### Fake News Characterization (30min)
To better understand and fight fake news, we next address some fundamental questions of characterizing fake news based on underlying source bias, reporting agenda, propaganda techniques, and target audience. First, we introduce modeling approaches for detecting political and socio-cultural biases in news articles. Next, we introduce the recent EMU benchmark that require models to answer open-ended questions capturing the intent and the implications of a media edit. We cover methodologies for identifying the specific propaganda techniques used, e.g., _smears_, _glittering generalities_, _association transfer_, etc. We also discuss the latest explorations in predicting the intended target of harmful media content, e.g., the person, the organization, the community, or the society level. 

### Corrective Actions for Misinformation and Biased News Reporting (30min)
After misinformation has been detected and categorized based on its various characteristics, there is naturally follow-up interest in corrective explanations on why a piece of information is fake or misleading, and how to report less biased and more comprehensive news in general. Hence, we cover frameworks for explaining why a given piece of news is actually fake news through the leverage of reader comments, as well as appropriate strategies for placing the corrective explanations based on user studies. We also cover research on mitigating media bias, such as through neutral article generation.


#### Industry Initiatives:
We further point out recent actions by tech companies with media-hosting platforms for fighting fake news. With urges from the government, they experiment with removing economic incentives for traffickers of misinformation, promoting media literacy, suspending improper posts and accounts, and adding colored labels, with corrections constructed from a community-based point system similar to Wikipedia, directly beneath misinformation posted by public figures (https://www.nbcnews.com/tech/tech-news/twitter-testing-new-ways-fight-misinformation-including-community-based-points-n1139931).


### Concluding Remarks & Future Directions (30min)
Finally, we summarize the major remaining challenges in this space, including the detection of subtle inconsistencies, enforcing schema or logical constraints in the detection, identifying semantically consistent but misattributed cross-media pairings, and greater precision in fine-grained explanations for the detected misinformation.

## Tutors
<img align="left" src="images/yi.png" width="180" > **Yi R. Fung** is a second-year Ph.D. student at the Computer Science Department of UIUC, with research interests in knowledge reasoning, misinformation detection, and computation for the social good. Her recent works include the InfoSurgeon fake news detection framework, and multiview news summarization. Yi is a recipient of the NAACL'21 Best Demo Paper, the UIUC Lauslen and Andrew fellowship, and the National Association of Asian American Professionals Future Leaders award. She has also been previously selected for invited talk (1 hour presentation) at the Harvard Medical School Bioinformatics Seminar. Additional information is available at [https://yrf1.github.io](https://yrf1.github.io).


<img align="left" src="images/kung-hsiang.jpeg" width="180" > **Kung-Hsiang Huang** is a first-year Ph.D. student at the Computer Science Department of UIUC. His research focuses on fact-checking and fake news detection. Prior to joining UIUC, he obtained his B.Eng. in Computer Science from the Hong Kong University of Science and Technology, and his M.S. in Computer Science from USC. He is also a co-founder of an AI startup, Rosetta.ai. Additional information is available at [https://khuangaf.github.io](https://khuangaf.github.io).


<img align="left" src="images/preslav.png" width="180" > **Preslav Nakov** is a Principal Scientist at the Qatar Computing Research Institute (QCRI), HBKU, who received his PhD degree from the University of California at Berkeley (supported by a Fulbright grant). Dr. Nakov is President of ACL SIGLEX, Secretary of ACL SIGSLAV, a member of the EACL advisory board, as well as a member of the editorial board of Computational Linguistics, TACL, CS&L, IEEE TAC, NLE, AI Communications, and Frontiers in AI. His research on fake news was featured by over 100 news outlets, including Forbes, Boston Globe, Aljazeera, MIT Technology Review, Science Daily, Popular Science, The Register, WIRED, and Engadget, among others. He has driven relevant tutorials such as:

* WSDM’22: Fact-Checking, Fake News, Propaganda, Media Bias, and the COVID-19 Infodemic.
* CIKM'21: Fake News, Disinformation, Propaganda, and Media Bias.
* EMNLP'20: Fact-Checking, Fake News, Propaganda, and Media Bias: Truth Seeking in the Post-Truth Era.

Additional information is available at [https://en.wikipedia.org/wiki/Preslav_Nakov](https://en.wikipedia.org/wiki/Preslav_Nakov).


<img align="left" src="images/heng.JPG" width="180" > **Heng Ji**  is a Professor at the Computer Science Department of the University of Illinois Urbana-Champaign, and an Amazon Scholar. Her research interests focus on NLP, especially on Multimedia Multilingual Information Extraction, Knowledge Base Population and Knowledge-driven Generation. She was selected as ``Young Scientist'' and a member of the Global Future Council on the Future of Computing by the World Economic Forum. The awards she received include ``AI's 10 to Watch'' Award, NSF CAREER award, Google Research Award, IBM Watson Faculty Award, Bosch Research Award, Amazon AWS Award, ACL2020 Best Demo Paper Award, and NAACL2021 Best Demo Paper Award. She has given a large number of keynotes and 20 tutorials on Information Extraction, Natural Language Understanding, and Knowledge Base Construction in many conferences including but not limited to ACL, EMNLP, NAACL, NeurIPS, AAAI, SIGIR, WWW, IJCAI, COLING and KDD. A selected handful of her recent tutorials include:

* AAAI’22: Deep Learning on Graphs for Natural Language Processing.
* EMNLP’21: Knowledge-Enriched Natural Language Generation.
* ACL’21: Event-Centric Natural Language Processing.

Additional information is available at [https://blender.cs.illinois.edu/hengji.html](https://blender.cs.illinois.edu/hengji.html).

For more information about this tutorial, please refer to our [proposal](#)
