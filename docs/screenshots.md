# Screenshots


#Architecture Diagram- Metaverse IAM 

<img width="940" height="292" alt="image" src="https://github.com/user-attachments/assets/dde97d91-ab01-49d9-bd9e-82b7ac90e699" />


## Figure 1
**Metaverse IAM Lab virtual machine environment overview**  

<img width="940" height="623" alt="image" src="https://github.com/user-attachments/assets/a0d7aa0b-c3c9-43c8-8d0a-e8a8e53d690d" />

Shows the VMware-based environment hosting the lab infrastructure.

## Figure 2
**Microsoft Entra Connect Sync running on VM for hybrid identity synchronization**  

<img width="940" height="638" alt="image" src="https://github.com/user-attachments/assets/2fcb1e81-dea7-4caf-b80a-d4a594127db3" />

Shows the sync component connecting on-prem AD to Entra ID.

## Figure 3
**Active Directory organizational structure supporting identity governance inputs**  

<img width="940" height="722" alt="image" src="https://github.com/user-attachments/assets/3aee90ef-5aad-47c6-9dcb-6da5ffcc3b57" />

Shows the AD layout and identity containers.

## Figure 4
**Test Windows identity with lifecycle attributes used for provisioning decisions**  

<img width="940" height="776" alt="image" src="https://github.com/user-attachments/assets/9105180a-ebde-44ea-bff9-f407d3ed2b59" />

Shows governance-driving identity attributes sourced from AD.


## Figure 5A
**SailPoint AD connector configuration for identity aggregation and provisioning** 

<img width="940" height="387" alt="image" src="https://github.com/user-attachments/assets/0aadd27f-588a-4a9b-a843-55e1c26b7229" />

## Figure 5B
<img width="940" height="619" alt="image" src="https://github.com/user-attachments/assets/90ff8001-b8b6-4f74-9585-7e912b5f76ef" />
Figure 5B: SailPoint search scope and connection validation for Active Directory integration

Shows IIQ application settings for AD integration.

## Figure 7
**Identity mapping and governance inputs used for lifecycle-based automation**
<img width="940" height="336" alt="image" src="https://github.com/user-attachments/assets/22d9337f-b0c8-48ac-9b2d-b399deab9a50" />


Shows primary source mappings for identity attributes.

## Figure 8
**Lifecycle event configuration supporting automated JML processing**  

<img width="940" height="245" alt="image" src="https://github.com/user-attachments/assets/a472f714-e4ba-4588-8fd3-dcf7dd6435b8" />


Shows Joiner, Mover, and Leaver events.

## Figure 9
**Joiner workflow logic used to evaluate identity attributes and assign governed access**  
<img width="940" height="372" alt="image" src="https://github.com/user-attachments/assets/b9ed43bf-0a4d-4bb1-9a91-68a12f30ba04" />

Shows BP_JML_Joiner workflow structure.

## Figure 9A

<img width="940" height="296" alt="image" src="https://github.com/user-attachments/assets/d73056db-21f6-413a-8721-5cbc74863bee" />

Figure 9A: Shows BP_JML_Mover workflow structure.


## Figure 9B

<img width="940" height="394" alt="image" src="https://github.com/user-attachments/assets/9821d8ab-8c47-4e2b-8a9b-c736afcaaae3" />

Figure 9B: BP_JML_Leaver  workflow logic used to evaluate identity attributes and assign governed access

## Figure 10
**Business role and entitlement structure used for governed access assignment**  

<img width="940" height="536" alt="image" src="https://github.com/user-attachments/assets/5ce97c8a-ea5f-41e3-8216-4bace1b919c0" />

Shows the role-based access model.

## Figure 11
**Workgroup and ownership structure supporting access accountability**  

<img width="940" height="284" alt="image" src="https://github.com/user-attachments/assets/30a792e1-300c-48d8-8ab4-c225fe54925a" />

Shows workgroups supporting delegated governance.


## Figure 12-15
**Hybrid identity and cloud visibility**  

<img width="940" height="563" alt="image" src="https://github.com/user-attachments/assets/7776933b-cf19-4862-8ef8-68c99a333140" />

<img width="940" height="447" alt="image" src="https://github.com/user-attachments/assets/66b84d97-b907-41a7-83d2-a1df75193cc7" />

<img width="940" height="424" alt="image" src="https://github.com/user-attachments/assets/e9e607fc-2caf-4f35-a450-ead911346e3c" />

<img width="940" height="330" alt="image" src="https://github.com/user-attachments/assets/0a21a012-edf2-4cbd-89ea-cab8dd53634a" />


Shows synced users, synced groups, and Entra Connect health.


## Figure 16-21

<img width="1047" height="842" alt="image" src="https://github.com/user-attachments/assets/8503a28d-35f4-4825-b0a9-5ce6eb72512d" />

Figure 20-21: Troubleshooting and validation evidence across connector, certificate, Tomcat, and governance layers

<img width="1011" height="1447" alt="image" src="https://github.com/user-attachments/assets/6f8ed998-aeca-4e11-a30e-a40b72eb7c56" />

Figure 5: Server runtime and service validation across the IAM platform



## Figure 22-25

**Final governed state and operational validation across the IAM flow**  

<img width="940" height="401" alt="image" src="https://github.com/user-attachments/assets/5a9ae6bd-fdf2-41b8-9052-14bc84a168be" />

<img width="940" height="407" alt="image" src="https://github.com/user-attachments/assets/dcd928b8-dcf0-4e61-8118-72e924915276" />

<img width="940" height="419" alt="image" src="https://github.com/user-attachments/assets/d3a59fa2-9f04-460e-9aef-3df049386171" />

<img width="940" height="255" alt="image" src="https://github.com/user-attachments/assets/7101558a-ba74-4e57-b19c-0ac3bfc5454e" />

<img width="940" height="221" alt="image" src="https://github.com/user-attachments/assets/dda79b75-6aa0-4ff7-9fbc-98d60fef773c" />

Figure 19: Provisioning engine result showing committed role and group updates

<img width="940" height="722" alt="image" src="https://github.com/user-attachments/assets/ec2ae41b-0acb-4dc9-9e66-dbed22099e9d" />
Figure 20: Active Directory group membership validation after provisioning



Shows successful scheduled task execution, approvals, provisioning, ownership, and final operational state.
