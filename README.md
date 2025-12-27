# Mental Health Screening Tool

A Python-based mental health assessment tool that screens for depression and anxiety using standardized clinical questionnaires (PHQ-9 and GAD-7).

## 📋 About

This project provides a comprehensive mental health screening system that:
- Assesses depression using the PHQ-9 (Patient Health Questionnaire-9)
- Assesses anxiety using the GAD-7 (Generalized Anxiety Disorder-7)
- Analyzes symptoms and matches them to potential conditions
- Provides urgency level classification
- Generates personalized recommendations
- Creates data visualizations of assessment scores

## 🔧 Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib** - Data visualization
- **Jupyter Notebook** - Interactive development environment

## 📊 Features

### Clinical Assessments
- **PHQ-9 Depression Scale**: 0-27 scoring system
  - 0-4: Minimal depression
  - 5-9: Mild depression
  - 10-14: Moderate depression
  - 15-19: Moderately severe depression
  - 20-27: Severe depression

- **GAD-7 Anxiety Scale**: 0-21 scoring system
  - 0-4: Minimal anxiety
  - 5-9: Mild anxiety
  - 10-14: Moderate anxiety
  - 15-21: Severe anxiety

### Additional Features
- Symptom-based condition matching
- 5-level urgency classification system
- Crisis detection and emergency resources
- Visual score representations using bar charts
- Comprehensive screening reports

## 🚀 Installation
```bash
# Install required packages
pip install pandas numpy matplotlib jupyter
```

## 💻 Usage
```python
# Initialize the screener
screener = MentalHealthScreener()

# Collect patient information
patient = screener.collect_patient_info("Patient Name", 28, "Female")

# PHQ-9 Depression assessment (9 questions, 0-3 scale each)
dep_responses = [2, 2, 1, 2, 1, 1, 1, 0, 0]
dep_score = screener.calculate_depression_score(dep_responses)

# GAD-7 Anxiety assessment (7 questions, 0-3 scale each)
anx_responses = [2, 2, 1, 1, 1, 1, 1]
anx_score = screener.calculate_anxiety_score(anx_responses)

# Symptom analysis
symptoms = ['persistent_sadness', 'excessive_worry', 'sleep_problems']
conditions = screener.screen_symptoms(symptoms)

# Generate and display report
report = screener.generate_report(patient, dep_score, anx_score, symptoms, conditions)
screener.display_report(report)

# Visualize scores
screener.visualize_scores(report)
```

## 📁 Project Structure
```
mental-health-screening-tool/
│
├── mental_health_screening_tool.ipynb    # Main Jupyter notebook
└── README.md                              # Project documentation
```

## 🆘 Crisis Resources

- **National Suicide Prevention Lifeline (US)**: 988
- **Crisis Text Line**: Text HOME to 741741
- **International**: [IASP Crisis Centres](https://www.iasp.info/resources/Crisis_Centres/)

## ⚠️ Disclaimer

This tool is for **educational and screening purposes only**. It does not provide medical diagnosis or replace professional mental health care. Always consult licensed mental health professionals for diagnosis and treatment.

## 📝 Clinical Background

The assessments used in this tool are based on:
- **PHQ-9**: Validated screening tool for depression (Kroenke et al., 2001)
- **GAD-7**: Validated screening tool for anxiety disorders (Spitzer et al., 2006)

## 👤 Author

**Izedike Benson Anita**
GitHub: [@Anita-Izedike](https://github.com/Anita-Izedike)
- Email: izedikeanita081@gmail.com
  
  

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Clinical assessment tools based on validated PHQ-9 and GAD-7 questionnaires
- Built as part of a portfolio project to demonstrate Python programming and healthcare technology skills

---

**Note**: If you or someone you know is in crisis, please seek immediate help from emergency services or crisis hotlines.
