# References
## 1. Greenstein, Shane, and Feng Zhu. “Is Wikipedia Biased?” American Economic Review 102.3 (2012): 343–348.

- Context
- Describes the terms of the general problem
- Defines the general problem
- Summarizes the approach
- Presents the results
- Frames the topic in more detail
    - How does Wikipedia aggregate new information?
- Figures and deductions
- Conclusion

A **“Neutral Point of View”** (NPOV) is one of the tenets that all Wikipedia articles aspire to achieve, along with “verifiability” and “the absence of original research”.

The conflicting opinions are presented next to one another with all significant points of view represented.

Verified information: many sources state the information.

Study that measures the slant at a point in time within a sample of 28 thousand entries about U.S. political topics. It documents its evolution over time.

**Result**: Wikipedia contains a bias and the level or direction of bias is not fixed over time. The overall slant changes mainly due to the entry of articles with opposite slants. The revision of existing articles reduces only moderately their initial slant.

Wikipedia uses a commons-based approach to aggregate information from a widely dispersed set of contributors and is oriented toward the production of non-proprietary information.

**Fields**: media content bias

Wikipedia’s editors are instructed to “assert facts, including facts about opinions – but do not assert the opinions themselves”.

**Problem studied**: Examines the bias of Wikipedia on political topics.

**Approach (high-level)**: Retrieve articles that focus on a broad and inclusive definition of U.S. political topics. Then ask whether a given article uses phrases favored more by Republican members or by Democratic members of Congress.

- First, examine the latest version of each article and select all articles with keywords “republican” or “democrat”.

- Then, eliminate articles that cover countries other than the U.S. The article can argue about the Iraq war but does not relate to political parties in foreign countries.

- For each article, construct a slant index by applying the G&S (Gentzkow and Shapiro) method. Articles with a slant index below 0.49 are left-leaning and articles with a slant index above 0.49 are right-leaning.

    - Select 1,000 phrases based on the number of times these phrases appear in the 2005 Congressional Record.

    - Apply statistical methods to identify phrases that separate Democratic representatives from Republican representatives.

**Key results:**

- Topics of articles show considerable variance of the observed slant mean (between -0.16 and 0.06), and some seemingly controversial topics are centered at zero (mean). Explaining such variance is another open question.

- Wikipedia is left-leaning biased. Indeed, -0.09 implies Democrat-leaning.

- The average old political article in Wikipedia leans Democratic. The number of recent articles far outweighs the number of older articles, so by the last date, Wikipedia’s articles appear to be centered close to a middle point on average. There is a weak tendency for articles to become less biased over time after revision. The overall change arises from the entry of later vintages of articles with an opposite point of view from earlier articles.

**Limitations:**

- This research does not seem to take into account the cognitive biases of authors who have personal political opinions. We therefore do not know, among the authors, whether the majority votes left and whether this explains Wikipedia’s left-leaning bias.

- The G&S method provides a statistical benchmark to measure the slant of an article. Compared to its application to newspapers, the measure cannot be compared with external sources, given that there is no equivalent to Wikipedia.

- Wikipedia articles contain far fewer sentences than newspaper articles.

**Open questions:**

- Explaining the variance of the observed slant.

- Causality: do more or fewer revisions of an article cause the article to contain lower or greater slant? Does lower or greater slant cause articles to receive more or less attention?

**Personal analysis:**

- The choice of the analysis context, “political topics”, maximizes the chances of observing divergences of opinion given that it is a highly controversial subject.

- Moreover, the article dates from 2012: are its conclusions still valid today?

## 2. Yasseri, Taha, and Saeedeh Mohammadi. “How Similar Are Grokipedia and Wikipedia? A Multi-Dimensional Textual and Structural Comparison.” arXiv preprint arXiv:2510.26899 (2025).

- Abstract
- Vocabulary and context
- State of the art
- Problematic
- Plan
- Methods
- Comparison within semantic metrics
- Comparison within references
- Comparison within topics

**Grokipedia**: an AI-generated encyclopedia developed by Elon Musk’s xAI. It aims to produce “truthful” entries using the Grok large language model. Grokipedia relies on the Grok LLM.

xAI: Musk’s company.

**Wikipedia**: a non-profit, volunteer-edited project governed by policies such as Neutral Point of View and verifiability.

“Grokipedia reportedly contained roughly 800–900 thousand entries, supported a suggest-edit rather than direct-edit workflow, and offered only limited transparency about licensing and code provenance.”

