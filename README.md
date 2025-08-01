# Azure Active Directory & Help Desk Simulation Lab 🖥️

This project simulates a realistic IT environment using Microsoft Azure and Windows Server 2019 to deploy and configure an Active Directory Domain Controller (AD DC) and a Windows 10 client VM. It demonstrates key systems administration and help desk support skills by walking through domain setup, client domain joining, user management, and password reset scenarios.

---

## Project Overview💡

- Deploy and configure Azure VMs for Domain Controller and client
- Promote a Windows Server 2019 VM to an Active Directory Domain Controller
- Configure DNS and Network Security Groups for proper communication
- Join a Windows 10 VM to the newly created domain
- Manage Active Directory users and organizational units (OUs)
- Simulate a help desk ticket workflow for user password reset

---

## Key Skills & Commands Demonstrated 🎯 

- Azure VM provisioning and network configuration  
- Windows Server roles installation and promotion to Domain Controller  
- DNS troubleshooting with `nslookup` and network verification using `ping`  
- Active Directory Users and Computers (ADUC) for user and OU management  
- PowerShell commands such as `Install-WindowsFeature RSAT-DNS-Server`  
- Help desk procedures including password reset and account unlocking  
- Understanding of domain join processes and client VM network settings

---

## Detailed Walkthrough 👀

The full step-by-step configuration and troubleshooting guide is documented in the included **Walkthrough.pdf** file. Refer to it for comprehensive instructions, screenshots, and explanations.

---[Walkthrough Guide (PDF)](https://github.com/Unitech22Pro/ad-helpdesk-lab/blob/main/VM%20deployment_Active%20Directory%20setup_User%20onboarding.pdf)

**Help Desk 101! Just for Fun!** 😃

---

### 🎫 Simulated Help Desk Ticket 💎

> **Ticket ID:** #1428
> **Submitted by:** John Joe
> **Issue:** Unable to log in — password not accepted
> **Priority:** Medium
> **Date Submitted:** 2025-08-01
> **Description:**
> "Hi, I tried to log into my workstation this morning and it keeps saying my password is incorrect. I’m not sure if I forgot it or if something else is wrong. Can someone please reset it for me?"

**Resolution Steps:** 🥸

1. Open **Active Directory Users and Computers**, navigate to your domain → **Users**, and locate the user **John Joe**.
2. Right-click the user, select **Reset Password…**.
3. Enter a temporary password, check **User must change password at next logon**, and unlock the account if locked.

✅ **Outcome:** Password successfully reset. User was able to log in and change password on next sign-in.



## Password Reset Procedure

Below are the critical steps to reset a user’s password in Active Directory:

1. Open Active Directory Users and Computers (ADUC), navigate to your domain, and then to the **Users** folder.  
   
  ![Navigate to ADUC User](https://github.com/Unitech22Pro/ad-helpdesk-lab/blob/main/Step%201%20Navigate%20to%20AD%20DS%20Users%2Bclient.png)


2. Locate the user account needing a password reset, right-click and select **Reset Password...**. Here, you can unlock the account and enforce password change at next login.
   
  ![Confirm Client Password Reset](https://github.com/Unitech22Pro/ad-helpdesk-lab/blob/main/Step%201%20Navigate%20to%20AD%20DS%20Users%2Bclient.png)

---

### 🛠️ Technician Response

> **Response by:** (Your Favorite Helpdesk Specialist)
> **Date:** 2025-08-01
> **Status:** Resolved
> **Response:**
> Hi John,
>
> I’ve reset your password and set it to require a new one at your next login for security. You can now log in using the temporary password provided via secure message. If you continue experiencing issues or need further assistance, feel free to reach out.
>
> 🔐 *Reminder:* Please choose a strong, memorable password and avoid reusing old credentials.
>
> Thanks,
> – Unitech22Pro | IT Support Technician

**Ticket Status:** ✅ Closed
**Resolution:** Password reset completed and user confirmed successful login.

