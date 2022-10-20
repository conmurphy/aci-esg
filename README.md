# Cisco ACI Configuration: Endpoint Security Groups

Example Nexus as Code Configuration files for setting up ACI with ESGs

See [Nexus as Code](https://developer.cisco.com/docs/nexus-as-code/) for the full documentation.

## Quick Start

- `git clone https://github.com/conmurphy/aci-esg.git`
- `cd aci-esg`
- Update `terraform.tfvars` with your environments details or add the variables as environmental variables
  - `export TF_VAR_aci_username=my_username`
  - `export TF_VAR_aci_password=my_password`
  - `export TF_VAR_aci_url=https://my-apic-url.local`
- `terraform init`
- `terraform plan`
- `terraform apply`

# Notes

- The Terraform code will deploy one tenants with VRF, BDs, Contracts, and ESGs
- It will not configure the L3Domain, AAEP, or VLAN pool
- If using UCS with Fabric Interconnects you will need to configure the Private VLANs

## License

This project is licensed to you under the terms of the [Cisco Sample
Code License](./LICENSE).


