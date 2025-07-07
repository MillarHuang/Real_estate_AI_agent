# Build a real estate AI agent
### Background of project:
This project aims to build an AI agent to give property recommendation based on the user's perference.

### Set up environment:
Make sure to have conda installed and ready, then create a new environment using the ``requirements.txt``
file provided in the root of the repository and activate it:

```bash
> conda env create -name <name_of_environment> python=3.10
> conda activate <name_of_environment>
> pip install -r requirements.txt
```

### Files
* **HomeMatch.ipynb**: this notebook includes the whole workflow of building a real estate AI agent. To be specific, the workflow is as followings:
  1. Generate 20 real estate listings using a Large Language Model as dataset.
  2. Generating and Storing Embeddings: Convert the LLM-generated listings into suitable embeddings that capture the semantic content of each listing, and store these embeddings in the vector database, like ChromaDB.
  3. Collect user preferences, such as the number of bedrooms, bathrooms, location, and other specific requirements from a set of questions or telling the buyer to enter their preferences in natural language.
  4. Build an LLMChain that maintains conversation history in memory, performs semantic search in a vector database using both user preferences and the current query, incorporates the retrieved text as context into a customized prompt, and generates a response using the LLM.
  5. Example Showcase: Provide a sample query to the LLM to generate personalized property listing descriptions.
    
* **listings**: the generated listings text, including 20 real estate listings.

* **requirements.txt**: the relevant dependencies.


