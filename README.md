#  DevOps Task 3 – Infrastructure as Code (IaC) with Terraform

##  Objective
Provision a **local Docker container** using **Terraform** to understand Infrastructure as Code (IaC).

---

##  Tools Used
- **Terraform**
- **Docker**
- **Windows PowerShell**

---

##  Files in this Repository

| File Name          | Description                                      |
|--------------------|--------------------------------------------------|
| `main.tf`          | Terraform config to provision an Nginx container |
| `apply_log.txt`    | Output of `terraform apply` command              |
| `destroy_log.txt`  | Output of `terraform destroy` command (optional) |
| `README.md`        | This documentation file                          |

---

## Steps to Run the Project

###  Prerequisites
- Docker Desktop must be **installed and running**
- Terraform installed on your system
- Run terminal as **Administrator**

---
### Clone the Repo
git clone https://github.com/vishwajeet937/terraform-docker-container.git

cd terraform-docker-container

###  Step-by-Step Commands

#### Initialize Terraform
```bash
terraform init
terraform plan
terraform apply -no-color | tee apply_log.txt
Type *yes* when prompted.

### Check the Running Container
Open your browser and go to:

http://localhost:8080

You should see the Nginx Welcome Page.

###  Clean Up (Destroy the Infrastructure)
terraform destroy -no-color | tee destroy_log.txt
Type *yes* when prompted.


### Author
vishwajeet Kumar
DevOps Intern
