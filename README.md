# Azure-AD-Authentication-for-Azure-Files---Implementation-Review

# Enabling Azure AD Authentication for Azure Files
- Azure Files does not directly interact with Azure AD. 
- They have an implementation with Azure AD Domain Services


# Create your own Azure AD Domain Services #272
- Properties > Select the virtual network created when creating Azure AD DS > DNS Servers > Place private IP addresses in the custom and click save
- Create a new virtual machine in that virtual network
- Join the virtual machine to a domain (ensure that one Azure AD users is in the AAD DC Administrator group)
- Username and PW will be prompted. Reset the password at least once.
- Now join the domain and restart and then log in to the Azure VM as the Azure Admin user.
