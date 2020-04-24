# aelf DAO Bounty Project Instruction

Chinese version tutorial URL: [dao-member-management-zh](https://github.com/DAO-Testnet/Bounties/blob/master/operation-guide-zh.md)

The aelf DAO Management Committee provides community users two ways to participate in aelf’s development, encouraging an active ecosystem: Grant Projects and Bounty Projects:

* [Grant Projects](https://github.com/DAO-Testnet/Grants): When community users have good project ideas that will be beneficial to the aelf ecosystem, they can apply as a Grant project. The Committee will provide resources to aid the project’s development.
* [Bounty Projects](https://github.com/DAO-Testnet/Bounties): When the Committee sees the need to enhance aelf’s ecosystem, a Bounty project will be launched to allow community users to assist in project development.

Here are the[ bounty project](https://github.com/DAO-Testnet/Bounties) steps:

## (1) Introduction
The aelf DAO Management Committee makes decisions for the ecosystem of an open-source project through decentralized governance, while also providing financial support to developers in the aelf community.

## (2) aelf DAO funds planning
It is up to the Committee and any willing investors to decide the amount of the reward and the rules for its payment.

## (3) aelf DAO Users Guideline 
Process Overview:

![图片](https://uploader.shimo.im/f/ZbXP7m0xiolZiTW3.png!thumbnail)

Note: 

* The VOTE Token referendum proposal is a community members’ pre-approval of the  project (non-essential steps)
* Proposals 3 is the step for aelf DAO management committee to choose the developer, which is optional. But, it might be required according to the rule of Bounty project.

The following steps do not include the referendum proposal on the Non-ELF DAO ecosystem.

 

### Step 1: Release
**1.1  ****off-chain release outside the chain**

From the [GitHub repository for 'Bounty Projects'](https://github.com/DAO-Testnet/Bounties), developers need to open up the [projects-template.md](https://github.com/DAO-Testnet/Bounties/blob/master/projects-template.md) to check the project requirements and copy the content.

![图片](https://uploader.shimo.im/f/jY5Fg2St77kRkrVG.png!thumbnail)

Figure 1.1 - aelf DAO Management Committee copy projects-template

 

Click '[project-apply](https://github.com/DAO-Testnet/Grants/tree/master/projects-apply)' and select the appropriate year and quarter folder.

![图片](https://uploader.shimo.im/f/lUpr4SfB1zugR5en.png!thumbnail)

Figure1.2 -  aelf DAO Management Committee go to projects folder 

 

The Committee member needs to clicks ‘Create new file’ to Create the project application file.

![图片](https://uploader.shimo.im/f/9kJbABdowadzLnVM.png!thumbnail)

Figure1.3 - aelf DAO Management Committee create project application file 

 

Paste the copied content of the [projects-template.md](https://github.com/DAO-Testnet/Bounties/blob/master/projects-template.md) into the current file, and make additions and changes based on the project request (Markdown format is available, and the file title suffix is ‘.MD’). Click ‘Propose new file’ to publish the file.

![图片](https://uploader.shimo.im/f/nFHVSWY1IuJwxHYz.png!thumbnail)

![图片](https://uploader.shimo.im/f/FP4VFsTfynQTHlBU.png!thumbnail)

 Figure 1.4 - aelf DAO Management Committee editing and publishing application file

 

After proposing a file, the Committee member will enter the following page and click ‘create pull request’ to create a pull request, that is, ‘pr’.

![图片](https://uploader.shimo.im/f/KIfYdLU3DXR4z1BD.png!thumbnail)

Figure 1.5 - aelf DAO Management Committee creates pr-step 1

 

After the Committee member enters a brief description of the project application (optional), Click ‘Create pull request’ and the project pr is created.

![图片](https://uploader.shimo.im/f/35h1jCUcoNgpIGX3.png!thumbnail)

Figure 1.6-aelf DAO Management Committee creates pr-step 2

 

**1.2 Release**** on the Chain:**

After the Committee submits a pr (pull request) on Github, go to the [proposal page](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply) and apply for Association Proposal in the aelf Explorer and fill in the following:

![图片](https://uploader.shimo.im/f/zseYujbSuEIaw4BC.png!thumbnail)

Figure 1.7 -  aelf DAO Management Committee apply for proposal

* Proposal Mode: Association
* Organization: aelf DAO Management Committee
* Contract Address: aelf DAO Contract Address
* Method Name: ProposeRewardProject
* Method Params: GitHub pr (pull request) link, Git commit ID, pre-approval proposal ID (optional)
* URL: Provide a link to describe the proposal, which can be GitHub pr (pull request) link (optional)
* Expiration Time: You need to choose the right time period, ensure that it does not affect project development and organization’s members have enough time to vote. (Suggestions: 7 days for Small and medium-scale projects, 14 days for large-scale projects.) 

Approved project proposals will be displayed on the proposal page.

After you apply for a proposal, you can synchronize the proposal link with the PR conversation to ensure that the information on Github corresponds to the information on the chain.

 

### Step 2: Review
After the pr (pull request) and the proposal submission, aelf DAO Management Committee members will receive the request on Github and the aelf Explorer.

2.1 Chain Review - Vote on the proposal: The aelf DAO Management Committee and the production nodes first vote on the proposal in two rounds in the aelf Explorer (Agree / Disagree / Abstain):

1. Round 1 Voting: aelf DAO Management Committee chooses the project and votes on the proposal (Agree / Disagree / Abstain).
2. Round 2 Voting: After the round 1 voting, aelf DAO Management Committee are required to execute the proposal before applying for the same Parliament Proposal.

 

Data on Application Proposals:

* Proposal Mode: Parliament
* Organization: Production Nodes Organizations
* Contract Address: aelf DAO Contract Address
* Method Name: ProposeIssueRewardProject
* Method Params: Project ID, application for funding plan (Support for multiple phases and multiple developers)
* URL: Provide a link to describe the proposal, which can be GitHub pr (pull request) link (optional)
* Expiration Time: You need to choose the right time period, ensure that it does not affect project development and that the organization’s members have enough time to vote. (Suggestions: No more than 7 days) 

 

1. Round 2 voting: The production node votes on the proposal.

When the vote is passed, it means that the proposal is approved. Funding will be automatically released if the proposal is implemented successfully by a Committee member before it expires.

![图片](https://uploader.shimo.im/f/hKF5Cekh2k4zBCHl.png!thumbnail)

Figure 2.1-voting

 

2.2 Off-chain Review - Merge the pr (pull request) on GitHub: After the Committee member executes the proposal, and they will Merge the pr (pull request). After the Merge, you can view the project application file in the [project](https://github.com/DAO-Testnet/Bounties/tree/master/projects/2020) folder.

During the review process, if the Committee reaches a new consensus on the content of the project application, they need to modify the pr (pull request).

![图片](https://uploader.shimo.im/f/VcUIy2w1Ls8eE3nr.png!thumbnail)

Figure 2.2 - Merge pr (pull request)

 

### Step 3: Select the developer (non-essential step)
**3.1 Developers’ off-chain application**

Depending on the project release document, the developer chooses whether or not to apply to develop the project. After the developer has decided to develop, he or she will need to open up the [apply-template.md](https://github.com/DAO-Testnet/Bounties/blob/master/apply-template.md) in the [GITHUB ‘bounty project’ repository](https://github.com/DAO-Testnet/Bounties) to check the project release requirements and copy the document content. The template is for reference only and specific content can be supplemented or modified according to the project release documents: 

![图片](https://uploader.shimo.im/f/CbC1UDm6g4Am058u.png!thumbnail)

Figure 3.1 - Developers copy apply-template

 

The developer visits the [apply-docs](https://github.com/DAO-Testnet/Bounties/tree/master/apply-docs) folder for the corresponding project.

![图片](https://uploader.shimo.im/f/goM72rCsPviKvcSX.png!thumbnail)

Figure2 - developers visit apply-docs folder 

Paste the copied content of the [apply-template.md](https://github.com/DAO-Testnet/Bounties/blob/master/apply-template.md) file into the current file and make additions and changes based on the project request (Markdown format is available, and the file title suffix is ‘.MD’). Click ‘Propose new file’ to publish the file. After submitting the document, developers can create a pr (pull request). The detailed procedure is referred to in Step 1: Release.  

![图片](https://uploader.shimo.im/f/h6fk1vLds2Pslsbj.png!thumbnail)

Figure 3.3 - Developers create project application file 

 

**3.2 Applications on the Chain:**

After visiting the[ ](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply)[proposal page](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply) to apply for association proposal in aelf Explorer, fill in the following:

![图片](https://uploader.shimo.im/f/vYj0lU6uFUXgb3t7.png!thumbnail)

Figure 3.4 - Developers apply for proposal

* Proposal Mode: Association
* Organization: aelf DAO
* Contract Address: aelf DAO Contract Address
* Method Name:ProposeTakeOverRewardProject or ProposeDevelopersAudition (This approach is used by more than one developer.
* Method Params: GitHub pr (pull request) link, Git commit ID, pre-approval proposal ID (optional)
* URL: Provide a link to describe the proposal, which can be GitHub pr (pull request) link (optional)
* Expiration Time: You need to choose the right time period, to ensure that it does not affect project development and that organization’s members have enough time to vote. (Suggestions: No more than 7 days) 

 

Approved project proposals will be displayed on the proposal page.

After you apply for a proposal, you can synchronize the proposal link with the pr (pull request) conversation to ensure that the information on Github corresponds to the information on the chain.

 

**3.3 aelf DAO Management Committee Review**

After the pr (pull request) and the proposal submission, the Committee will receive the request on Github and the aelf Explorer.

Vote on the proposal: The Committee will first vote on the proposal in the aelf Explorer (Agree / Disagree / Abstain):

![图片](https://uploader.shimo.im/f/rVdGrO2kHQMgNfHV.png!thumbnail)

Figure 3.5 - Voting

 

After the vote, the developer is required to execute the proposal before it expires and the Committee will Merge the developer's submitted pr (pull request) in Github and designate the developer to develop the project.

![图片](https://uploader.shimo.im/f/uYvq7rjR1C0m7PzK.png!thumbnail)

Figure 3.6 - Merge developers submitted pr (pull request)

 

**3.4 Off-chain Discussion**

During the review period, if the project needs to be discussed between developers and the Committee, the Issue for this project could be created by the either party for discussion.

![图片](https://uploader.shimo.im/f/EjJOtyEXjIqM2sja.png!thumbnail)

Figure 3.7 - Creating  project Issue for discussion 

### Step 4: Development and Delivery
4.1 Off-chain Delivery: Developers are required to follow the plan of the project application document and submit the Development Delivery document (reference template:[ ](https://github.com/DAO-Testnet/Bounties/blob/master/deliver-template.md)[deliver-template](https://github.com/DAO-Testnet/Bounties/blob/master/deliver-template.md). Markdown format is available and the file title suffix is ‘.MD’). After submitting the document, developers can create a pr (pull request). The detailed procedure is referred to in Step 1: Release. The development delivery document is recommended to be named: ‘Project Name’-’stage’-‘development delivery File’.

![图片](https://uploader.shimo.im/f/o06CdcZsgWQca9g2.png!thumbnail)

Figure 4.1 - developers visit deliver-docs folder

If the project needs to be developed in multiple stages, a folder for each stage of the project will need to be created in the[ deliver-docs](https://github.com/DAO-Testnet/Bounties/tree/master/deliver-docs) folder and documents submitted to the corresponding folder according to the stage plan. After submitting the document, developers can create a pr (pull request). The detailed procedure is referred to in Step 1: Release.

![图片](https://uploader.shimo.im/f/xmuIvuRa3qkAhR3q.png!thumbnail)

Figure 4.2 - Developers create a project folder for deliver-docs

 

4.2 Deliver on the chain:

After the developer submits the Pr on Github, visit the [proposal page](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply) to apply for association proposal in aelf Explorer and fill in the following:

![图片](https://uploader.shimo.im/f/S8BTNUkwXCNPe93m.png!thumbnail)

Figure 4.3 - Developers apply for proposal

* Proposal Mode: Association
* Organization: aelf DAO Management Committee
* Contract Address: aelf DAO Contract 
* Method Name: ProposeDeliver
* Method Params: Project ID, GitHub Pr Link, Git commit ID, index of the grant application
* URL: Provide a link to describe the proposal, which can be GitHub Pr link (optional)
* Expiration Time: You need to choose the right time period, ensure that it does not affect project development and that the organization’s members have enough time to vote. (Suggestions: No more than 7 days)

 

Approved project proposals will be displayed on the proposal page.

After you apply for a proposal, you can synchronize the proposal link with the pr (pull request) conversation to ensure that the information on Github corresponds to the information on the chain.

 

### Step 5:  Funds Release
5.1 Chain Review - Vote on the proposal: The Committee will review and vote on the proposal in the aelf Explorer (Agree / Disagree / Abstain):

After the proposal is accepted, the developer must execute the proposal before it expires and the funding will be automatically released after the proposal is successfully and completely executed.

![图片](https://uploader.shimo.im/f/uMwT3hhuzXbVlMay.png!thumbnail)

Figure 5.1 - Voting on proposals

5.2 Off-chain Review - Merge Pr (pull request) on GitHub:

Following the successful implementation of the proposal, the Committee will merge pr (pull request).

![图片](https://uploader.shimo.im/f/CSWpV66DCfgiQmhL.png!thumbnail)

Figure 5.2 - Merge pr

 
---


# aelf DAO Project Pre-audit
In a Grant or Bounty Project, after the Pr (pull request) of the project application is submitted by a Committee member in GitHub. It can be pre-audited before the formal application proposal to launch a referendum model proposal. In this way, the Committee can be allowed to pre-audit the project content to evaluate the value of the project and to attract the attention of the Committee Members and Production nodes to the formal proposal.

The referendum is not part of the aelf DAO ecosystem, it is a non-essential step.

The steps are as follows:

1. After the developer submits the Pr on Github, visit the [proposal page](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply) to apply for referendum proposal in aelf Explorer and fill in the following:

![图片](https://uploader.shimo.im/f/MWjrPYZrmfYn5lOb.png!thumbnail)

Figure 1-aelf DAO Management Committee apply for proposal

* Proposal Mode: Referendum
* Organization: VOTE Token Referendum Organization
* Contract Address: aelf DAO Contract
* Method Name: ProjectPreAudit
* Method Params: GitHub pr links, Git commit ID
* URL: Provide a link to describe the proposal, which can be GitHub Pr link (optional)
* Expiration Time: You need to choose the right time period, to ensure that it does not affect project development and that organization’s members have enough time to vote. (Suggestions: No more than 7 days) 
1. Successful applications for the referendum proposal will be displayed on the proposal page. The VOTE Token holders will VOTE for the proposal. After you apply for a proposal, you can synchronize the proposal link with the Pr (pull request) conversation to ensure that the information on Github corresponds to the information on the chain.
2. After the proposal is accepted, the applicant executes the proposal and decides whether to hold a formal vote or not.


---


# aelf DAO proposal creation and modification
1. aelf DAO process-related organizations
* aelf DAO Management Committee (Created by the aelf DAO Contract)
* Production Nodes Organization
* Referendum Organization (Use Vote Token for Referendum)


## aelf DAO Create Organization steps
### 1. Production Nodes Organization
* **Role: Review the Round 2 voting for a DAO Grant or Bounty project proposal, vote for the proposal, and ‘join or leave the aelf DAO Management Committee Members’.**
* **Creator: Production Nodes**
* **Organization Actual Threshold Modification Authority: Whitelist Users**
* **Organization:**
| Model   | Parliament Contract Model   | 
|:----|:----|
| Organization Members   | Production Nodes   | 
| Proposal Whitelist   | All users   | 
| Threshold for the proposal adoption    | Agree ≥ 50%, Disagree ≤ 50%, Abstain ≤ 50%，Total votes ≥ 50%   | 




**Create Organization**

![图片](https://uploader.shimo.im/f/3lhLShN1fgIpromJ.png!thumbnail)

Figure: Create Organization

### 2. Referendum Organization
* **Role: Pre-audit the project by referendum outside the aelf DAO ecosystem.**
* **Creator: Community Users**
* **Organization Actual Threshold Modification Authority: Whitelist Users**
* **Organization:**
| Model   | Referendum Contract Model   | 
|:----|:----|
| VOTE Token Type   | VOTE Token (After voting, these tokens will be locked and can not be redeemed until the proposal expires or is released)   | 
| Organization Members   | All users who have VOTE Tokens   | 
| Proposal Whitelist   | The users’ address that you entered when you created the organization. If the applicant is not in the whitelist, you need to re-create an organization, or contact users in the white list to modify the organization whitelist and threshold.   | 
| Threshold for the proposal adoption   | Agree ≥ 0.5%, Disagree ≤ 0.5%, Abstain ≤ 0.5%, Total Votes ≥ 1%  (Object: Total number of VOTE Token)  (When changing the threshold value, you need to enter a value to convert the corresponding value in proportion)   | 



**Create Organization**

![图片](https://uploader.shimo.im/f/LBLncfQP2VJdSpOT.png!thumbnail)

Figure: Create Organization

## (3) Change Organization Steps
1. **Apply for a ‘Change Organization’ proposal**

If you need to change the organization (change the membership of the organization, the whitelist of proposals, or the threshold) , click the ‘change icon’, and the webpage will jump to the proposal application page. 

![图片](https://uploader.shimo.im/f/o6v6gRx0aFEQx7zx.png!thumbnail)

Step 1 - Change Organization

![图片](https://uploader.shimo.im/f/eQSN3VqG0uQMCRMJ.png!thumbnail)

Step 2 - Apply for ‘change organization proposal’ proposal

Enter the following as required in this step:

* Step 1 - Select the Method Name from the following names: (Only one parameter can be amended at a time)
  * ChangeOrganizationMember
  * ChangeOrganizationproposerWhiteList
  * ChangeOrganizationThreshold
* **Step 2 **- Enter the method name parameter: You need to enter the parameter corresponding to the method name in the following format.

①Example of changing organization member: (method name: ChangeOrganizationMember)

```
{
    "organizationMembers": [
        "2hxkDg6Pd2d4yU1A16PTZVMMrEDYEpr8oQojMDwWdax5LsBaxX",
        "2W8f3QhQxjAy9KK3obokfDpKZMfR2hp2Wn5HFr1JgxVNiPTdWY"
    ]
}
```
②Example of changing whitelist: (method name:ChangeOrganizationproposerWhiteList)

```
{
    "proposers": [
        "HqDfy3pXV6g9aKhXNqQMVHXxLQRU611XaWgXD48ieNcoPnyyv",
        "2h2SFeyLUJ3nPLpiG3BbqNUcjAQX5BUi3gRG9KWDpfHh7Jo5cp"
    ]
}
```
③Example of changing threshold: (method name:ChangeOrganizationThreshold)

```
{
    "minimalApprovalThreshold": "2",
    "maximalRejectionThreshold": "2",
    "maximalAbstentionThreshold": "2",
    "minimalVoteThreshold": "2"
}
```
* **Step 3 **- URL: Enter the URL related with the organization’s change (optional).
* **Step 4 **- Expiration time: Set the appropriate time, as appropriate, to ensure that all of the organization members have enough time to vote before the expiration date.
1. **Voting and Execution**

After you apply for a proposal, you can view the proposal information on the proposal  page. The amended organizational data shall not take effect until the original organizational members have voted for it and the applicant has executed the proposal.



---
 

# Our Community
### GitHub Organization
The GitHub Organization is used for funding project applications, Bounty projects release, project progress tracking, and development results submission. At the GitHub Organization, you can see all the development status of DAO community projects. Community users can access the DAO GitHub Organization through the following link:

aelf DAO Testnet:[ https://github.com/DAO-Testnet](https://github.com/DAO-Testnet)

1. GitHub ‘Grant Project’ repository：[https://github.com/DAO-Testnet/Grants](https://github.com/DAO-Testnet/Grants)
2. GitHub ‘Bounty Project’ repository：[https://github.com/DAO-Testnet/Bounties](https://github.com/DAO-Testnet/Bounties)
3. GitHub ‘DAO Documents’ repository：[https://github.com/DAO-Testnet/Docs](https://github.com/DAO-Testnet/Docs)
### Telegram Community
A new decentralized autonomous community of aelf: **saelf governed community** 

Through the ‘**saelf governed community’**, users can participate with ease in the aelf DAO development. Simultaneous to this, according to the degree of users' participation and contribution, users can get corresponding rights and share in aelf’s development achievements. Members of the community can participate in discussions and decision-making of the aelf DAO management system draft within the group and are eligible to apply to join the aelf DAO management committee. In order to ensure the community’s quality and protect the rights of every member participating in the aelf ecosystem governance, there will be an official invitation to join the saelf-governed community. Join the ‘**saelf governed community’** to view the full **aelf DAO Management System Draft**. For more details on how to join the group: [aelf Saelf-Governed Community](https://medium.com/aelfblockchain/join-the-aelf-saelf-governed-community-911338fd1a08)

