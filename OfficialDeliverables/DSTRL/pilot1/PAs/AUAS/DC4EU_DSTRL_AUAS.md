# DC4EU Deployment and Testing Scenarios Results Library (DTSRL) – Scenario: Amsterdam University of Applied Sciences (AUAS)

## 1. Scenario identification
- **Piloting agent name**: Amsterdam University of Applied Sciences (AUAS)  
- **Scenario title**: Activating wallet, PID and credential issuance with QR-based verification and deleting wallet  
- 4 juli 2025  
- **Point of contact (SPOC)**: SURF  

## 2. Scenario characterisation
- User journeys to be implemented: onboarding, PID retrieval, diploma/microcredential/EHIC issuance, QR-based verification of PID/diploma/microcredential/EHIC  
- Target groups and end-user roles: Students and/or employees (target: 25) Results: 53 users, with 43 filled in surveys  
- Electronic Attestations of Attributes (EAAs) involved (to be issued or verified)  : PID/diploma/microcredential/EHIC
- Institutional systems/databases connected to the credential workflows  : Not applicable (SaaS solution)
- Technical components used (e.g. PID service, Issuer/Verifier platforms, EUDIW wallet)  : Technical components of the WP7 interoperability lab
- Governance configuration (DIDs, authorisation templates, trust model references)  : WP7 SaaS
- Monitoring and feedback mechanisms (tools, frequency, KPIs)  : task 3.6 survey end-users, weekly report, readyness tracker, filled in KPI results

## 3. Legal, organisational and operational details
- Regulatory context (GDPR, national rules, education-specific laws)  : synthetic data interop lab, Governance analysis Dutch education in PPT dec 2024
- Risk management (identified risks and mitigations)  : availability/performance SaaS solution and effect on perceived reliability of wallet, feasability end-users for testsessions.
- Credential lifecycle management (revocation, updates, suspension) :revocation and suspension were not yet available in the interoperability lab. Updates received on credentials and other testmaterials on a regular basis. 
- Infrastructure readiness (hardware, software, endpoints, availability) : rather late readiness, bumpy road in the beginning of testsessions. Great improvement of performance during the following weeks 
- Training and onboarding plans for end-users and administrators: received on time  
- Issue escalation procedures (with SPOC contacts)  : available/excellent (short response times). 
- Success indicators and KPIs  : see output surveys + summary in weekly report: # end-users 53, # Total transactions users including activated/deleted wallets: 389

## 4. Trust model onboarding evidences
- Issuer X.509v3 certificate issued by the trust anchor (include PEM or screenshot link as provided by WP7) : provides by WP7 to wp5-leader. PEM:
  **Piloting issuer 1**
-----BEGIN PUBLIC KEY-----
MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEi3v64MrIKoS9Aofws9Dg3Vd7Ej9Z
MBUYJ8DuHxb2mNDiRbrmJ6KqdIsrXWRfzguJUceYWZuo8Fx6RVP+E7Muvg==
-----END PUBLIC KEY-----
 
**Piloting issuer 2**
-----BEGIN PUBLIC KEY-----
MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEZd+VkUmChe4KausswJ87UtAggrtd
BAg+K/5U+fBmZP3JR3dly/Ir0fMLoA0+xPA+nP3pp7JrjgPSktHXAZPt0Q==
-----END PUBLIC KEY-----

 
- Relying party X.509v3 certificate (access cert) and scope of authorised EAAs (not available, as it was expected to be provided by WP7. Due to time constraints it has not been provided)  
- PID access credentials and service metadata:  Credential issuer: http://vc-interop-1.sunet.se:8080/
- For dPKI-based actors: Decentralised Identifiers (DIDs) with metadata and authorisation status: not applicable for Classical PKI
- Reference to the authoritative registry where these credentials are validated (e.g. EAA catalogue, trust list): WP7 Interoperability lab  

## 5. Implementation and testing progress
- **Status**: Scenario available during testphase, except for EducationalID and credential revocation. Testmaterial and test-environment ready from May 28th.  
- **Wallets activated**: **53** 
- **Credentials issued**: **224**
- **Credentials verified**: **100**
- **deleted wallets**: **12**
- Current scenario status: **Completed**  
- Number of users onboarded: **53 in total, of which 13 students**    
- Summary of operations executed successfully:**Total transactions users including activated/deleted wallets: 389**   
- Issues encountered (brief description): **see remarks weekly reports**  
- Deviation from plan (if any) : **delay in piloting with the result of cancelling 6 testsessions; adding EHIC, skipping EducationalID and revoking credentials**