Explaination:
- Database size: Grokipedia contained approximately 800,000 to 900,000 entries (articles or pages), which is far fewer than Wikipedia.
- Contribution process: Unlike Wikipedia, where users can directly edit pages, Grokipedia used a “suggest-edit” system, meaning that changes had to be suggested before being validated, rather than applied immediately.
- Limited transparency: Grokipedia provided little clear information about the licenses used (copyright, reuse of content) and about code provenance (origin, development, external contributions).

**Question**
Whether an AI-driven alternative can escape the biases and limitations of human-edited platforms remains unclear. Is Wikipedia biased, and if so, can an AI-first encyclopedia do better? Can Grok produce a less biased encyclopedia than Wikipedia?

**Wikipedia bias:**
- Early left-right slant in political pages that attenuated over time.
- Topical and coverage imbalances.
- Framing asymmetries across ideology and gender.

Research on LLMs demonstrates measurable political and cultural biases that vary across model architectures and prompts.

Grok stood out as one of the few models that did not fabricate references, although roughly 40% of references contained incomplete or inaccurate details.

Study on how source framing influences model judgments: Grok 2 demonstrates high consistency and minimal ideological bias, with only modest shifts in evaluation when the framing of the input changed.

Problematic: For topics that exist on both platforms, how similar are Grokipedia and Wikipedia in practice?

**Metrics**

- Editorial workflows (human vs model-generated) influence both form and content:
    - Descriptive indicators
    - Article length
    - Reference density
    - Link structure
- Three dimensions:
    - Semantic similarities
    - Stylistic similarities: readability, part-of-speech composition
    - Lexical similarities
- Political bias:
    - Outlet-level political-leaning scores were taken from the News Media Bias and Factuality dataset. This public dataset describes the political orientation score of each media outlet and allows evaluation of the slant of each cited reference.
    - To compare political bias between the two platforms, the bias shift was computed as the difference between the average bias score of the Grokipedia article and that of its Wikipedia counterpart. Positive values indicate that the Grokipedia version relies more heavily on right-leaning sources, whereas negative values reflect a shift toward left-leaning sources.

To conduct the study, the authors take the 20,000 most-edited English-language articles in Wikipedia. Among these, approximately 17,700 titles had valid, nontrivial matches on Grokipedia.

Prior research shows that heavily edited entries correlate strongly with controversy, topical salience, and social polarization. This is why the study focuses only on the most-edited articles.

**Results**
- Rightward shift in the political bias of cited sources, concentrated primarily in entries related to politics, history, and religion.

- Bias shift: articles that differ more substantially across platforms are markedly more likely to exhibit a right-leaning shift.

- The strongest rightward shifts in source bias occur in articles on religion, history, languages, and business, indicating that ideological divergence is especially pronounced in these domains.

- AI-generated encyclopedic content diverges from established editorial norms—favoring narrative expansion over citation-based verification. This pattern suggests that Grokipedia’s generation process elaborates on existing material, expanding text length and rhetorical flow, rather than producing substantively new or more rigorously sourced knowledge.

- Semantic similarity averages around 0.86 and stylistic similarity around 0.88, indicating that Grokipedia reproduces much of Wikipedia’s linguistic and conceptual structure.

## 3. Source framing triggers systematic bias in large language models

https://www.science.org/doi/10.1126/sciadv.adz2924

**Context**
Elon Musk has praised xAI Grok 2 for its allegedly “free” approach to content, drawing a contrast with what he describes as the “woke” bias embedded in OpenAI’s models.

AI nationalism—the framing of AI technologies as extensions of national identity, ideology, or geopolitical ambition.

**Study**
The study examines inter- and intramodel agreement across four state-of-the-art LLMs tasked with evaluating 4,800 narrative statements on 24 different topics of social, political, and public health relevance, for a total of 192,000 assessments.

The focus is not on how LLMs generate biased outputs, but on whether, and to what extent, source attribution introduces systematic bias into their agreement judgments with externally produced content.

**Existing research**
- Lior and colleagues: LLMs exhibit framing effects similar to those seen in humans, suggesting that the way input is framed can substantially shape AI-generated responses.

- Lin and colleagues examined political biases in LLMs, particularly in bias prediction and text continuation tasks, revealing that such models may harbor intrinsic biases that affect their evaluative performance.

- Recent research on LLMs’ political bias has shown that some reward models used to fine-tune language outputs cause the models to exhibit political bias, favoring content that aligns with left-leaning political views. The bias appears to originate from training data as well as from the structural design of reward mechanisms. This is not surprising given that models are mainly trained on Wikipedia.

**Methods**

