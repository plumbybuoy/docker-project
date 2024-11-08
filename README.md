DevOps project where I deployed Jenkins on a Docker container using a Google Cloud Platform N2 VM. Here's a quick breakdown of how I achieved this:


>>Provisioned a GCP N2 VM:

 Choose an N2 instance for optimal performance.

>>Installed Docker:

 Set up Docker on the VM with a streamlined Bash script.

>>Pulled Jenkins Docker Image:

 Utilised Docker Hub to pull the Jenkins image:

>>docker pull jenkins:2.60.3

 Ran Jenkins in a Container:

>>Launched Jenkins, making sure to map necessary ports and volumes:

 docker run -d -p 8080:8080 -p 50000:50000 --name jenkins-app-1 jenkins:2.60.3

>>Accessed Jenkins Interface:

 Configured Jenkins by accessing it through the browser at  http://<GCP_VM_IP>:8080.
