Proficio Metrica is an advanced tool designed to enhance the job application process by leveraging the power of natural language processing (NLP) and data analytics. This tool aims to parse and extract relevant information from resumes, identify keywords, cluster the data into sectors based on these keywords, and provide insightful recommendations, predictions, and analytics to both applicants and recruiters. The primary goal of this project is to streamline the recruitment process and assist users in improving their resumes for better job matching. By transforming unstructured resume data into actionable analytics, this tool facilitates better job matching, strengthens the skills of applicants, and helps organizations make data-driven recruitment decisions. Furthermore, the tool’s user-centric design and continuous improvement approach promise to attract and retain users, making it a vital asset in the modern recruitment landscape. 

Steps for successful execution

1.Download this repository

2.Open command prompt and change the directory to Proficio Metrica

3.Create a virtual environment and activate it using following commands
  python -m venv venvapp
  cd venvapp/Scripts
  activate
	
4.Downloading packages from requirements.txt inside App folder using following commands
  cd../..
  cd App
  pip install -r requirements.txt
  python -m spacy download en_core_web_sm
	
5.After installation is finished create a Database cv
  And change user credentials inside App.py
  at line 95, connection = pymysql.connect(host='localhost',user='root',password='root',db='cv')
	
6.Go to venvapp\Lib\site-packages\pyresparser folder
  And replace the resume_parser.py with resume_parser.py
  which was provided by me inside pyresparser folder
	
7.Finally,Run the App.py file using
  streamlit run App.py

