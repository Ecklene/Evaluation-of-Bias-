# Evaluation-of-Bias
Evaluating Social Bias in Language Model

This evaluates Social Bias in Small Language Models. Four models (BERT-BASE, BART, and ROBERTA-BASE) are used and fine-tuned on a text-three dataset (CrowsPair and Stereotype). BOLD Dataset was used for text generation using GPT2 only.

The Crowspair dataset consists of stereotype and anti-stereotype text. The dataset is annotated and consists of 1,508 examples covering nine types of biases: race, gender, sexual orientation, religion, age, nationality, disability, physical appearance, and socioeconomic status. Each example consists of two sentences, the first of which always refers to a historically underrepresented group in the United States and the second of which always refers to a contrastingly privileged group. A stereotype may be illustrated or violated in the first sentence. The second statement only slightly modifies the first. Each illustration has the following details: -The more stereotypical statement is sent_more. -A sentence with fewer stereotyped elements is sentence-less.
The labels (bias_type) that show if the statement is stereotypical or anti-stereotypical: Annotations: The crowd workers biased annotations Anon_writer: The author's pseudonymous ID. Anon_annotators: The annotators' anonymized IDs.

Stereotype Dataset StereoSet is a large dataset that measures stereotype bias in language models. It consists of 17,000 sentences that measure model preferences across gender, race, religion, and profession. The data contains: -ID, which is the question id
Target which is the label for the stereotype, anti_stereotype, and unrelated Bias_type: type of biases including gender, race, religion, and profession Context: context sentence

Bias in Open-ended Language Generation Dataset (BOLD) BOLD dataset evaluates fairness in open-ended language generation in the English language. It consists of 23,679 different text generation prompts that allow fairness measurement across five domains: profession, gender, race, religious ideologies, and political ideologies. 
Domain. # of prompts Gender 3,204 Race 7,657 Profession 10,195 Religious ideologies 639 Political ideologies 1,984 Total 23,679 Reference for Crows-Pairs Dataset 


Reference:
@inproceedings{nangia2020crows, title = "{CrowS-Pairs: A Challenge Dataset for Measuring Social Biases in Masked Language Models}", author = "Nangia, Nikita and Vania, Clara and Bhalerao, Rasika and Bowman, Samuel R.", book title = "Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing", month = Nov, year = "2020", address = "Online", publisher = "Association for Computational Linguistics" } 

Reference for stereotype Dataset @misc{nadeem2020stereoset, title={StereoSet: Measuring stereotypical bias in pre-trained language models}, author={Moin Nadeem and Anna Bethke and Siva Reddy}, year={2020}, eprint={2004.09456}, archivePrefix={arXiv}, primaryClass={cs.CL} } 

Reference for Bold Dataset @inproceedings{bold_2021, author = {Dhamala, Jwala and Sun, Tony and Kumar, Varun and Krishna, Satyapriya, and Pruksachatkun, Yada and Chang, Kai-Wei, and Gupta, Rahul}, title = {BOLD: Dataset and Metrics for Measuring Biases in Open-Ended Language Generation}, year = {2021}, isbn = {9781450383097}, publisher = {Association for Computing Machinery}, address = {New York, NY, USA}, url = {https://doi.org/10.1145/3442188.3445924}, doi = {10.1145/3442188.3445924}, book title = {Proceedings of the 2021 ACM Conference on Fairness, Accountability, and Transparency}, pages = {862–872}, numpages = {11}, keywords = {natural language generation, Fairness}, location = {V
