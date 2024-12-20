# ChemCrow Red-Teaming Protocols

This zip file contains:
- **`ChemCrow_Redteaming.ipynb`**: A Jupyter Notebook to simulate, analyze, and extend chemical workflows using a toolset for molecular operations.
- **`requirements.txt`**: A file listing the dependencies required to run the notebook.
- **`run_log_modified.json`**: A log file documenting the prompts crafted using prompt engineering and the corresponding responses, including potentially malicious outputs generated by the LLM agent.

## 👩‍💻 Installation

To set up the required environment, follow these steps:

1. Extract the contents of the zip file to a directory on your local machine.
2. Install the necessary Python libraries using the `requirements.txt` file:
   ```bash
   pip install -r requirements.txt
   ```
   Alternatively, you can manually install:
   - RDKit
   - Pandas
   - NumPy
   - Matplotlib

3. Optionally, install the ChemCrow package for direct usage:
   ```bash
   pip install chemcrow
   ```

## 🔥 Usage

### Notebook Execution
1. Launch the Jupyter Notebook environment:
   ```bash
   jupyter notebook ChemCrow_Redteaming.ipynb
   ```
2. Follow the notebook instructions to simulate, validate, and analyze workflows.
3. Modify workflows or add new ones directly in the notebook as needed.

### API Interaction
Set up your API keys for enhanced functionality:
- OpenAI API Key:
  ```bash
  export OPENAI_API_KEY=your-openai-api-key
  ```
- (Optional) Serp API Key:
  ```bash
  export SERP_API_KEY=your-serpapi-api-key
  ```

In a Python session:
```python
from chemcrow.agents import ChemCrow

chem_model = ChemCrow(model="gpt-4-0613", temp=0.1, streaming=False)
chem_model.run("What is the molecular weight of tylenol?")
```

## File Details

### `ChemCrow_Redteaming.ipynb`
This notebook:
- Simulates molecule modifications, safety summaries, and property predictions.
- Logs and visualizes outputs for analysis.

### `requirements.txt`
Lists the Python libraries required to run the notebook.

### `run_log_modified.json`
Documents the logs of prompt engineering experiments and responses, serving as a reference for analyzing and improving red-teaming strategies.

## Extending the Notebook

### Adding New Workflows
1. Open the notebook.
2. Append a new workflow directly in the relevant sections.
3. Save and execute the new workflow for validation and analysis.

### Enhancing the Notebook
- Add new cells for advanced simulations or visualizations.
- Incorporate additional chemical tools or libraries for extended functionality.

Happy experimenting with ChemCrow!
#
