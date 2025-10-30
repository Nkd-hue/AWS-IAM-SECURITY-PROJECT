 AWS IAM Security Project

 Overview
This project demonstrates how to strengthen cloud security by using **AWS Identity and Access Management (IAM)** to manage permissions and access to **EC2 instances**.  
It reflects my ability to apply IAM concepts such as least privilege, policy simulation, and access control in a real-world environment.



 Services Used
- **Amazon EC2** – for creating and managing virtual machines
- **AWS IAM** – for managing users, groups, and permissions
- **Policy Simulator** – to test IAM policies safely before implementation
- **AWS Management Console**

 Key Tasks Performed
1. Created and launched multiple **EC2 instances**
2. Configured **IAM users** and **groups**
3. Created **custom IAM policies** and attached them to groups
4. Used **Account Alias** for a personalized AWS sign-in URL
5. Tested permissions using **IAM Policy Simulator**
6. Controlled access to specific EC2 instances using **tags and policy conditions**

---

 Testing Permissions
I used the **IAM Policy Simulator** to test specific actions like:
- `ec2:StopInstances`
- `ec2:DeleteTags`

Initially, both were denied due to attached policies.  
After modifying the “Stop Instances” policy to include the `development` tag condition, access was approved — demonstrating **granular access control** in action.



 Tagging Structure
| Tag Key | Tag Values |

| nextwork-dev-nadia | production, development |

This allowed selective instance management while maintaining compliance with least privilege principles.



 Lessons Learned
- Importance of IAM in enforcing secure access
- How to simulate permissions before deployment
- Real-world tagging strategies for access control
- Practical use of the principle of least privilege

About Me;
Hi, 
I’m **Nadia Kroduah**, a passionate **Cloud & Cybersecurity student** dedicated to building secure and scalable environments.  
This project is part of my continuous learning journey in **AWS**


