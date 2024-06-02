# Evaluation of English-Russian Machine Translation of Technical Terms Using Large Language Models

### Description
This project investigates the application of Large Language Models (LLMs) to the translation of technical terms between English and Russian, addressing the challenge of accurately conveying domain-specific terminology across languages. The study introduces a novel approach by constructing a dedicated corpus of technical terms and contexts. 

### Motivation and Background
Machine translation has advanced significantly, but accurately translating domain-specific terminology remains challenging. Existing models often struggle with specialized vocabulary, leading to inaccuracies. This project aims to improve the translation quality of technical terms by utilizing LLMs and developing effective prompting strategies.

### Key Features
- Corpus Construction: A specialized corpus created from multiple sources including a linguistic encyclopedic dictionary, Wikipedia, Paracrawl, TED Talks, and CyberLeninka.
- Prompting Strategies: Exploration of various prompting strategies for LLMs when translating scientific texts, focusing on the domains of linguistics and physics.
- Comprehensive Evaluation: Use of BLEU, ROUGE, CHRF, and COMET scores to systematically assess translation quality.
- Focused Domains: Comparative analysis conducted in the fields of linguistics and physics to evaluate the impact of different prompting strategies.

### Data Access
The databases created during this project are available in the following Google Drive folder: [Google Drive Folder](https://drive.google.com/drive/folders/1DTp3FRMgDZisBo7ulZa1jhLpqiyAWwms?usp=sharing

### Results
The results of this study indicate that term translation prompts significantly improve the accuracy and contextual relevance of translations. Detailed evaluation using BLEU, ROUGE, CHRF, and COMET metrics supports this finding.

#### Database Statistics
| Database             | BLEU Mean  ROUGE Mean | CHRF Mean | COMET Mean |
|----------------------|-----------|------------|-----------|------------|
| ling_ParaCrawl.db    | 0.16      | 0.35       | 50.49     | 0.78       |
| phys_ParaCrawl.db    | 0.16      | 0.41       | 52.42     | 0.79       |
| ling_ted.db          | 0.18      | 0.34       | 52.22     | 0.83       |
| phys_ted.db          | 0.19      | 0.35       | 50.51     | 0.83       |
| ling_cyberleninka.db | 0.28      | 0.35       | 59.87     | 0.79       |
| phys_cyberleninka.db | 0.30      | 0.49       | 59.62     | 0.80       |
| Overall              | 0.21      | 0.37       | 53.66     | 0.80       |

#### Prompt Type Statistics
| Prompt Type          | BLEU Score | ROUGE Score | CHRF Score | COMET Score |
|----------------------|------------|-------------|------------|-------------|
| general_translation  | 0.22       | 0.39        | 56.59      | 0.83        |
| term_definition      | 0.17       | 0.33        | 46.49      | 0.75        |
| term_translation     | 0.23       | 0.40        | 57.65      | 0.83        |

#### Best Prompt Types
The term translation prompts were found to be the best for all metrics.

### Visualization
The results include several visualizations that show the statistics of different metrics across various databases and prompt types.

BLEU Score by Prompt Type:
![BLEU Score by Prompt Type](https://github.com/elinkamaeva/terminology_translation/blob/main/vizes/bleu_score_prompt_type_statistics.png)

BLEU Score by Database:
![BLEU Score by Database](https://github.com/elinkamaeva/terminology_translation/blob/main/vizes/bleu_score_statistics.png)

CHRF Score by Prompt Type:
![CHRF Score by Prompt Type](https://github.com/elinkamaeva/terminology_translation/blob/main/vizes/chrf_score_prompt_type_statistics.png)

CHRF Score by Database:
![CHRF Score by Database](https://github.com/elinkamaeva/terminology_translation/blob/main/vizes/chrf_score_statistics.png)

COMET Score by Prompt Type:
![COMET Score by Prompt Type](https://github.com/elinkamaeva/terminology_translation/blob/main/vizes/comet_score_prompt_type_statistics.png)

COMET Score by Database:
![COMET Score by Database](https://github.com/elinkamaeva/terminology_translation/blob/main/vizes/comet_score_statistics.png)

ROUGE Score by Prompt Type:
![ROUGE Score by Prompt Type](https://github.com/elinkamaeva/terminology_translation/blob/main/vizes/rouge_score_prompt_type_statistics.png)

ROUGE Score by Database:
![ROUGE Score by Database](https://github.com/elinkamaeva/terminology_translation/blob/main/vizes/rouge_score_statistics.png)

### License
This project is licensed under the MIT License.
