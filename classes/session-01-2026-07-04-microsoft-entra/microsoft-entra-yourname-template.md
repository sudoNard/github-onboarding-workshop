# My Notes — [ENEH KOSISOCHUKWU]

## Key Concepts I Learned
- Learned that OAuth is a more secure, industry-standard authorization protocol that authenticates users individually using access tokens, allowing APIs to act on behalf of the signed-in user.
- Learned that at runtime, the declarative agent retrieves the stored credentials from the Vault and uses them to authenticate and call the API securely.
- Learned that enabling Proof Key for Code Exchange (PKCE) provides an additional layer of security for OAuth integrations and is recommended by Microsoft.
- Learned that during development, API keys and OAuth credentials can be registered using the Teams Developer Portal or Microsoft 365 Agents Toolkit, while production credentials are typically managed by an administrator.
---

## Lab / Hands-On Work
- I had issues retreiving the actual zip file so i couldnt follow the actual lab on the module but i researched for a lab i could do to understand the topic.

### What I did
I integrated a Microsoft 365 Copilot API plugin with an API secured using an API key while following security best practices by storing the API key in the Microsoft 365 Vault instead of exposing it in the application.

## Tools Used
Microsoft 365 Teams Developer Portal
- Microsoft 365 Copilot
- NASA Open API (Astronomy Picture of the Day API)

### What happened / Result
- first obtained a free API key from the NASA API portal

![alt text](image.png)

- Registered the NASA API key in the Microsoft 365 Vault.
- Verified that the API key is securely stored in the Microsoft 365 Vault and is not exposed in the application.
- Confirmed that the API plugin references the **API Key Registration ID** instead of the actual API key.

## Outcome
The NASA API key was successfully registered in the Microsoft 365 Vault. An API Key Registration ID was generated, enabling Microsoft 365 Copilot to securely retrieve the API key at runtime and authenticate requests to the protected API without exposing sensitive credentials.

### Challenges I faced
- I faced authorization issue because i was using a managed microsoft 365 account.
---

## My Takeaways

- Understood the role of the Microsoft 365 Vault in securely storing API credentials.
- Learned that API plugins reference an **API Key Registration ID** rather than the API key itself.
- Understood that Microsoft 365 Copilot retrieves the API key from the Vault during runtime before making API requests.
- Recognized that storing secrets in the Vault enhances security and allows API keys to be updated without modifying or redeploying the plugin.

---

## Questions I Still Have

<!-- Anything you want to follow up on or ask the mentor -->

-
-

---

## Resources I Found Useful

<!-- Any links, docs, or Microsoft Learn modules you found helpful -->

-

---

*Submitted by: ENEH KOSI · KoceeEneh*
