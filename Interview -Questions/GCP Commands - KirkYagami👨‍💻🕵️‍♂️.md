## NOTE: Run the following commands in a Linux type terminal (e.g. git bash )

# 1. Cloud Dataproc
https://drive.google.com/drive/u/0/folders/1Ht8rvmz11NzuVh4X-9WIM-iweZsvZVlB
## 1. To create a Dataproc Cluster
```shell
gcloud dataproc clusters create pyspark-cluster2 \
  --enable-component-gateway \ 
  --region=us-central1 \
  --zone= \
  --master-machine-type=e2-standard-2 \
  --worker-machine-type=e2-standard-2 \
  --num-workers=2 \
  --master-boot-disk-size=50GB \
  --worker-boot-disk-size=50GB \
  --image-version=2.1-ubuntu20 \
  --optional-components=JUPYTER
```


# --- OR --- 

```shell
gcloud dataproc clusters create pyspark-cluster --enable-component-gateway --region us-central1 --master-machine-type e2-standard-2 --master-boot-disk-type pd-balanced --master-boot-disk-size 50 --num-workers 2 --worker-machine-type e2-standard-2 --worker-boot-disk-type pd-balanced --worker-boot-disk-size 50 --image-version 2.1-ubuntu20 --optional-components JUPYTER --project bigdata3844
```

### gcloud Commands: Cloud Dataproc: CleanUp

```shell
# Set Project
gcloud config set project PROJECT_ID
gcloud config set project bigdata3844

# Set Cloud Dataproc Region
gcloud config set dataproc/region VALUE
gcloud config set dataproc/region us-central1

# List Jobs
gcloud dataproc jobs list

# List Clusters
gcloud dataproc clusters list

# Delete Cluster
gcloud dataproc clusters delete pyspark-cluster2

# List Clusters
gcloud dataproc clusters list
```



# 2. Some GCS commands

### **GCP Bucket Operations: File Transfer from Source to Target**

This set of commands helps in logging into Google Cloud, setting the project, creating two storage buckets, uploading `.pdf` files from a local directory to a source bucket, and then moving those files to a target bucket for further use or processing.

```sh
gcloud auth login
gcloud config set project PROJECT_ID
gsutil mb gs://source-bucket
gsutil mb gs://target-bucket
gsutil cp C:/data/source/*.pdf gs://source-bucket/
gsutil mv gs://source-bucket/*.pdf gs://target-bucket/
```

