# Cloud-Identity-Access-Management-Project-using-Microsoft-Entra-ID
Hands-on cloud identity management project using Microsoft Azure and Microsoft Entra ID.   Covers tenant setup, custom domain integration with Namecheap DNS, user and bulk user provisioning, group management, MFA configuration, authentication policies, and company branding customization.
![Azure](https://img.shields.io/badge/Cloud-Microsoft%20Azure-blue?logo=microsoftazure)
![Entra ID](https://img.shields.io/badge/Identity-Microsoft%20Entra%20ID-5E5E5E?logo=microsoft)
![IAM](https://img.shields.io/badge/Security-Identity%20&%20Access%20Management-red)
![DNS](https://img.shields.io/badge/DNS-Namecheap-orange)
![Project Type](https://img.shields.io/badge/Project-Cloud%20Security-green)
![Status](https://img.shields.io/badge/Status-Completed-success)


## Table of Contents

- Introduction  
- Tools Used  
- Outlook Account Creation  
- Azure Account Setup  
- Understanding Azure Tenant  
- Microsoft Entra ID Overview  
- Domain Purchase on Namecheap  
- DNS Configuration & Domain Verification  
- User Creation  
- Bulk User Provisioning  
- Group Management  
- Company Branding & Customization  
- Image Resizing Requirements  
- Assigning Custom Domain to Users  
- Security Practices  
- MFA, Conditional Access & PAM  
- Future Improvement
- Key Takeaways
- Skills Demonstrated

# Microsoft Azure & Microsoft Entra ID Setup Documentation

## Introduction
This documentation explains everything I did while setting up Microsoft Azure and Microsoft Entra ID.

Honestly, when I started, Azure looked more complicated than it really is 😩.
But step by step, things started making sense.

This write-up covers:
- Outlook account creation
- Domain purchase on Namecheap
- Azure account setup
- Microsoft Entra ID
- Tenant setup
- Domain integration
- User and bulk user creation
- Branding, customization and image resizing

Basically, everything I touched in Azure.

---

## Tools I Used (So You Know I Didn’t Dream It)

- Outlook (Microsoft account)
- Microsoft Azure Portal
- Microsoft Entra ID (formerly Azure AD)
- Namecheap (for domain purchase)
- Canva / online image resizers

---

## Creating My Outlook Account

Before Azure will even look at you, you need a Microsoft account.

What I did:
1. Went to outlook.com
2. Clicked Create free account
3. Created an Outlook email (admin vibes activated 😎)
4. Verified my account

That Outlook account became the key to everything else.

---

## Creating My Azure Account

Now the real journey started.

Steps:
1. Went to portal.azure.com
2. Logged in with my Outlook account
3. Signed up for Azure (Free trial / Pay-As-You-Go)
4. Entered billing details (yes, card is required, don’t panic)
5. Azure account was successfully created

![Azure Free Account Offer](images/azure-free-account-offer-page.PNG)
![Azure Profile Information](images/azure-account-profile-information-form.PNG)
![Azure Payment Information](images/azure-account-payment-information.PNG)
![Azure Verification Complete](images/azure-account-verification-complete.PNG)
![Azure Welcome Dashboard](images/azure-portal-welcome-dashboard.PNG)

At this point, Azure automatically created a tenant for me.

---

## Understanding Azure Tenant (Very Important)

At first I was confused, but here’s what I learned:

A tenant is like your organization’s home inside Azure.
Everything happens inside it.

Azure automatically gave me:
- A tenant
- A default domain (something.onmicrosoft.com)
- Admin access

So yes, you don’t create tenant manually, Azure does it for you.

![Tenant Overview](images/tenant.PNG)

---

## Microsoft Entra ID (The Brain of Everything)

Microsoft Entra ID is where identity management lives.

This is where I manage:
- Users
- Groups
- Domains
- Branding
- Login experience

How I accessed it:
Azure Portal → Microsoft Entra ID

![Entra Service Overview](images/azure-entra-id-service-overview.PNG)

---

## Buying a Domain on Namecheap

Because onmicrosoft.com is not giving “professional” 😌

What I did:
1. Went to namecheap.com
2. Searched for my preferred domain
3. Purchased the domain
4. Opened the domain dashboard
5. Located Advanced DNS

This domain is what I later connected to Azure.

Due to excitement I spelled my domain name wrong😂, I used it like that tho😜.

![Namecheap Dashboard](images/namecheap-dashboard-home.PNG)
![Domain Search Result](images/namecheap-domain-search-results.PNG)
![Domain Details](images/name-cheap-domain-details.png)

---

## Connecting My Domain to Azure (Entra ID)

This part made me feel like a real cloud engineer 😂.

Steps:
1. Azure Portal → Microsoft Entra ID
2. Clicked Custom domain names
3. Added my domain name
4. Azure generated a TXT record
5. Copied the TXT record
6. Went back to Namecheap → Advanced DNS
7. Added the TXT record
8. Returned to Azure and clicked Verify

![Custom Domain Sidebar](images/entra-custom-domain-sidebar-view.PNG)
![Custom Domain Overview](images/entra-custom-domain-overview.PNG)
![TXT Record Details](images/entra-domain-txt-record-details.PNG)
![Advanced DNS Settings](images/namecheap-advanced-dns-settings.PNG)
![DNS Records Added](images/namecheap-advanced-dns-records.PNG)
![Domain Verification Success](images/entra-domain-verification-success.PNG)

After verification, Azure accepted my domain.

Achievement unlocked ✅

---

## Domain & Tenant Configuration

After domain verification:
- My custom domain became available
- onmicrosoft.com remained as backup
- Users could now use the custom domain to login (nicky@po9cloudsec.online)

![Domain Page](images/Domain.PNG)

---

## Creating Users in Entra ID

Single User Creation:
1. Entra ID → Users
2. Click New user
3. Enter name and username
4. Assign role
5. Save

![Users Page Header](images/entra-users-header.PNG)
![Users List](images/users.PNG)
![Create New User Form](images/entra-create-new-user-form.PNG)
![Single User View](images/entra-users-list-single-user.PNG)
![Edit Username](images/entra-edit-user-username.PNG)
![User Identity Properties](images/entra-user-identity-properties.PNG)

---

## Bulk User Creation (For Big Organizations)

This one is for when you’re tired of creating users one by one.

Steps:
1. Entra ID → Users → Bulk create
2. Download CSV template
3. Fill user details in Excel
4. Upload CSV
5. Validate and submit

Azure does the heavy lifting.

![Bulk Operations Menu](images/bulk-operations-menu.PNG)
![Bulk Create Panel](images/entra-bulk-create-users-panel.PNG)
![CSV Template](images/entra-bulk-user-template-excel.PNG)
![Upload CSV Step](images/entra-bulk-upload-csv-step.PNG)
![Validate and Submit](images/entra-bulk-upload-validate-submit.PNG)

---

## Creating Groups

Groups make life easier.

Steps:
1. Entra ID → Groups
2. Create new group
3. Choose Security or Microsoft 365 group
4. Add users/owners

Instead of managing users one by one, I manage them as a group. Smart move😜.

![Groups Overview](images/Group.PNG)
![Groups Dashboard](images/entra-groups-dashboard.PNG)
![New Group Type Selection](images/entra-new-group-type-selection.PNG)
![Create New Group](images/entra-create-new-group.PNG)
![Add Owner User](images/entra-group-add-owner-user.PNG)

---

## Company Branding & Customization

This was my favorite part because aesthetics matter 😌

Entra ID → Company branding

What I customized:

- Company logo  
- Background image  
- Sign-in text  
- Brand colors  

Now when users sign in, they see the company branding, not plain Microsoft.

![Company Branding Menu](images/company-branding.PNG)
![Branding Overview](images/entra-company-branding-overview.PNG)
![Customize Sign-in Page](images/entra-company-branding-customize-signin.PNG)
![Sign-in Background Branding](images/azure-entra-signin-background-branding.PNG)
![Background Color](images/entra-company-branding-background-color.PNG)
![Sign-in Text](images/entra-company-branding-signin-text.PNG)
![Favicon Upload](images/azure-entra-company-branding-favicon-upload.PNG)

---

## Image Resizing for Branding (Very Important)

Azure is very specific with image sizes.
If the size is wrong, Azure will embarrass you by rejecting it 😭

Recommended Sizes:

Sign-in logo: 280×60 px. PNG with transparent background so it looks neat everywhere.  
Square logo: 240×240 px. This is what shows on profiles and app tiles.  
Background image: 1920×1080 px. JPG or PNG. Don’t put important text near edges or it might get cut off.  
Banner image (optional): 1024×200 px. For headers or fancy landing screens if you want.  
Favicon: 16×16 px or 32×32 px. Tiny icon for browser tabs.

Tools I used:

Canva  
Online image resizers  

![Image Resizer Tool](images/image-resizer-tool-home.PNG)
![Logo Resize Process](images/image-resizer-logo-resize.PNG)

---

## Assigning Domain to Users

After domain verification, I updated user email addresses.

Steps:
1. Entra ID → Users  
2. Select user  
3. Edit username  
4. Change domain to custom domain  
5. Save  

Clean and professional email addresses achieved.

---

## Security Practices I Followed

- I limited admin access to just my primary and mother account  
- Strong passwords(azure are very particular when it comes to to password setting)  
- I kept my default domain as my backup account  
- I added MFA (just so you know, Microsoft have thier own authenticator app)

![Authentication Method Policies](images/entra-authentication-methods-policies.PNG)

---

## MFA, Conditional Access & PAM in Azure

Conditional Access  
Think of Conditional Access like the bouncer at a club with a clipboard.

Rules, rules, rules. You decide: who gets in, when, and how.

Example:
Only company laptops can log in.  
MFA is required if someone logs in from another country.  
Block access if the device is sketchy.

Basically, users don’t always get bothered with MFA, only when the rules say “Hey, prove it.”

PAM (Privileged Access Management)

PAM = VIP security for admin accounts.

Admins are special, if their accounts get hacked, chaos ensues.

So Pam security will say  
“Do you really need admin access right now?”  
“Where are you signing in from?”  
“Prove it with MFA.”

It’s like giving admins a helmet, armor, and a bodyguard, while regular users just have a helmet sometimes.

---

## How They Work Together

General MFA = everyone wears a helmet all the time (boring but safe)  
Conditional Access MFA = helmets only when conditions trigger (smart)  
PAM = VIP admins get helmets, armor, AND bodyguard (serious business)🧑‍💼😎 

---

## Note

This documentation covers everything I did while setting up Microsoft Azure and Microsoft Entra ID.

From being confused at the beginning to understanding how tenants, domains, users, and branding work.

Azure looked scary at first, but once you understand the flow, it actually makes sense.


## Project Overview

This project demonstrates the end to end implementation of Identity and Access Management (IAM) within a Microsoft Azure tenant using Microsoft Entra ID.

The objective of this project was to simulate a real world enterprise identity environment, where users, domains, groups, branding, and security controls are centrally managed in the cloud.

The implementation covers the complete lifecycle of tenant configuration, from account creation and domain integration to user provisioning, bulk operations, branding customization, and security hardening.

## This hands on project showcases practical experience in:
	•	Azure tenant setup and configuration
	•	Microsoft Entra ID identity management
	•	Custom domain verification and integration
	•	User and group administration
	•	Bulk user provisioning using CSV templates
	•	Organizational branding and sign-in customization
	•	Security implementation using MFA and Conditional Access

By completing this project, I gained a deeper understanding of how cloud identity services support secure authentication, authorization, and enterprise governance in modern cloud environments.

This project reflects real administrative tasks performed by Cloud Engineers, IAM Engineers, and Cloud Security Engineers in production environments.

## Skills Demonstrated
	•	Azure Tenant Deployment & Configuration
	•	Microsoft Entra ID Administration
	•	Identity & Access Management (IAM)
	•	User Provisioning (Single & Bulk)
	•	Security Group Management
	•	Custom Domain Integration & DNS Verification
	•	Azure Sign-in Branding Customization
	•	Multi-Factor Authentication (MFA) Implementation
	•	Conditional Access Policy Configuration
	•	Role-Based Access Control (RBAC)
	•	Least Privilege Security Enforcement
	•	Cloud Identity Troubleshooting & Validation

 ## Key Takeaways
	•	Azure tenants serve as the foundation for enterprise identity management
	•	Custom domain integration improves organizational authentication structure
	•	Bulk user provisioning enhances scalability in cloud environments
	•	Security groups simplify access control and permission management
	•	Branding customization improves user authentication experience
	•	Multi-Factor Authentication and Conditional Access strengthen identity security
	•	Proper identity governance is critical for secure cloud administration

## Future Improvements
	•	Implement Azure Conditional Access policies for device and location-based access control
	•	Configure Self-Service Password Reset (SSPR) for improved user autonomy
	•	Integrate Azure AD Connect for hybrid identity synchronization
	•	Implement Privileged Identity Management (PIM) for just-in-time admin access
	•	Enable Azure Identity Protection risk policies for enhanced threat detection
	•	Automate user provisioning using PowerShell or Microsoft Graph API
	•	Integrate tenant authentication with enterprise applications (SSO configuration)

## Author

Love Daniel  
Cloud Engineer | DevOps | Cloud Security