## 6. Testing results and observations
- What worked as expected: after initial hickups: most features worked as planned**   
- What did not work and why: revocation did not work as it was not available in the interop lab, the same goes for EducationalID
- Feedback from users (students, staff, relying parties): see end-user surveys. most important: 1)technical and user experience challenges. The most prominent technical issues involve slow performance and unreliable credential loading, with users frequently reporting long wait times, timeouts, and the need to repeat actions multiple times to achieve successful results. 2)Users report confusion regarding the process flow, unclear instructions, and a lack of visual guidance, which complicates onboarding and credential management.3)only manageable for those with strong digital literacy, potentially excluding less tech-savvy individuals. 
- Impact on user experience, technical feasibility or legal compliance. **Result: users recommending improvements in performance, clarity, and accessibility.**

## 7. Evidence archive and references
- Screenshots or logs of key stages (onboarding, issuance, verification): **see comments on issues in weekly report**
- Links to shared environment/demo (if applicable): **Credential issuer: http://vc-interop-1.sunet.se:8080/. Credential verifier: https://dc4eu-verifier.wwwallet.org/**
- Reference to shared documentation, Git repos, dashboard entries etc.: **https://sites.ey.com/:x:/r/sites/DC4EU-EBSINE/_layouts/15/Doc.aspx?sourcedoc=%7B603E5860-E8C1-4D1E-B33D-31E33147739F%7D&file=AUAS%20Readyness%20and%20weekly%20report_DC4EU.xlsx&action=default&mobileredirect=true; https://sites.ey.com/sites/DC4EU-EBSINE/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FDC4EU%2DEBSINE%2FShared%20Documents%2FGeneral%2FDC4EU%2FWP5%2F40%20Technical%20tracks%2FClassical%20PKI%20Trusted%20Lists%2FDocuments&viewid=1d5f5777%2D8eec%2D44ab%2Da8a2%2D488cd0136ef2; https://sites.ey.com/:p:/r/sites/DC4EU-EBSINE/_layouts/15/Doc.aspx?sourcedoc=%7BF96E3971-C8ED-4695-BD00-489ACE5A65BE%7D&file=AUAS%20-%20PPT%20Scenarios%20description.pptx&action=edit&mobileredirect=true**
- KPI data submission (format, frequency, where sent) : **T3.6 end-user surveys; piloting agent survey; weekly report, see link above;final results in mail to wp5 leader c.s. on June 24th and this document on Github**

## 8. Next steps and recommendations
- Actions pending or in progress: internal evaluation document, internal reporting on project; financial reporting withing DC4EU.  
- Recommendations for future pilots or replication: **performance and UX-levels before starting testphase should be much higher; planning testmaterials more timely; workshops more interactive**  
- Changes proposed to methodology or components: **improved survey end-users, based on industry standard questionnaires concerning UX**    


## 9. Summary of end-user feedback (students, staff, verifiers)
- General impressions about the onboarding, issuance and use of digital credentials: **Overall, the feedback emphasized the importance of simplicity, clarity, and inclusivity in the design and operation of electronic identity wallets, with a strong focus on meeting the needs of non-technical users and ensuring robust security and privacy protections.**  
- Perceived ease of use of the EUDIW wallet: **depending on digital savvyness, performance (later testsessions had much better performance) and target group: students were much more positive than staff.**   
- Specific challenges or confusions encountered: **see LLM summary of surveys (Tamas Miseta)** 
- Suggestions for improvement: **tool-tips, performance, usability, explaining the walet and the ecosystem behind (what happens with my data, where am i in the process).**   
- Overall acceptance and readiness to use these services in real life: **6,4 on a scale of 1-10 in answer to question would you recommend this service to frneds/family**

## 10. Summary of piloting agent insights
- Feedback on the support received from WP5 / SPOC: **to satisfaction**  
- Barriers faced during implementation (technical, legal, procedural) : **planning!!** 
- Lessons learned that could inform future scenarios: **planning!!**  
- Perceived benefits and areas of impact: **knowledge on working with wallets and verifiable credentials, the fact that staff could try out the functions of wallets and the issuance and verification of credentials**
- Recommendations for scaling up or replicating the scenario: **improved performance, usability and planning**  
