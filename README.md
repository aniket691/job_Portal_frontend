# Job Portal System: AI-Powered Career Connections 🚀
# Deployed Link: [PROHIRE](https://prohirejobs.netlify.app)
## Overview

This project is an **AI-Enhanced Job Portal System** designed to intelligently connect job seekers with their ideal opportunities and empower recruiters with smart talent acquisition tools. Leveraging cutting-edge Artificial Intelligence and Machine Learning, the platform goes beyond traditional job boards to offer personalized experiences, efficient matching, and insightful analytics. Built with a robust **React.js frontend**, a scalable **Spring Boot backend**, and a reliable **MySQL database**, this system streamlines the entire hiring process for both job seekers and recruiters.

---

## 🌟 Key Features with AI Integration

### For Job Seekers:

* **Smart Registration & Login**: Secure account creation and login, with **AI-driven anomaly detection** for enhanced security.
* **AI-Powered Profile Management**:
    * Create and manage comprehensive profiles, including skills, experience, and resume uploads.
    * **Intelligent Resume Parsing**: Automatically extracts key information (skills, experience, education) from uploaded resumes, populating the profile and identifying relevant keywords.
    * **Skill Gap Analysis**: AI identifies potential skill gaps based on desired job roles and suggests relevant courses or certifications.
    * **Profile Optimization Suggestions**: AI provides recommendations to enhance profile visibility and match potential jobs.
* **Personalized Job Search & Recommendations**:
    * Search for job listings using advanced filters (job title, location, required skills).
    * **AI-Driven Job Matching**: Receives highly personalized job recommendations based on profile, past applications, and learned preferences.
    * **Semantic Search**: Understands the *intent* behind job seeker queries, providing more relevant results even with varied phrasing.
* **Intelligent Job Application**:
    * Apply for jobs directly through the platform.
    * **AI-Assisted Cover Letter Generation**: Provides intelligent suggestions or drafts for personalized cover letters based on the job description and seeker's profile.
    * **Application Status Tracking with Insights**: Track application status with **predictive insights** on typical response times or next steps.

### For Recruiters:

* **Smart Registration & Login**: Secure account creation and login, with **AI-driven anomaly detection** for enhanced security.
* **Company Profile Management**: Recruiters can manage their company profiles and branding.
* **AI-Assisted Job Posting**:
    * Post job openings with details like title, description, required skills, and location.
    * **Intelligent Job Description Writing**: AI assists in crafting compelling and keyword-rich job descriptions based on role and industry.
    * **Skill Suggestion**: AI recommends relevant skills based on the job title and description, ensuring comprehensive listings.
* **AI-Powered Job & Applicant Management**:
    * Manage, update, and monitor job postings efficiently.
    * **Smart Candidate Matching**: AI ranks and recommends the most suitable candidates for each job opening based on skills, experience, and resume content.
    * **Automated Applicant Screening**: AI can pre-screen applications based on defined criteria, highlighting top candidates and reducing manual review time.
    * **Resume Parsing & Analysis**: Automatically extracts and analyzes key information from applicant resumes, providing a quick overview of qualifications.
    * **Market Trend Analysis**: AI provides insights into talent availability, salary benchmarks, and trending skills for specific roles.

---

## 🚀 Technology Stack

* **Frontend**: React.js
* **Backend**: Spring Boot (for core business logic and API endpoints)
* **AI/ML Services**: Python (Flask/FastAPI for ML model serving), TensorFlow, PyTorch, Scikit-learn, NLTK, spaCy (for NLP tasks like resume parsing, semantic search, content generation).
* **Database**: MySQL
* **Deployment (Optional AI Component)**: Docker, potentially cloud services like AWS SageMaker, Google Cloud AI Platform, or Azure Machine Learning for scalable model deployment.

---

## 🛠️ Installation & Setup

### Prerequisites

* Node.js and npm (for frontend)
* Java 17+ and Maven (for Spring Boot backend)
* Python 3.8+ and pip (for AI/ML services)
* MySQL Server

