# Generate TOTP Using an Encrypted Secret Key - MFA - #57746

**Type:** User Story
**Status:** In Progress
**Assigned To:** Unassigned
**Area Path:** Avo EEC
**Iteration:** Avo EEC

## Description
As a test automation engineer,I want to generate a Time-based One-Time Password (TOTP) using an encrypted MFA secret key,So that I can automate applications protected by Multi-Factor Authentication (MFA) without storing or exposing the secret key in plain text.The TOTP secret will be encrypted using the existing Avo Encryption Utility (AES-256-GCM) during test design. During test execution, the new Generate TOTP keyword will accept the encrypted secret, decrypt it only in memory, generate the OTP using the RFC 6238 standard, return the OTP, and immediately remove the plaintext secret from memory. 
Keyword name : Generate TOTPInput Value : Place Holder in UI <Encrypted Secret Key>Output Value : {Dynamic Variable} - This will store the TOTP code generated using Encrypted Secret Key 
Test Step Description in Report:Enter secure secret key '**************' in the '<Object Name>' to generate TOTP.

---
[View in Azure DevOps](https://dev.azure.com/AvoAutomation/Avo%20EEC/_workitems/edit/57746)