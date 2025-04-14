# SpringBoot-GitHubActions
CICD Implementation using GitHub Actions(Self Hosted Runners)


  buils_docker_image_and_push:
  1. Install maven on self-hosted VM
  3. Install docker on self-hosted VM
  4. sudo apt install docker.io -y
  5. sudo usermod -aG docker ubuntu
  6. sudo chmod 666 /var/run/docker.sock
  7. Update your image tag: <dockerhub username>/<repo name>:latest

  deploy_to_kubernetes:
  1. Create VM
  2. Install AWS CLI and configure it
  3. Install Terraform
  4. Terraform init
  5. Terraform apply
  6. aws eks update-kubeconfig --region <region-name> --name <cluster-name>
  7. Install kubectl
  8. cat ~/.kube/config
  9. Create secrets.EKS_KUBECONFIG
