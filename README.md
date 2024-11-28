## CitySTI 2024: A System for Tabular data to Knowledge Graph Matching
SemTab 2024 Challenge - STI vs LLMs Track (https://sem-tab-challenge.github.io/2024/tracks/sti-vs-llm-track.html)

The code was executed using Python 3.9.13 and on a virtual environment (virtualenv).
Insert the API key before execution. 

### Round 1
- **Gemini Model from Google**: py cea-gemini.py
- **Llama Model from HuggingFace**: py cea-hf-llama.py
- **GPT Model from OpenAI**: py cea-openai.py  (version used in SemTab 2024)

- **Command-Line Interface**: main-r1.py

Dataset: SuperSemTab24 (https://zenodo.org/records/11031987)

### Round 2 
- **Gemini Model from Google**: py cea-gemini-r2.py

Compared to the version for Round 1:
- Refined prompts.
- Set response safety of prompts to "None".
- Processed the cleaning of data by the LLM in batches of 15 instead as a whole.
- Provided few rows for context during the matching process by the LLM, rather than using the entire table.
- Used Gemini-1.5-Flash instead of GPT-4o-Mini.


Dataset: MammoTab24 (https://zenodo.org/records/11031987)


### Evaluate CEA task with Wikidata Entities
- **CEA_WD_Evaluator**: py CEA_WD_Evaluator.py

### Publications
- Dylan Li Tin Yue and Ernesto Jimenez-Ruiz. **CitySTI 2024 System: Tabular Data to KG Matching using LLMs**. Proceedings of the Semantic Web Challenge on Tabular Data to Knowledge Graph Matching (SemTab 2024), co-located with the 23rd International Semantic Web Conference (ISWC), November 11-15, 2024, Baltimore, USA.

