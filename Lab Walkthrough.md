# Network Load Balancer Lab Walkthrough

This walkthrough documents the exact steps I completed while building a Layer 4 Network Load Balancer on Google Cloud.

---

## Task 1: Set Default Region and Zone

Configured Cloud Shell defaults:
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d36a2648-c9c9-437d-ad7e-b1107a792ce7" />

---

## Task 2: Create web server instances
Created three VM instances (`www1`, `www2`, `www3`) with Apache installed and unique homepages.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/1b070eca-1b71-4a74-bf0e-20a71a662868" />

Create a firewall rule to allow external traffic to the VM instances.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/560566da-09b9-4597-a6ac-7e48a6986383" />

Verify Instances are running
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/98b17ae5-e50a-4be0-a16e-82094b43886b" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/750d472e-f654-465e-a1d6-9e8ab8b7bef4" />

---
## Task 3: Configure the load balancing server
Create a static external IP address for the load balancer
<img width="1914" height="412" alt="image" src="https://github.com/user-attachments/assets/9d44ed5c-baf4-4f2f-a19a-85598fd786e8" />
Add a legacy HTTP health check resource
<img width="1915" height="314" alt="image" src="https://github.com/user-attachments/assets/c88e1553-83fe-439d-b613-b35f8235ff14" />

---
## Task 4: Create the target pool and forwarding rule
Create the target pool and use the health check
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0a97df07-d847-4881-b50a-98ec5f0b4f16" />

Add the instances to the pool
<img width="1919" height="399" alt="image" src="https://github.com/user-attachments/assets/e5d977ce-0134-4607-9b2d-d3e5458dc456" />

Add a forwarding rule
<img width="1919" height="366" alt="image" src="https://github.com/user-attachments/assets/48f15b67-1439-474f-b0f2-d5933f40cc03" />

---

## Task 5: Send traffic to your instances
View the external IP address of the www-rule forwarding rule used by the load balance
<img width="1919" height="420" alt="image" src="https://github.com/user-attachments/assets/fcf78afd-9424-4b10-b2db-81ef2a0c0915" />

Access and show the external IP address
<img width="1919" height="157" alt="image" src="https://github.com/user-attachments/assets/5ec2c9ba-9e84-4641-b43c-081c654a99fc" />










