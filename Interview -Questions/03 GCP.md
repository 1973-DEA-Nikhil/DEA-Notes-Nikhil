### GCP (GOOGLE CLOUD PLATFORM) INTERVIEW QUESTIONS

#### General GCP Questions

1. **Cloud Fundamentals**
   - "Why did you choose GCP over AWS and Azure?"
   - "What are the benefits of using cloud over on-premises solutions?"
   - "What are the different services you're familiar with in GCP?"
   - "Rate yourself in GCP services - how comfortable are you with each service?"

2. **Project Implementation**
   - "Which GCP services did you use in your project?"
   - "Why didn't you implement other Google services in your project except BigQuery?"
   - "How are components of one service connected to another service?"
   - "How can you analyze and bring the result of the combination of two service components?"

#### BigQuery Questions

1. **Basic BigQuery**
   - "What is BigQuery and why do we use it?"
   - "Is BigQuery relational? Can we use primary/foreign keys in BigQuery?"
   - "What are the limitations of BigQuery?"
   - "What are the BigQuery optimization techniques?"

2. **Data Loading & Export**
   ```python
   # Write code to import data from GCS to BigQuery
   # Show both command-line and manual approaches
   ```

   ```python
   # How do you export table from BigQuery to GCS?
   # How do you export only 10 tables out of 20 tables?
   # How do you export table as CSV file to GCS?
   ```

3. **BigQuery Integration**
   ```python
   # Write code to connect BigQuery using Python
   ```
   - "How do you import data from on-premises into BigQuery?"
   - "How would you handle 1TB of relational table data for analysis in BigQuery?"

4. **BigQuery Advanced**
   - "What are materialized views in BigQuery?"
   - "What are authorized views in BigQuery?"
   - "What operators are used to retrieve records in BigQuery?"
   - "How do you optimize BigQuery performance?"

#### Cloud Storage (GCS) Questions

1. **Basic GCS**
   - "What are the different storage classes in GCS?"
   - "Which storage class would you choose for [specific scenario]?"
   - "How do you create a bucket in GCS?"

2. **Data Transfer**
   ```python
   # Write code to upload files from local system to GCS
   ```
   
   ```python
   # How do you import file from bucket1 to bucket2 using commands?
   ```

3. **GCS Integration**
   - "How do you connect your local system with GCS?"
   - "How would you copy file from local system to GCS?"

#### Data Processing Services

1. **Dataflow**
   - "What is Dataflow and how do you integrate it?"
   - "What are the types of windows present in Dataflow?"
   - "Explain Dataflow implementation"
   - "What is lag in Dataflow?"
   - "How do you implement streaming service pipeline?"
   - "What is PCollection?"

2. **Dataproc vs Dataprep**
   - "What's the difference between Dataproc and Dataprep?"
   - "When would you use Dataproc over Dataprep?"

3. **Data Fusion**
   - "What is Data Fusion?"
   - "What is the importance of Data Fusion?"
   - "Have you used Data Fusion in your projects?"

#### Cloud Composer Questions

1. **Basic Composer**
   - "What is Cloud Composer?"
   - "Explain Cloud Composer in depth"
   - "What are DAGs?"

2. **Advanced Composer**
   - "How do you apply transformations in Cloud Composer?"
   - "What operators are available in Composer?"
   - "Explain your DAG implementation"

#### Pub/Sub Questions

1. **Basic Pub/Sub**
   - "What is Pub/Sub?"
   - "What is a subscriber?"
   - "What are Pub/Sub message formats?"

2. **Implementation**
   - "Give a real-time example of Pub/Sub"
   - "How would you implement Pub/Sub in a real-world scenario?"

#### Security & Access Management

1. **IAM**
   - "Basic questions in IAM"
   - "If 10 developers are accessing dataset, instead of giving permission to individual developers, what's the best way?"
   - "What is unified access?"
   - "What is fine-grained access?"
   - "Where do you find these services?"

2. **Security**
   - "What is DLP (Data Loss Prevention)?"
   - "How do you handle sensitive data in GCP?"

#### Scenario-Based Questions

1. **Data Migration**
   ```python
   # You have 1TB of relational data that needs to be analyzed. 
   # Which GCP service would you use and why?
   ```

2. **Performance**
   - "How would you optimize costs in GCP?"
   - "How would you handle high-volume data processing?"

3. **Integration**
   - "How would you implement Oracle database inside GCP?"
   - "How do you validate data in your project?"

4. **Architecture**
   ```python
   # Design a real-time data processing pipeline using GCP services
   # Explain your choice of services and their integration
   ```

5. **Storage Solutions**
   - "When would you choose Cloud SQL over BigQuery?"
   - "What factors influence your choice of storage service?"

6. **Cost Optimization**
   - "How would you optimize costs for large-scale data processing?"
   - "What strategies would you use to reduce BigQuery costs?"

#### Project-Specific Questions

1. **Implementation**
   - "Explain your project end to end"
   - "What was your role in the project?"
   - "What feedback did you get from your guide?"
   - "Is it an internship project or is it using in real life?"

2. **Technical Decisions**
   - "Why did you choose specific services in your project?"
   - "What alternatives did you consider?"
   - "How did you handle data cleaning and validation?"

3. **Challenges**
   - "What challenges did you face in implementing GCP services?"
   - "How did you overcome performance issues?"
   - "What would you do differently if you were to rebuild the project?"
