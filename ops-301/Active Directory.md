# ***[What is Active Directory?](https://www.cyberark.com/what-is/active-directory/)***
### What exactly is “Active Directory” and are the key services it provides?
Active Directory (AD) is Mircrosoft's directory and identity management service for windows domain networks.
* ***Key Services it provides:***
  * Active Directory Domain Services (AD DS) – the core Active Directory service used to manage users and resources.
  * Active Directory Lightweight Directory Services (AD LDS) – a low-overhead version of AD DS for directory-enabled applications.
  * Active Directory Certificate Services (AD CS) – for issuing and managing digital security certificates.
  * Active Directory Federation Services (AD FS) – for sharing identity and access management information across organizations and enterprises.
  * Active Directory Rights Management Services (AD RMS) – for information rights management (controlling access permissions to documents, workbooks, presentations, etc.)
### What are the differences between a domain, forest, and tree in Active Directory?
* A domain is a collection of objects (e.g. users, devices) that share the same Active Directory database. A domain is identified by a DNS name like company.com.
* A tree is a collection of one or more domains with a contiguous namespace (they have a common DNS root name like marketing.company.com, engineering.company.com, and sales.company.com).
* A forest is a collection of one or more trees that share a common schema, global catalog, and directory configuration—but aren’t part of a contiguous namespace. The forest typically serves as the security boundary for an enterprise network.
### How can objects (e.g. users, devices) within a domain be grouped?
Objetcs within a domain can be grouped into organization units (OUs) to simplify administration and policy managements. Administrators can create arbitrary organizational units to mirror functional, geographical, or business structures, and then apply group policies to OUs to simplify administration. OUs also make it easier to delegate control over resources to various administrators.
### Explain the benefits of Active Directory, as you would to a family member.
Just imagine Active Directory as a big family for computers and users. Just like a family organizer helps keep track of everyone's schedules, Active Directory keeps track of who's and what they can do on the computer network.
* Security – Active Directory helps businesses improve security by controlling access to network resources.
* Extensibility – companies can easily organize Active Directory data to align with their organizational structure and business needs.
* Simplicity – administrators can centrally manage user identities and access privileges across the enterprise, helping businesses simplify management and reduce operations expenses.
* Resiliency – Active Directory supports redundant components and data replication to enable high availability and business continuity.
