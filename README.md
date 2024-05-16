# Legal Case Analysis Project

This project uses a Large Language Model (LLM) to analyze legal cases and identify potential issues, such as hearsay. 

## Requirements

* Python 3.8 or higher
* Required Python packages are listed in `requirements.txt`. You can install them with `pip install -r requirements.txt`.
* An OWL file (`LMSS.owl` is provided) containing legal ontology classes.
* Access to a supported LLM. This project provides examples using Google Gemini Pro and Open Llama 7b.  

## Configuration

1. **LLM Path:** Update the `LLM_PATH` variable in the Jupyter notebooks to point to the location of your LLM model.  
2. **OWL File Path:** Make sure the `PATH_TO_OWL` variable correctly points to your OWL file. 
3. **API Keys:** If you're using Google Gemini Pro, replace the placeholder `GOOGLE_API_KEY` with your actual API key.

## Running the Code

The project includes multiple Jupyter notebooks demonstrating different LLM configurations and prompting techniques:

* `Final_Files/hearsay_LMSS_geminiapi.html`: This notebook uses Google Gemini Pro to determine whether a given legal statement constitutes hearsay.
* `hearsay_LMSS_llama_instruct.html`: This notebook utilizes Open Llama 7b (instructed) to analyze legal statements for hearsay.
* `hearsay_LMSS_gemma_instruct.html`: This notebook employs Gemma 7b (instructed) to classify legal statements as hearsay or not.

To run a notebook:

1. Open the notebook in a Jupyter environment.
2. Update the configuration variables as described above.
3. Execute the cells sequentially.

## Output

The notebooks generate responses from the LLM and evaluate its performance on a set of test cases. The results are also saved to CSV files (`hearsay_results.csv`, `scalr_results.csv`, `reasoning_casuality_results.csv`) for further analysis.

## Note

The code is provided as a starting point and may need to be adjusted depending on your specific requirements and the chosen LLM. Make sure to read the comments in the notebooks for guidance on how to modify the code.
content_copy
Use code with caution.

This README explains how to run the code, including dependencies and configuration, and provides a brief overview of the project's functionality and output. Remember to replace the placeholders with your actual file paths and API keys before running the code.