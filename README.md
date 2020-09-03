<!-- Change title below -->

# gads-2020-project-submission-template

## QwikLabs Completed

<details>
  <!-- The complete lab title goes here 👇🏾-->
  <summary>Lab 1: Google Cloud Fundamentals: Getting Started with Compute Engine
</summary>
  <!-- Provide path to the screenshot here. Example 👇🏾-->
  <img src="screenshots/example_screenshot.png">
</details>

<details>
  <!-- The complete lab title goes here 👇🏾-->
  <summary>Lab 2: Title Goes here</summary>
  <!-- Provide path to the screenshot here. Example 👇🏾-->
  <img src="screenshots/example_screenshot.png">
</details>

## Translation code

```
# LAB 1: Google Cloud Fundamentals: Getting Started with Compute Engine

## Objectives:
In this lab, you will learn how to perform the following tasks:
    - Create a Compute Engine virtual machine using the Google Cloud Platform (GCP) Console.
    - Create a Compute Engine virtual machine using the gcloud command-line interface.
    - Connect between the two instances.
##Steps:

1. Create a Compute Engine virtual machine using the GCP Console.
      gcloud compute instances create my-vm-1 --machine-type "n1-standard-1" --image-project "debian-cloud" --image "debian-9-strech-v20198213" --subnet "default" --tags http
      
      gcloud compute firewall-rules create allow-http --action=ALLOW --destination=INGRESS --rules=http:80 --target-tags=http
      
      
2. Create a virtual machine using the gcloud command line.
   1. Choose a zone from the output of this region and use the grep command to filter the results associated with us-central1           region:
   
      gcloud compute zones list | grep us-central1
      
   2. After choosing a zone other than the one assigned to you, create the virtual machine:
   
      gcloud config set compute/zone us-central1-b
      gcloud compute instances create "my-vm-2" --machine-type "n1-standard-1" --image-project "debian-cloud" --image "debian-9-stretch-v20190213" --subnet "default"
      
3. Connect between the two virtual machine instances.
    
    1. Use the ping command to confirm that my-vm-2 can reach my-vm-1 over the network
      - Connect to my-vm-2:
            gcloud compute ssh my-vm-2
      - ping my-vm-1 from my-vm-2:
            ping -c 4 my-vm-1
      - Use the ssh command to open a command prompt on my-vm-1 from my-mv-2:
            ssh my-vm-1
      - At the command 
      
```