### Backend Setup (Spring Boot)

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/aniket691/job_portal.git](https://github.com/aniket691/job_portal.git)
    ```
2.  **Navigate to the backend directory:**
    ```bash
    cd job_portal/backend
    ```
3.  **Update the `application.properties` file** with your MySQL database credentials:
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/career_crafters?useSSL=false&serverTimezone=UTC
    spring.datasource.username=root
    spring.datasource.password=yourpassword
    ```
4.  **Build and run the Spring Boot application:**
    ```bash
    mvn clean install
    mvn spring-boot:run
    ```

### AI/ML Services Setup (Python)

1.  **Navigate to the AI/ML services directory:**
    ```bash
    # Assuming an 'ai_services' directory within the project
    cd job_portal/ai_services 
    ```
2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    # On Windows:
    .\venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate
    ```
3.  **Install required Python packages:**
    ```bash
    pip install -r requirements.txt # You'll need to create this file with all AI/ML dependencies
    ```
    *(Example `requirements.txt` content: `flask`, `tensorflow`, `scikit-learn`, `spacy`, `nltk`, `pandas`, `numpy`)*
4.  **Download any necessary NLP models (e.g., spaCy models):**
    ```bash
    python -m spacy download en_core_web_sm
    ```
5.  **Run the AI/ML service (e.g., Flask/FastAPI server):**
    ```bash
    python app.py # Or whatever your main AI service file is named
    ```
    *(Note: This service will typically expose APIs that the Spring Boot backend consumes.)*

### Frontend Setup (React.js)

1.  **Navigate to the frontend directory:**
    ```bash
    cd job_portal/ProHireFrontEnd
    ```
2.  **Install the required npm packages:**
    ```bash
    npm install
    ```
3.  **Start the React development server:**
    ```bash
    npm run dev
    ```

### Database Setup (MySQL)

1.  **Create a new database in MySQL:**
    ```sql
    CREATE DATABASE career_crafters;
    ```
2.  The database schema will be automatically created by the Spring Boot application when it runs for the first time.

---

## 🚀 Usage

Once all components (Backend, AI/ML Services, Frontend) are running:

* Access the application through `http://localhost:3000` (React frontend).
* **Register** as a job seeker or recruiter.
* **Job seekers** can leverage AI for:
    * **Smart Profile Creation**: Upload your resume and watch as key details are automatically extracted.
    * **Personalized Job Feed**: Discover jobs uniquely suited to your skills and career aspirations.
    * **Cover Letter Assistance**: Get AI-powered suggestions to tailor your applications.
* **Recruiters** can utilize AI for:
    * **Efficient Job Posting**: Receive AI suggestions for crafting effective job descriptions.
    * **Intelligent Candidate Screening**: Quickly identify top talent with AI-ranked applicants and resume analysis.
    * **Market Insights**: Understand talent availability and skill trends to refine your hiring strategy.

---

## 🤝 Contributing

Contributions are highly encouraged! We are particularly interested in expanding our AI/ML capabilities. Please fork the repository and submit a pull request with your improvements.

### Areas for AI/ML Contributions:

* **Advanced Resume Parsing**: Improve accuracy and extraction for diverse resume formats.
* **Enhanced Job-Seeker/Job Matching Algorithms**: Explore deep learning models for more nuanced matching.
* **Interview Preparation Tools**: Develop AI-powered mock interview features with feedback.
* **Fraud Detection**: Implement ML models to identify suspicious job postings or applications.
* **Skill Taxonomy & Mapping**: Create a robust system for understanding and mapping skills across industries.
* **Sentiment Analysis**: Analyze job descriptions and applications for tone and fit.

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/aniket691/job_portal/blob/main/LICENSE.md) file for details.

---

## 📞 Contact

For any questions, suggestions, or collaboration opportunities, feel free to reach out:
* **Aniket Dalal**
* **Email:** [aniketdalal126@gmail.com](mailto:aniketdalal126@gmail.com)
* **GitHub:** [@aniket691](https://github.com/aniket691)
"# prohire_backend" 
