# VaccineTogether
> Imagine being able to know the side-effects YOU might have before being administered a COVID vaccine. Presenting VaccineTogether, a one-stop solution enabling individuals to be more informed and confident before getting a COVID Vaccine. Moreover, it will enable health care professionals and researchers to crowdsource data, without compromising **data privacy and anonymity**.   

# Problem Statement 
Our application intelligently addresses two problem statement under the SAP Cloud Track, which are as follows:  

1. **Smart data sharing**: How can various countries share data while preserving the privacy of the public in order to order to understand the virus and its effects better?
2. **Vaccination Effects**: How can we better track and monitors the effects of vaccinations on administered people in order to understand their effects and improve them further. 


# What it does
The Application offers 3 key functionalities:
1.  Predict side-effects of a vaccine for a specific user based on their health-related data, while preserving **user privacy and anonymity**
2. Enable users to track their vaccine side-effects using useful analytics as well as crowdsource data for improving the accuracy of the central ML model.
3. Provide global data analytics and insights about vaccination side effects

![Horizontal Federated Learning Algorithm](https://i.postimg.cc/kMjKhx8d/Screenshot-2021-02-28-at-7-05-49-AM.png)


# How we built it
Tech Stack: 
   **Machine Learning**: Tensorflow, Keras
   **Web App**: JavaScript, Flask, Python
   **UI**: SAP UI5 Framework based on Fiori Guidelines 
   **Maintaining User Privacy and Anonymity**: Using Federated Horizontal Learning & Deep Neural Network

# Challenges we ran into
   - Finding the right dataset to train our models
   - The datasets are very recent (1 Month old) and hence with no documentation or metadata
   - Data Preprocessing, cleaning and extracting useful insights
   - Integrating the Central Machine Learning model hosted on the cloud,  to the locally hosted machine learning model  (Updating the model weights with the new gradients. _Refer to horizontal federated learning_)
    
# Accomplishments that we're proud of
   - Predicting side-effects on new users, with high accuracy for the federated model (Compared to a traditional model trained on a completely centralised dataset)
   - Training the model comprising a user's personal information, and health data, through horizontal federated learning
   - Deploying an entire ML-based application to the SAP Cloud Platform with client-side integrations 
   - Understanding about the state-of-the-art method Horizontal Federated    


# What we learned
   - We learned how to use the SAP UI5 framework for building responsive application following the Fiori guidelines. 
  - We deployed our entire application on the SAP Cloud Platform, leveraging its robust infrastructure and platform for application development
 - Staying awake for 24 hours (_I am writing this at the 23rd hour of the Hackathon XD_)


# What's next for VaccineTogether
- Increase the acceptance rate of our application to get more data
- Improving our central Federated ML Model as and when more data is available from our users.  
- Vaccine Cold chain integration with SAP Ariba and SAP S4HANA.  


# Screenshots
![Screenshot 1](https://i.postimg.cc/63fLQgy7/Screenshot-2021-02-28-at-1-00-41-AM.png)
![Screenshot 2](https://i.postimg.cc/fLCmsdrm/Screenshot-2021-02-28-at-2-31-08-AM.png)
![Screenshot 3](https://i.postimg.cc/SKWcZ3LZ/Screenshot-2021-02-28-at-2-24-01-AM.png)


# Installation
**Steps**:
1.  Download/ Clone this git repository  

**To run the Juptyer notebooks, download:**
1. Download Jupyter notebook 
2. Navigate to the `notebooks` directory
3. Run each cell  

**To run the UI5 Web App Application:**
1. Execute  `ui5 serve  -o  /index.html`
**To run flask backend:**
1. Execute `FLASK_APP=model.py flask run`

The global model is already hosted on the SAP Cloud Platform. 

# Team Members
1. Jay Gupta
2. Ritwik Kanodia
3. Palak Somani
4. Aditya Bansal
