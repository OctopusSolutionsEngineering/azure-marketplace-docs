# Octopus Deploy (self-managed application) Azure Marketplace listing 

Octopus Deploy is the leading DevOps automation platform that enable organizations to deploy your software to multi-cloud, hybrid, and on-premises environments with ease. 

Octopus is available as a hosted solution as well as a self-managed solution on-prem or in a company's cloud of choice. Octopus licenses can be purchased direct from Octopus.com or the Azure Marketplace. 

Octopus Deploy has a self-managed Azure Application which enables customers to get a bootstrapped Octopus instance up and running quickly that they can customise to meet their organisations needs. 

# Octopus Administration tasks 

The Octopus Azure Application is self-managed which means that your organization configures and scales it to meet your needs. 

* Octopus Deploy does not have any access to your managed resource group. This configuration means that you self-manage your installation and you can contact [Octopus support](https://octopus.com/support) for assistance. 
* Organizations have full access to the Azure Application managed resource group. This configuration means that you have full access to self-manage and adminster your Ocotpus isntance. 

The Octopus Azure application includes the following core Azure resources. 

This listing includes some of the following resources. 
* Azure virtual machine 
* Azure SQL instance

## Configuring HTTPS 

The Octopus Deploy Azure Managed Application does not include an HTTPS certificate. It is pre-configured to allow HTTPS traffic but we strongly recommend our review the network configuration and configure it to meet your needs. 

1. Navigate to the Octopus Deploy Azure Application and Managed Resource Group
2. Allow Remote Desktop Protocol network traffic (RDP) so you can remote into the virtual machine running Octopus Deloy
3. Remotely connect to the Octopus Deploy virtual machine.
4. Start the Octopus Manager Application
5. Configure HTTPS traffic as per [Octopus documentation](https://octopus.com/docs/security/exposing-octopus/expose-the-octopus-web-portal-over-https).
6. Allow HTTPS traffic (port 443) and disallow HTTP traffic (port 80) to your virtual machine. 
7. Disallow RDP network traffic (Port 3389) access.
8. Validate that you connect to your Octopus instance securely via it's DNS name or IP address. 

# Support 

Navigate to the [Octopus support page](https://octopus.com/support) to contact us for help.