- Phase 1: Prompt four distinct LLMs—OpenAI o3-mini, DeepSeek Reasoner, xAI Grok 2, and Mistral—to produce narrative statements in response to 24 controversial or socially sensitive topics, grouped into eight thematic clusters. Each model generated 50 distinct statements per topic.

- Phase 2: Evaluate the interpretive responses of the same four LLMs by asking them to assess each of the narrative statements (50 × 24 × 4 = 4,800) under 10 attribution conditions:
    - No source attribution, person, national origin, LLM that generated the narrative statements

**Results**

- LLMs’ own judgments of agreement with narrative statements exhibit systematic bias from framing effects, with substantial implications for the neutrality and fairness of LLM-mediated information systems.

- Grok 2 showed the flattest agreement profile, highlighting a uniform agreement level regardless of the source of narrative statements.

- The four LLMs demonstrated a generally high degree of agreement (intramodel and intermodel).

- Grok 2 and DeepSeek Reasoner exhibited more pronounced shifts and negative effects on agreement levels under self-attribution conditions, suggesting a stronger influence of perceived authorship on their rate of agreement with narrative statements.

- Grok 2 displayed a comparable negative bias against DeepSeek Reasoner in the cluster “Politics and international relations,” meaning it evaluated narratives less favorably when it believed they had been written by DeepSeek Reasoner (even if the source was misattributed).

## 4. Large language models reflect the ideology of their creators

19 popular LLMs to describe 3,991 prominent persons with political relevance, and then judge how positively they portray each person.

A growing body of recent research also focuses on broader 'trustworthiness', encompassing not only truthfulness but also safety, fairness, robustness, ethics and privacy.

Ideology: set of beliefs about the proper order of society and how it can be achieved.

Question: How the ideological positions exhibited by different LLMs differ from each other, and whether they may be reflecting the ideological viewpoints of their creators.

Philosophers (Foucault and Gramsci) have argued that the notion of "ideological neutrality" is ill-posed. 

Agonistic pluralism: democratic model where a plurality of ideological viewpoints compete, embracing political differences rather than suppressing them.

Study: investigate the ideological diversity among popular LLMs, while withholding judgment about which LLMs are more 'neutral' and which are more 'biased'.

Methodology:
- Quantifiably eliciting the ideological position of an LLM in a natural setting is challenging.
- Past research submit LLMs to questionnaires designed for political orientation, ask them to resolve ethical dilemmmas or poll them for their opinions on contentious issues. LLMs are highly sensitive to the precise way in which the prompt is formulated.
- Ask LLMs to freely generate descriptions about people with political relevance (political persons) and ask them to judge how positively or negatively the person is portrayed in the description. (Open-ended approach).
- Used the Pantheon dataset: a large annoted database of historical figures from various fields including politics, science, arts, and more, sourced from Wikipedia.
- Selection of political persons: filter out all political persons for which no full name was available, who were born before 1850 or died before 1920, ensuring contemporary relevance of all political persons.
- Score all selected polical persons according to their popularity on the different language editions of Wikipedia.
- Annotated each of the political persons with tags based on the manifesto Project's coding scheme of political manifestos. This resulted in 61 unique tags that differentiate positive and negative sentiments toward specific ideological concepts (European Union
indicating a positive sentiment toward the EU, and European Union a
negative sentiment)
- Stage 1: prompted an LLM to simply describe a political person.
- Stage 2: presented the Stage 1 response to the same LLM in a new conversation, asking it to determine on a five-point Likert scale the sentiment toward the political person reflected in the description.


Results:
- Disparties in ideological positions between LLMs accross different geopolitical regions and across different languages.
- The ideological stance of an LLM reflects the worldview of its creators. 

## 5. Unexpected Knowledge: Auditing Wikipedia and Grokipedia Search Recommendations

Study: search engine in Wikipedia and Grokipedia. In this paper, they present a systematic comparison of the recommendation behavior of Wikipedia and Grokipedia.

Methology:
- 10,000 neutral English words as queries, they collect over 70,000 search engine results and examine their semantic alignment, overlap and topical structure.
- Analyze the semantic alignment between queries and search-engine results.
- select 10,000 most common English words, identified through an n-gram frequency analysis of the Google Trillion Word Corpus
- NSFW terms have been removed.
- the package selenium5 to retrieve search engine results from Wikipedia and Grokipedia
- Word2Vec to generate word embeddings and compute the average cosine similarity between the embedding of the query and those of its recommandations.
Results:
- Both platforms frequently generate results that are weakly related to the original query and, in many cases, surface unexpected content starting from innocuous queries.
- 