## Initial set up
Open Google Cloud Shell from the Google Cloud console

### Set Project ID
gcloud config set project [ID] - Sets the current project to the ID

### Identify Regions
gcloud compute regions list - Check the list of available regions

### Set region
gcloud config set compute/region us-east1 - Sets the default region to us-east1

### Set Zone
gcloud config set compute/zone us-east1-c - Sets the default zone to c

## Labels

### Create Virtual Machine Instance with Labels
gcloud compute instances create [instance-name] --labels key=value, key=value

### List existing labels
gcloud compute instances desceibe [instance-name] --format "[format](labels)"
gcloud compute instances desceibe [instance-name] --format "yaml(labels)" - displays in yaml format

### Update existing labels
gcloud compute instances update instance-2 --update-labels team=performance