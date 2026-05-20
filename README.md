
# **AI-Agents-for-Medical-Diagnostics**

## **Project Description**

The **AI-Agents-for-Medical-Diagnostics** project leverages machine learning and artificial intelligence agents to analyze medical reports and generate a **final diagnosis**. The system utilizes three specialized agents:

1. **Cardiologist Agent**: Diagnoses potential cardiovascular conditions, particularly arrhythmia, based on symptoms and reports.
2. **Psychologist Agent**: Analyzes potential psychological conditions, particularly anxiety and panic disorders.
3. **Pulmonologist Agent**: Assesses respiratory issues and evaluates the impact of anxiety-induced panic episodes on pulmonary health.

Each agent processes the provided data and generates a diagnosis, which is combined to produce a **final diagnosis**. This output is saved in a text file for further review.

---

## **Project Requirements**

### **System Requirements**
- **Operating System**: Windows/Linux/Mac
- **Python Version**: Python 3.7+ (Python 3.10+ recommended)

### **Python Libraries**

You will need the following Python libraries to run this project:

- `flask` (for the web framework, if applicable)
- `numpy` (for numerical computations)
- `pandas` (for data processing)
- `scikit-learn` (for machine learning models)
- `tensorflow` or `pytorch` (for AI model processing, depending on which framework you use)
- `openai` (if using OpenAI models for agent responses)
- `matplotlib` (for data visualization, if needed)

### **Installing Dependencies**

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/AI-Agents-for-Medical-Diagnostics.git
````

2. Navigate into the project directory:

   ```bash
   cd AI-Agents-for-Medical-Diagnostics
   ```

3. Set up a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   ```

4. Activate the virtual environment:

   * On Windows:

     ```bash
     .\venv\Scripts\activate
     ```
   * On Linux/Mac:

     ```bash
     source venv/bin/activate
     ```

5. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

---

## **Database Setup**

This project requires a database to store results and manage input data. You can use SQLite or any SQL database you prefer.

### **Database Configuration:**

1. Ensure you have **SQLite** or another SQL database set up on your local machine. If you're using SQLite, the database file will be created automatically when you run the project.

2. If you’re using a different database (e.g., PostgreSQL, MySQL), make sure to update the connection settings in `config.py` or the relevant configuration file.

3. The database schema includes tables for storing agent outputs and the final diagnosis. Here’s a basic overview of the database schema:

   * **Agents Table**: Stores the output of each individual agent (Cardiologist, Psychologist, Pulmonologist).
   * **Final Diagnosis Table**: Stores the combined final diagnosis from all agents.

   Ensure that your database is accessible by the application for reading and writing data.

---

## **How to Run the Project Locally**

1. **Set Up the Database**:

   * If you’re using SQLite, no extra configuration is required. The database will be created automatically when you run the project.
   * For other databases, update the database configuration in `config.py` or the relevant configuration file.

2. **Run the Flask Application** (if the project uses Flask for a web interface):

   * Start the Flask server by running:

     ```bash
     python app.py
     ```

   * The server will start, and you should be able to access the project at:

     ```
     http://127.0.0.1:5000/
     ```

3. **Running the Agents Locally**:

   * The project includes three AI agents: **Cardiologist**, **Psychologist**, and **Pulmonologist**. When running the project locally, the agents will automatically process medical reports and generate their respective diagnoses.

   * The results from each agent will be combined into a **final diagnosis**, which will be saved as a `.txt` file in the `results/` folder.

4. **Testing the System**:

   * Test the functionality by uploading a sample medical report (if the project includes a UI) or using the default input data for testing.

5. **Final Diagnosis**:

   * The final diagnosis will be saved in the `results/final_diagnosis.txt` file.
   * You can view the final diagnosis by opening this text file.

---

