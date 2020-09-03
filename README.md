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
      
      
2. 
```
