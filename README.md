# Dockerized OpenResty Deployment with Bitnami  
>This project demonstrates deploying OpenResty using Bitnami Docker images. OpenResty is a high-performance web platform based on Nginx and optimized for serving dynamic web applications.

---

## Table of Contents  
>[About the Project](#about-the-project)<br>  
>[Technologies Used](#technologies-used)<br>  
>[Prerequisites](#prerequisites)<br>  
>[Installation](#installation)<br>  
>[Usage](#usage)<br>  
>[Troubleshooting](#troubleshooting)

---

## About the Project  
>This project sets up an OpenResty instance using Bitnami's pre-configured Docker images. The containerized deployment simplifies the process of running OpenResty and ensures portability, scalability, and ease of use.

---

## Technologies Used  
>**OpenResty:** A high-performance web platform combining Nginx with additional Lua modules.<br>  
>**Docker:** A containerization platform for lightweight and scalable application deployments.<br>  
>**Bitnami Docker Images:** Secure and up-to-date container images for various applications.  

---

## Prerequisites  
>Ensure the following software is installed:  
>>**Docker**
>>>To verify Docker installation:  
```bash  
docker --version  
```  

---

## Installation  

### 1. Pull the Bitnami OpenResty Docker Image  
>Pull the Bitnami OpenResty image from Docker Hub:  
```bash  
docker pull bitnami/openresty  
```  

### 2. Run the Docker Container  

>Run OpenResty using the default settings:  
```bash  
docker run --name openresty bitnami/openresty:latest  
```  

---

## Usage  

>After running the container, OpenResty will be accessible on the specified port.<br>  
>Open a web browser and navigate to:  
   ```  
   http://localhost:8080
   ```
>Use OpenResty to serve your dynamic web applications or test configurations.  

---

## Troubleshooting  

>**Port Conflict:**  
>>If the specified port is already in use, choose a different port:  
   ```bash  
   docker run -p 9100:8080 bitnami/openresty:latest  
   ```  

>**Stopping the Container:**  
>>Stop the OpenResty container with:  
   ```bash  
   docker stop openresty  
   ```  

>**Removing the Container:**  
>>Remove the container to clean up:  
   ```bash  
   docker rm openresty  
   ```  

---
