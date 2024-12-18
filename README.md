# Intelligent Tutoring System (ITS) for Basic Arithmetic

This project implements an **Intelligent Tutoring System (ITS)** for basic arithmetic operations (addition, subtraction, multiplication, and division). The system uses an ontology-based approach to dynamically adapt to learners' needs, leveraging AI algorithms to deliver personalized feedback and tailored instruction.

---

## Features
- **Ontology-driven Knowledge Representation**: Uses an OWL ontology for representing mathematical operations and associated questions, solutions, and hints.
- **Dynamic Adaptation**: Automatically adjusts question difficulty based on learner performance.
- **Interactive UI**: Built with Python's Tkinter library for an engaging user experience.
- **Scaffolding Support**: Provides hints and simpler questions to help struggling learners.
- **Real-time Feedback**: Offers immediate feedback on learner inputs.

---

## Requirements
To run the ITS, ensure you have the following installed:
1. **Python 3.8+**
2. **Jupyter Notebook**
3. **owlready2** library for ontology management
4. **Tkinter** for GUI development
5. A pre-defined OWL ontology file (`ontology.owl`)

---

## Setup Instructions

### 1. Clone the Repository
To get started, clone this repository to your local machine:
```bash
git clone https://github.com/focuslegon/basic-arithmetic-its.git

```


## 1. Navigate to the project directory:

``` cd your-repository-name ```

## 2. Install Dependencies

Install the required Python libraries using pip:

``` pip install owlready2 ```

## 3. Place the Ontology File

Ensure the ontology file ontology.owl is available in the project directory. Alternatively, specify the correct path in the get_ontology() function within the Python file or notebook:

``` self.onto = get_ontology("path/to/ontology.owl").load() ```

## 4. Launch the Jupyter Notebook

To run and test the ITS, open the Jupyter Notebook:

jupyter notebook

# Navigate to the notebook file (BasicArithmeticITS.ipynb) and open it.
## Usage Instructions

## 1. Load the Ontology

In the notebook or script, make sure the ontology is loaded correctly:

``` self.onto = get_ontology("ontology.owl").load()```

## 2. Run the ITS Application

Run all cells in the notebook sequentially. This initializes the ITS interface, built with Tkinter, and opens the GUI for interaction.

## 3. Use the Application

    Start the ITS: The main window will display a math question. Enter your answer in the input field and click "Submit Answer."
    Hints and Feedback: Use the "Show Hint" and "Teaching Hint" buttons for guidance if you're unsure about the answer.
    Next Question: Upon submitting a correct answer, the "Next Question" button will become active.

## 4. Test the Adaptive Learning

    Intentionally answer questions incorrectly to test the system's scaffolding functionality (easier questions and hints).
    Observe the progress tracker and adaptivity in real-time.

## Testing the System

    Modify questions in the ontology (ontology.owl) to test custom instances and properties.
    Run the ITS in both normal and "easy mode" to evaluate adaptability.
    Analyze learner performance data (if applicable) by integrating with tools like Jupyter for visualization.

## File Structure

├── aasicarithmetic.ipynb  # Main Jupyter Notebook file
├── ontology.owl   # Ontology file for arithmetic operations
├── README.md             # Project documentation

## Future Enhancements

    Expand ontology to cover advanced topics in mathematics.
    Integrate machine learning models for predictive adaptivity.
    Add natural language processing (NLP) for conversational interactions.

 ## Contributing

```Contributions are welcome! Fork the repository and submit a pull request with your updates. For major changes, please open an issue first to discuss your ideas.
License```

This project is licensed under the MIT License.