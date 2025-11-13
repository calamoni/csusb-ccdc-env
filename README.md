## -- Usage Instructions -- 

**Pre-requisite**:
Install Terraform 
> https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli

1. Clone repository
`git clone https://github.com/CSUSB-CISO/csusb-ccdc-env.git`
2. Set variables
Linux
```
export TF_VAR_VIRTUAL_ENVIRONMENT_ENDPOINT="https://YOUR_ENDPOINT:8006"
export TF_VAR_PROXMOX_VE_API_TOKEN='YOUR_API_TOKEN'
```
Windows 
```
$env:TF_VAR_VIRTUAL_ENVIRONMENT_ENDPOINT = 'https://YOUR_ENDPOINT:8006'
$env:TF_VAR_PROXMOX_VE_API_TOKEN = 'YOUR_API_TOKEN'
```
3. Change into desired environment directory and create the environment
```
cd terraform/moon.mine
terraform apply --auto-approve
```

**Note**: You might need to adjust the VMID numbers respective to your environment

