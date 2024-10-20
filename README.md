# Terraform-S3bucket
 Project we will be using Terraform and AWS Cloud to set up static website.
## Prerequisite
 1. AWS Account
 2. Terraform Installed
 3. Vscode editor
### Steps:
 1. **Create an S3 Bucket**: Start by creating an S3 bucket to store your website files. The bucket name should be globally unique across all AWS accounts.
 2. **Step 2: Configure Bucket for Static Website Hosting**: In the S3 bucket properties, enable static website hosting and specify the default index document and              optional error document.
 3. **Upload Website Files**: Upload your static website files HTML to the S3 bucket. Make sure to set appropriate permissions for the objects to make them publicly            accessible.
 4. **Enable Public Access**: Allow public access to the S3 bucket and its objects by configuring the bucket policy or Access Control Lists (ACLs).
 5. **Testing the Website**: Once the setup is done, you can test your static website by accessing it through the S3 bucket URL or your custom domain.

**terraform init**<br>
<img width="476" alt="Screenshot 2024-10-20 205908" src="https://github.com/user-attachments/assets/7ca72f67-6f98-4447-b6dd-6c30e120b437"><br>
**terraform plan**<br>
<img width="731" alt="Screenshot 2024-10-20 210023" src="https://github.com/user-attachments/assets/640a9b90-0f17-48ed-8a89-975964e95563">

<img width="704" alt="Screenshot 2024-10-20 210048" src="https://github.com/user-attachments/assets/e1b3be87-5821-4f5a-bb95-97fb3026e741"><br>
**terraform apply**<br>
<img width="696" alt="Screenshot 2024-10-20 214327" src="https://github.com/user-attachments/assets/988e72c5-7f13-4a54-82cf-b5bcda5387a8"><br>

<img width="407" alt="Screenshot 2024-10-20 214343" src="https://github.com/user-attachments/assets/5fb00717-4ed9-41fb-ac6f-383478c6dc23"><br>
**Go to aws account and open S3 bucket you can see the bucket created automatically this happens because it can pull credentials from these secure sources: AWS CLI, environment variables, IAM roles, or AWS profiles.** <br>
<img width="746" alt="Screenshot 2024-10-20 221430" src="https://github.com/user-attachments/assets/ba344dfd-22f3-4f16-9319-c0d5cdbd4ce3"><br>
**Click on the S3 bucket**<br>
**Go to properties**<br>
<img width="725" alt="Screenshot 2024-10-20 221501" src="https://github.com/user-attachments/assets/c0cca226-b691-48ed-a164-0ff5a2e1842f"><br>
**Scroll down static website hosting**<br>
<img width="682" alt="Screenshot 2024-10-20 221526" src="https://github.com/user-attachments/assets/db87ba42-b567-4455-a31f-c45e073b10f7"><br>
**Open the website in new page**<br>
<img width="1095" alt="Screenshot 2024-10-20 214414" src="https://github.com/user-attachments/assets/e81733b4-46db-4959-bba0-c1d522287607"><br>
**After checking the website destroy the S3 bucket**<br>
**terraform destroy**<br>
<img width="683" alt="Screenshot 2024-10-20 215140" src="https://github.com/user-attachments/assets/3caab834-3fe9-459c-b657-54d035eecf7f"><br>
<img width="652" alt="Screenshot 2024-10-20 215158" src="https://github.com/user-attachments/assets/387c8dee-1716-41f7-add8-3302fff33c91"><br>
# You have succesfully created S3 bucket and hosted a static website using terraform.
