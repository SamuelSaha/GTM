# Automate Your Way to Success with Marketing Automation

**Author:** Unknown  
**Format:** PDF  
**Category:** demand-gen

---

## Page 3

SalesforceAutomation withSalesforce Flow andApex
Automate your way to success withSalesforce automation tools
Om Prakash
www.bpbonline.com

---

## Page 4

First Edition 2025
Copyright © BPB Publications, India
ISBN: 978-93-65899-122
All Rights Reserved. No part of this publication may be reproduced, distributed or transmitted in any form or by any means or stored in a
database or retrieval system, without the prior written permission of the publisher with the exception to the program listings which may be
entered, stored and executed in a computer system, but they can not be reproduced by the means of publication, photocopy, recording, or
by any electronic and mechanical means.
LIMITS OF LIABILITY AND DISCLAIMER OF WARRANTY
The information contained in this book is true to correct and the best of author’s and publisher’s knowledge. The author has made every
effort to ensure the accuracy of these publications, but publisher cannot be held responsible for any loss or damage arising from any
information in this book.
All trademarks referred to in the book are acknowledged as properties of their respective owners but BPB Publications cannot guarantee
the accuracy of this information.
www.bpbonline.com

---

## Page 5

Dedicated to
My familyFor their constant love, support, and faith in every step of my journey
AppyCrown Private LimitedMy company, which fuels my passion and purpose
Salesforce Trailblazer CommunityFor inspiring and empowering me to reach new heights

---

## Page 6

About the Author
Om Prakash is a respected Salesforce MVP, recognized since 2020 for his outstanding contributions tothe Salesforce ecosystem, marking his fifth consecutive year with this esteemed recognition. As theFounder and CEO of AppyCrown Private Limited—a Salesforce Consulting and AppExchange AppDevelopment company—he brings over 13 years of experience in the IT industry, including more than10 years focused on the Salesforce platform since 2014.
Driven by the belief that "Let's be a savior instead of superior," Om is dedicated to empoweringbusinesses by delivering exceptional solutions on the Salesforce Platform. He is a Salesforce CertifiedProfessional, holding prestigious certifications such as Salesforce Certified Application Architect,Developer, and Advanced Admin. His expertise in the Salesforce.com developer toolkit allows him toleverage no-code, low-code, and pro-code solutions, enabling organizations to craft robust, tailoredsolutions.
Throughout his career, Om has successfully developed multiple Salesforce Apps for various businessesand ISV partners, expertly overseeing the entire application lifecycle. He has helped many organizationsacross different industries with consulting and technical architecture, crafting effective solutions tailoredto their unique needs.
Additionally, he is a skilled technical trainer and public speaker, sharing his insights at various Salesforceonferences and events, and he leads by example within the Salesforce Trailblazer Community.
At AppyCrown, he and his team provide trusted Salesforce consulting services and AppExchange appdevelopment. His extensive experience includes leading the development and configuration of newfunctionalities for client Salesforce Orgs, optimizing legacy configurations for better performance, andsuccessfully executing various integrations using different methods.
As a trusted advisor in the Salesforce ecosystem, Om Prakash exemplifies expertise, leadership, andgenerosity. He makes a significant impact through mentorship, knowledge sharing, and collaboration.He invites readers to connect with him to leverage skills and expertise for their business success withSalesforce flow.
Om is passionate about sharing his knowledge and experiences, inspiring fellow learners in thecommunity. He regularly posts technical content and motivational messages on his YouTube channel,Inspiring Ohana, and he actively participates as a guest speaker on other community channels.
As the Community Group Leader for the Salesforce Developer Group, Motihari, Bihar—the first andoldest active Salesforce community group in the Indian state of Bihar—Om organizes community eventsthat foster knowledge sharing and collaboration among developers. He was co-founder and organizer ofBharat Dreamin’ 2024, a Salesforce Community conference.

---

## Page 7

About the Reviewer
Nipunu Wijesingha is an accomplished Salesforce professional with over 12 years in the IT industry,including 8 years specializing in Salesforce solutions. He holds multiple certifications, includingSalesforce Platform Developer and Administrator, as well as AWS Cloud Practitioner. As a 2x TrailheadRanger, Nipunu is committed to continuous learning and staying at the forefront of Salesforcetechnologies. His expertise spans Sales, Service, and Experience/Community Cloud, as well as FieldService Lightning (FSL) and Salesforce integration, making him a versatile asset to complex, large-scaleprojects.
Nipunu is passionate about driving business transformation through innovative Salesforce solutions.With extensive experience in Apex programming, Lightning Web Components (LWC), and integrationtools, he combines technical skill with best practices and a collaborative approach to problem-solving.He is also highly skilled in implementing Salesforce DevOps solutions, creating streamlined deploymentframeworks and automation strategies with tools like Gearset, Copado, Git, and Salesforce DX.
Currently a Salesforce Technical Lead at iTelaSoft Australia, Nipunu has previously worked with Micadoin New Zealand, where he focused on developing scalable, robust applications and integratingSalesforce with other enterprise systems. His career also includes lecturing roles, where he introducedSalesforce training to university curricula, sharing his passion for the platform with both students andindustry professionals. Nipunu’s background as a technical lead and mentor brings valuable insight toeach project, ensuring that teams are well-supported in delivering high-impact Salesforce solutions.

---

## Page 8

Acknowledgement
I want to say a big thank you to everyone who helped us finish this book. First, I am especially gratefulto my family and friends for their constant support and encouragement. Their love has been a truesource of motivation for us throughout this journey.
Thank you to Salesforce for its continuous innovation in flow development, which has greatly inspiredand enhanced the quality of this book. A heartfelt thank you to the Salesforce Trailblazer Community fortheir continuous inspiration and support, empowering us to bring this project to life.
I would like to extend my heartfelt thanks to the team at AppyCrown for their time to time support anddedication throughout this project. Your collective insights, feedback, and contributions have beeninstrumental in shaping the content and enhancing the quality of this book.
I am immensely grateful to BPB Publications for their guidance and expertise in bringing this book tolife. Their support and assistance were invaluable in navigating the complexities of the publishingprocess. I would also like to acknowledge the reviewers, technical experts, and editors who providedvaluable feedback and contributed to the refinement of this manuscript. Their insights and suggestionshave significantly enhanced the quality of the book.
Last but not least, I want to express our gratitude to the readers who have shown interest in our book.Your support and encouragement have been deeply appreciated.
Thank you to everyone who has played a part in making this book a reality.

---

## Page 9

Preface
In today's fast-paced business environment, the ability to adapt and innovate is paramount.Organizations are constantly seeking ways to optimize their operations, enhance customer experiences,and leverage technology to drive growth. In my career as a Salesforce professional, I have witnessedfirsthand the transformative power of automation within the Salesforce platform. This book is born outof a passion for sharing that knowledge with others who wish to harness the full potential of Salesforceautomation.
This journey begins with a foundational understanding of Salesforce and its automation capabilities,leading readers through the intricacies of Salesforce flow. Each chapter is carefully crafted to guide youfrom the basics to advanced concepts, offering practical insights, hands-on examples, and real-worldapplications. Whether you're a seasoned administrator, Developer or just starting your Salesforcejourney, you will find valuable information tailored to your level of expertise.
The chapters delve into the various facets of Salesforce automation, exploring topics such as screenflows, record-triggered flows, and the integration of Apex actions. Each section is designed to buildupon the previous one, creating a comprehensive roadmap to mastering automation in Salesforce. Wewill also address common challenges and best practices to ensure you not only understand how toimplement automation but also how to troubleshoot and optimize your flows for peak performance.
As you navigate through this book, I encourage you to engage with the material actively. Experimentwith the examples provided, and apply the concepts to your unique business scenarios. The world ofSalesforce automation is rich with opportunities, and I hope this book serves as a valuable resource onyour path to becoming a proficient Salesforce automation expert.
This book is designed for anyone interested in mastering Salesforce flow, whether you're a seasonedprofessional looking to enhance your skills or a beginner eager to learn the fundamentals. It serves asan essential resource for individuals aiming to understand the capabilities and applications of Salesforceflow in automating business processes.
Through practical examples, comprehensive explanations, and a structured approach, this book aims toequip readers with a solid understanding of Salesforce flow. Whether you are a novice or anexperienced learner, I hope this book will serve as a valuable resource in your journey of exploring theSalesforce flow.
Chapter 1: Necessity of Salesforce Automation– In this first chapter, you will learn a quick intro toSalesforce and Salesforce automation, available automation tools. Why automation is needed and startwith a common process automation scenario and use cases.
Chapter 2: Introducing Salesforce flow’s Features and Capabilities– Features and Capabilities:You will learn flow concepts and deep dive to learn about what flow is, and what can be achieved byflow . We dive into the world of workflow, Process Builder, and Salesforce flow within the Salesforceecosystem. In today's dynamic business environment, streamlining processes and automating repetitivetasks are paramount for organizations to stay competitive. This chapter aims to provide acomprehensive introduction to these tools, enabling readers to harness their power and drive efficientbusiness operations.
Chapter 3: Up and Running with Salesforce flow– Salesforce flow is a powerful automation toolthat enables users to automate complex business processes, integrate with other systems, andstreamline their operations. There are several types of flows available, including screen, autolaunched,and scheduled flows. Each type of flow has its own set of features and capabilities, making it easier forusers to create custom workflows that meet their specific needs.

---

## Page 10

Data manipulation and management are vital aspects of any automation solution, and Salesforce flowprovides robust capabilities in this regard. This chapter will help you to explore flows data elements,which empower you to access, manipulate, and store data within your flow.
Chapter 4: Salesforce flow Implementation and Debugging– In this chapter you will learn howto implement and debug the flowsflows effectively. You will explore the flow Builder, you will understandhow to create and configure flows, run them, and troubleshoot any issues that may arise. Additionally,you will learn to examine paused and failed flow interviews and learn how to resolve them.
Chapter 5: Creating Screen flows– With this chapter you will explore the concept of subflows andadopt a modular approach in screen flow design, and reflect on the key learnings and best practices forcreating effective screen flows.
Chapter 6: Implementing Screen flows– This chapter will guide users through department and roleselection using screen choice components, help to create consistent and efficient onboardingexperiences for new employees, and demonstrate how to distribute employee onboarding screen flowseffectively to users.
Chapter 7: Implementing Record-triggered flows– In this chapter, you will learn to extend thecapabilities of record-triggered flows using actions and related records. With an easy example, we willexplain how to automate the process when a record is deleted from Salesforce Org . The goal of thischapter is to make you familiar with flow Trigger Explorer and its usage for analyzing andtroubleshooting flows. You will have valuable insights and key learnings for successfully implementingrecord-triggered flows in your organization.
Chapter 8: Scheduling Triggered flows– This chapter is designed to leave you well-prepared toharness the power of schedule-triggered flows. Whether you are looking to streamline your operations,optimize your workflow, or implement industry specific use cases, the insights and knowledge gainedfrom this chapter will be invaluable in achieving your automation goals.
Chapter 9: Platform event-triggered flow– By the chapter's end, you will have a firm grasp onleveraging the platform event’s publish-subscribe model and flows' intuitive design interface to craftresponsive applications tailored to your business needs. Through structured exploration, we will uncoverthe symbiotic relationship between platform events and flows, spotlighting their role in ensuring theagility and responsiveness of your Salesforce environment. Get ready to embark on a journey into therealm of real-time event-driven automation, where the fusion of platform events and flows propels yourorganization towards heightened productivity and innovation.
Chapter 10: Autolaunched flows– This chapter will explain why autolaunched flows are so crucial ineveryday business situations. By looking at common challenges, we will show you why autolaunchedflows are the go-to solution. Then, we will get our hands dirty and guide you step-by-step in creatingthese flows. We will also share the best ways to design autolaunched flows that work well and growwith your business.
Chapter 11: Record-triggered Orchestration– This chapter is designed for Salesforceadministrators, developers, and users to gain a solid understanding of record-triggered orchestration. Bythe end, you will know how orchestration can improve workflows and automate key processes inSalesforce.
Chapter 12: Apex Actions and Lightning Web Components – In this chapter, we will explore howto create and use custom Apex actions. We will guide you through the basics of Apex programming,making it easy to understand even if you are new to coding.
Chapter 13: Best Practices and Troubleshooting Measures– In this chapter, our primary goal isto provide a comprehensive understanding of Salesforce flow, catering to both beginners and advancedusers. We aim to explore industry standard best practices and troubleshooting measures to optimize thedesign and execution of flows. Throughout this chapter, we will look at the flow limits, emphasizing ontopics essential for working within Salesforce multitenant environment.
Chapter 14: Distributing and Sharing flows– The chapter aims at providing you with theknowledge and skills needed to effectively distribute and share flows. We aim to provide a deep

---

## Page 11

understanding of the intricacies involved in granting user access, exploring packaging considerations,and leveraging different distribution methods.
Chapter 15: Integrating flow Outside Salesforce– In this chapter, our aim is to equip you with theknowledge and skills necessary to seamlessly integrate Salesforce flow processes with external datasources, services, and APIs. We will delve into various integration techniques, including accessing datafrom external databases, triggering actions in third-party systems, and interacting with external servicesvia HTTP requests.
Chapter 16: Migrating to flow from Workflow and Process Builder– The objective of thischapter is to equip readers with the knowledge and tools necessary to effectively test Salesforce flowsafter migrating from workflow rules and Process Builder. By emphasizing the importance of testing inthe migration process, this chapter aims to provide a comprehensive understanding of the testingconsiderations and strategies required to ensure the functionality, reliability, and performance of flows.Through practical insights and best practices, readers will learn how to conduct thorough unit testing,integration testing, user acceptance testing, and performance testing to identify and address any issuesearly in the migration process. Ultimately, the goal is to facilitate a seamless transition to Salesforceflow, empowering organizations to leverage their advanced automation capabilities with confidence andefficiency.
Chapter 17: Hands-on Apex Triggers for Automation– In this concluding chapter, our objective isto provide you with a holistic understanding of Apex triggers and their indispensable role in Salesforceautomation. We aspire to guide you through the foundational principles of Apex triggers, elucidatingtheir usage, nuances, and best practices. Moreover, we endeavour to demonstrate how Apex triggerscan seamlessly integrate with Salesforce flow, facilitating the creation of robust and comprehensiveautomation solutions.

---

## Page 12

Code Bundle and Coloured Images
Please follow the link to download theCode Bundle and the Coloured Images of the book:
https://rebrand.ly/4ff8cf
The code bundle for the book is also hosted on GitHub athttps://github.com/bpbpublications/Salesforce-Automation-with-Salesforce-Flow-and-Apex. In case there’s an update to the code, it will be updated on the existing GitHub repository.
We have code bundles from our rich catalogue of books and videos available athttps://github.com/bpbpublications. Check them out!
ErrataWe take immense pride in our work at BPB Publications and follow best practices to ensure the accuracyof our content to provide with an indulging reading experience to our subscribers. Our readers are ourmirrors, and we use their inputs to reflect and improve upon human errors, if any, that may haveoccurred during the publishing processes involved. To let us maintain the quality and help us reach outto any readers who might be having difficulties due to any unforeseen errors, please write to us at :
errata@bpbonline.com
Your support, suggestions and feedbacks are highly appreciated by the BPB Publications’ Family.
  
Did you know that BPB offers eBook versions of every book published, with PDF and ePub files available? You can upgrade to the eBook
version at www.bpbonline.com and as a print book customer, you are entitled to a discount on the eBook copy. Get in touch with us at :
business@bpbonline.com for more details.
At   www.bpbonline.com, you can also read a collection of free technical articles, sign up for a range of free newsletters, and receive
exclusive discounts and offers on BPB books and eBooks.
  
 Piracy 
If you come across any illegal copies of our works in any form on the internet, we would be grateful if you would provide us with the
location address or website name. Please contact us at business@bpbonline.com with a link to the material.
 If you are interested in becoming an author 
If there is a topic that you have expertise in, and you are interested in either writing or contributing to a book, please visit
www.bpbonline.com. We have worked with thousands of developers and tech professionals, just like you, to help them share their
insights with the global tech community. You can make a general application, apply for a specific hot topic that we are recruiting an author
for, or submit your own idea.
 Reviews 
Please leave a review. Once you have read and used this book, why not leave a review on the site that you purchased it from? Potential
readers can then see and use your unbiased opinion to make purchase decisions. We at BPB can understand what you think about our
products, and our authors can see your feedback on their book. Thank you!
For more information about BPB, please visit   www.bpbonline.com.
Join our book’s Discord space

---

## Page 13

Join the book’s Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 14

Table of Contents 
1. 1. Necessity of Salesforce Automation 1. Introduction2. Structure3. Objectives4. Quick introduction to the Salesforce platform5. Need for automation6. Salesforce automation overview7. Automation scenario and use cases8. Customer expectations and business processes 1. Customer expectations and business processes for automation9. Challenges with other automation tools10. Expectations and reality with business logic11. Mindset and mapping for automation12. Conclusion
2. 2. Introducing Salesforce flow’s Features and Capabilities 1. Introduction2. Structure3. Objectives4. Workflow and Process Builder 1. Workflow in Salesforce2. Process Builder in Salesforce3. Key differences between workflow and Process Builder5. Salesforce flow 1. Why use Salesforce flow 1. Functions with Salesforce flow2. Using Salesforce flow6. Salesforce flow capabilities7. Essential features and potential functions 1. Essential features2. Potential functions8. Think like a pro for Salesforce flow9. Introduction and start with pre-built automation10. Conclusion
3. 3. Up and Running with Salesforce flow 1. Introduction

---

## Page 15

2. Structure3. Objectives4. Types of Salesforce flow 1. Subflow5. Flows elements, connectors, and resources6. Flows data elements7. Assignment and Loop Elements8. Creating a formula in flow9. Decision in flow10. Conclusion
4. 4. Salesforce flow Implementation and Debugging 1. Introduction2. Structure3. Objectives4. Exploring the flow Builder 1. Elements2. Resources3. Screens4. Flow logic5. Testing and previewing5. Creating your flow 1. Accessing the flow Builder2. Creating a new flow3. Adding elements4. Configuring screen components6. Run your flow and flow versions 1. Running a flow2. Flow versions7. Debugging the flow8. Troubleshooting flows9. Paused and failed flow interviews 1. Paused flow interviews2. Failed flow interviews10. Conclusion
5. 5. Creating Screen flows 1. Introduction2. Structure3. Objectives4. Identifying the need for screen flows5. Fundamentals of screen flow6. Collecting information with screen flows7. Implementing business logic in screen flows8. Displaying records in screen flows

---

## Page 16

9. Distribution of screen flows10. Error handling and fault path in screen flows11. Subflows and modular approach12. Key learnings13. Conclusion
6. 6. Implementing Screen flows 1. Introduction2. Structure3. Objectives4. Requirement discussion5. Creating the employee onboarding flow6. Creating subflow and using it7. Distributing the Screen flow8. Conclusion
7. 7. Implementing Record-triggered flows 1. Introduction2. Structure3. Objectives4. Fundamentals of record-triggered flows5. Identify the need for record-triggered flows 1. Scenario 1: Automated updates and notifications2. Scenario 2: Approval processes3. Scenario 3: Data integrity4. Scenario 4: Workflow automation6. Insert record-triggered flows7. Criteria for the record trigger8. Fast Field Updates9. Actions and related records10. Delete record-triggered flows11. Conclusion12. Key learnings
8. 8. Scheduling Triggered flows 1. Introduction2. Structure3. Objectives4. Business need for the schedule-triggered flows5. Problem statement 1. Role of schedule-triggered flows6. Configure schedule-triggered flow7. Behaviors of schedule-triggered flow8. Schedule-triggered flow for batches of records

---

## Page 17

1. Batch processing definition2. Use cases3. Configuration for batch processing4. Benefits of batch processing9. Monitor schedule-triggered flows 1. Monitoring tools in Salesforce2. Error handling and alerts3. Performance optimization4. Scaling and capacity planning5. Regular reviews and audits10. Conclusion
9. 9. Platform event-triggered flow 1. Introduction2. Structure3. Objectives4. Platform events overview 1. Use cases5. Platform event-triggered flow 1. Use cases6. Publish event messages with flows7. Subscribe to platform event messages with flows8. Business use cases for platform events and flows9. Conclusion
10. 10. Autolaunched flows 1. Introduction2. Structure3. Objectives4. Business requirements for autolaunched flow5. Creating autolaunched flow 1. Scenario overview6. Calling autolaunched flow from record-triggered flow7. Calling autolaunched flow from Apex 1. Invoking the autolaunched flow8. Verifying the updated phone on contact9. Calling autolaunched flow from the REST API10. Autolaunched flow vs record triggered flows 1. Autolaunched flows2. Record-triggered flows3. Integrating autolaunched flows with record-triggered flows11. Conclusion
11. 11. Record-triggered Orchestration 1. Introduction

---

## Page 18

2. Structure3. Objectives4. Orchestrations overview5. Types of flow Orchestration 1. Autolaunched orchestration2. record-triggered orchestration6. Orchestration anatomy7. Difference between flow Builder and flow Orchestration 1. Flow Builder2. Flow Orchestration8. Orchestration run 1. Running context of an orchestration9. Hands-on example with record-triggered orchestration 1. Use case 1. Create a screen flow2. Create an autolaunched flow3. Create a record-triggered orchestration4. Testing of the use case10. Conclusion
12. 12. Apex Actions and Lightning Web Components 1. Introduction2. Structure3. Objectives4. Create your custom action5. Basics of Apex 1. Variables2. Conditions: If-else3. Loops4. Lists, sets, and maps: Collections5. Apex classes and methods6. Invocable method annotation7. Execute Apex actions8. Using a custom Lightning Web Component 1. Configuration steps9. Embed a flow in the custom Lightning Web Component 1. Significance of embedding flow in LWC2. A quick guide to embed a flow3. Considerations for success10. Conclusion
13. 13. Best Practices and Troubleshooting Measures 1. Introduction2. Structure3. Objectives

---

## Page 19

4. Flow limits and considerations 1. Limits for Salesforce flows2. Data handling considerations5. Flow best practices6. Bulkify your flow 1. Understanding transactions and governor limits2. Bulkified flow elements3. Guidelines for achieving bulkification in a flow7. Mastering to fix common issues in flow 1. Proactive testing with debug2. Check for required fields3. Handling flow errors caused by inactive users4. User permissions matter5. Beware of null values6. Reviewing and debugging7. Documentation and collaboration8. Considerations for flow data9. Debug log for running flow 1. Checking failed or paused flow interviews2. Debugging flow during development10. Considerations for flow Lightning runtime 1. Flow interview2. Limitations of Lightning runtime for flows3. Flow runtime accessibility considerations11. Conclusion
14. 14. Distributing and Sharing flows 1. Introduction2. Structure3. Objectives4. User access for the flow 1. Navigating flow access control2. Customizing access for your flows5. Distribute flows to internal users 1. Create an object-specific quick action2. Add a flow to the Actions & Recommendations component3. Add a flow to a utility bar4. Sharing the flow URL5. Embed a flow in a custom Aura component6. Embed a flow in a Visualforce page7. Call flow in Lightning Web Components8. Prepare your org for paused flow interviews6. Packaging considerations for flows7. Distribute flows to external users8. Experience Cloud and flows 1. Leveraging Salesforce flows in Experience Cloud

---

## Page 20

2. Key use cases3. Adding a flow to Experience Cloud9. Conclusion
15. 15. Integrating flow Outside Salesforce 1. Introduction2. Structure3. Objectives4. External objects 1. Using external objects in flow2. Access external data in flow5. Outbound message actions 1. Using outbound message actions in flow 1. Creating outbound message2. Creating triggered flow6. External Services7. Using External Services in flow8. HTTP callout 1. Using HTTP callout in flow9. Conclusion
16. 16. Migrating to flow from Workflow and Process Builder 1. Introduction2. Structure3. Objectives4. Strategy and plan for automation tool migration 1. Migration decision logic2. Logic for migration decision5. Converting workflow rules to flows 1. Using the Migrate to flow tool 1. Example2. Comparison3. Benefits of migration6. Converting processes to flows 1. Understanding the migration process2. Migration strategy3. Benefits of migration7. Reviewing the considerations for migration8. Testing strategy for flow after migration9. Conclusion
17. 17. Hands-on Apex Triggers for Automation 1. Introduction2. Structure3. Objectives

---

## Page 21

4. Flow versus Apex trigger 1. Choosing between flows and Apex triggers5. Apex trigger basics 1. Types of Apex triggers2. Key considerations for Apex triggers6. Apex trigger context variables 1. Types of Apex trigger context variables7. Automate using Apex trigger 1. Choosing Apex triggers for automation8. Bulkify the Apex trigger 1. Understanding bulk data operations2. Strategies for bulkification9. Best practices for the Apex trigger10. Combine the power of flow and Apex trigger11. Conclusion
18. Index

---

## Page 22

CHAPTER 1Necessity of Salesforce Automation
Introduction
In this first chapter, you will get a quick introduction to Salesforce and Salesforce automation, as wellas available automation tools. The chapter will look into why automation is needed and start with acommon process automation scenario and use cases.
Structure
The chapter covers the following topics: Quick introduction to the Salesforce platform
Need for automation
Salesforce automation overview
Automation scenario and use cases
Customer expectations and business processes
Challenges with other automation tools
Expectations and reality with business logic
Mindset and mapping for automation
Objectives
By the end of this chapter, you will be able to understand how to map the customer's expectations withyour complex business logic for seamless experiences. There are many decisions and actions behindevery step of the process, and you will explore how to map every process to the capabilities ofSalesforce flow.
Quick introduction to the Salesforce platform
Salesforce is a cloud-based customer relationship management (CRM) platform that helpsbusinesses manage their sales, marketing, customer service, and analytics functions all in one place.The platform provides a suite of tools and services that enable organizations to streamline theirprocesses, automate workflows, and build custom applications to meet their unique business needs.
The Salesforce platform is built on a multi-tenant architecture, meaning that multiple customers sharethe same infrastructure, which results in lower costs and improved scalability. The platform also offers awide range of products and services that can be customized and integrated with other third-partysystems, allowing businesses to tailor their Salesforce experience to their specific needs.
Some of the key features of the Salesforce platform include sales automation, marketing automation,customer service, analytics, mobile app development, and collaboration tools. The platform also has a

---

## Page 23

robust ecosystem of partners and developers who create third-party applications and integrations thatextend the functionality of Salesforce.
Overall, the Salesforce platform is a powerful tool for businesses looking to improve their customerengagement and drive growth through streamlined processes and data-driven insights.
Need for automation
Automation refers to the use of technology and software to perform tasks or processes that wouldotherwise require human intervention. This can include anything from simple, repetitive tasks like dataentry to complex processes like manufacturing, customer service, and financial analysis.
Automation can take many forms, such as robotic process automation (RPA), artificialintelligence (AI), machine learning (ML), and software automation. These technologies can beused to automate tasks and processes across a wide range of industries and functions, frommanufacturing and logistics to healthcare and finance.
One of the key benefits of automation is that it can help organizations reduce costs, improve efficiency,and increase productivity by removing the need for manual work and reducing the risk of human error.
Automation can also enable organizations to scale their operations quickly and efficiently, allowing themto meet changing customer demands and respond to new opportunities.
Overall, automation is a powerful tool that can help organizations improve their operations, streamlinetheir processes, and drive growth.
Automation can bring numerous benefits to businesses, including: Increased efficiency: Automation reduces the need for manual tasks, which can lead to fasterand more efficient processes. By automating repetitive tasks, employees can focus on morevaluable tasks that require their expertise and attention.
Improved accuracy: Automated processes can reduce human errors and ensure that tasks arecompleted consistently and accurately. This can result in higher quality work and fewer errors,which can improve customer satisfaction and reduce costs associated with rework or corrections.
Cost savings: Automation can help reduce costs associated with manual work, such as salaries,benefits, and training. In addition, automated processes can help reduce the risk of errors, whichcan save costs associated with rework, recalls, and other quality issues.
Scalability: Automated processes can be scaled quickly and easily to accommodate changingbusiness needs. This can help businesses adapt to changing market conditions and growthopportunities without the need for significant investments in infrastructure or staffing.
Competitive advantage: By automating processes, businesses can gain a competitive advantageby offering faster, more efficient, and more reliable services to their customers.
Overall, automation can help businesses save time, reduce costs, improve accuracy, and gain acompetitive edge, making it an important tool for organizations looking to streamline their operationsand drive growth.
Salesforce automation overview
Salesforce automation refers to the use of technology and software to automate sales, marketing,customer service, and other business processes on the Salesforce platform. This can include automatingrepetitive tasks like lead capture, data entry, and report generation, as well as more complex processeslike lead nurturing, sales forecasting, and customer support.
Salesforce automation is made possible through a range of tools and services offered on the Salesforceplatform, including:

---

## Page 24

Salesforce workflow: A visual process automation tool that allows users to automate repetitivetasks and processes, such as sending email notifications, updating records, and creating tasks.
Process Builder: A more advanced process automation tool that allows users to build complex,multi-step processes using a visual interface.
Sales cloud: A set of tools and services designed to help sales teams manage their salesprocesses more effectively, including lead and opportunity management, forecasting, andperformance metrics.
Marketing cloud: A suite of marketing automation tools that allow organizations to create andexecute targeted marketing campaigns across multiple channels, including email, social media, andmobile.
Service cloud: A set of tools and services designed to help customer service teams manage theirinteractions with customers more effectively, including case management, knowledge management,and customer self-service.
Salesforce automation offers various tools and services to automate business processes and streamlineworkflows on the Salesforce platform. Let us take a look at some of the key automation tools availableon Salesforce: Workflow: Salesforce workflow is a visual process automation tool that allows users to automaterepetitive tasks and processes. With workflow, users can create rules that automatically triggeractions such as sending email notifications, updating records, and creating tasks.
Process Builder: Process Builder is a powerful process automation tool that allows users to buildcomplex, multi-step processes using a visual interface. With Process Builder, users can automate awide range of business processes, including creating and updating records, sending emails, andcalling Apex methods.
Approval processes: Approval processes allow organizations to automate their approvalprocesses by setting up rules that automatically route records for approval to the appropriate usersor groups. With approval processes, organizations can ensure that their business processes areefficient and compliant while also ensuring that the right people are involved in the decision-makingprocess.
Salesforce flow: Salesforce flow is a visual tool that allows users to build complex, multi-stepprocesses using a drag-and-drop interface. With Salesforce flow, users can automate tasks such asupdating records, creating tasks, and sending email notifications. Salesforce flow can also integratewith other automation tools, such as Process Builder and Workflow, to create more complexbusiness processes.
Lightning App Builder: Lightning App Builder is a tool that allows users to create customSalesforce applications using drag-and-drop components. With Lightning App Builder, users canautomate tasks such as updating records and displaying real-time data.
Automation scenario and use cases
There are numerous scenarios and use cases where automation can be applied in Salesforce tostreamline business processes and increase productivity. Here are some examples of commonautomation scenarios and use cases: Lead management: Automating lead management processes can save time and increase theefficiency of sales teams. For example, a workflow can be created to automatically route leads tothe appropriate sales representative based on their location, product interest, or other criteria. AProcess Builder can also be used to automatically update lead status, assign tasks to sales reps,and send email notifications.

---

## Page 25

Opportunity management: Automating opportunity management processes can help salesteams manage their opportunities more effectively. For example, a process can be created toautomatically update the opportunity stage when certain criteria are met, such as when a certainamount of time has elapsed since the last contact with the prospect. A workflow can also be usedto notify sales reps when opportunities reach a certain stage or when new opportunities arecreated.
Customer service: Automating customer service processes can help organizations provide fasterand more efficient support to their customers. For example, a workflow can be created toautomatically route customer cases to the appropriate support agent based on their productexpertise or customer history. An approval process can also be used to ensure that customerservice requests are reviewed and approved by the appropriate parties before being resolved.
Reporting: Automating reporting processes can save time and increase the accuracy of dataanalysis. For example, a report can be scheduled to run automatically and sent to specific users orgroups on a regular basis. A dashboard can also be created to display real-time data from multiplesources, providing users with a quick and easy way to monitor key business metrics.
Lead routing: A business-to-business (B2B) software company uses Salesforce to manage itssales pipeline. They have a workflow in place to automatically route leads to the appropriate salesrep based on geographic location and product interest. This automation has saved the sales teamtime by ensuring that leads are assigned quickly and efficiently.
Quote generation: A manufacturing company uses Salesforce to manage their sales process.They have created a Process Builder to automatically generate quotes based on the customer'sproduct and pricing information. This automation has reduced errors and saved the sales team timeby eliminating the need to manually create quotes.
Customer onboarding: A software as a service (SaaS) company uses Salesforce to manageits customer onboarding process. They have created a Salesforce flow to guide new customersthrough the onboarding process, which includes setting up their accounts, configuring theirsettings, and completing required forms. This automation has improved the customer experience bymaking the onboarding process more efficient and streamlined.
Data integration: A marketing company uses Salesforce to manage their customer data. Theyhave integrated Salesforce with their marketing automation platform to automatically synccustomer data between the two systems. This automation has reduced errors and improved dataaccuracy while also saving time by eliminating the need for manual data entry.
Customer expectations and business processes
Customers have certain expectations when they interact with a business, and these expectations areoften shaped by their past experiences and the reputation of the business. For example, customers mayexpect a business to respond quickly to their inquiries, provide high-quality products or services, offercompetitive prices, and be easy to do business with.
To meet these expectations, businesses need to have efficient and effective business processes in place.Business processes are the series of steps or activities that a business uses to achieve a specific goal oroutcome. These processes may involve various departments and stakeholders within the business, suchas marketing, sales, operations, and customer service.
By optimizing their business processes, businesses can improve their ability to meet customerexpectations. For example, a business may streamline its order fulfillment process to ensure thatcustomers receive their products quickly and accurately. A business may also implement a CRM systemto provide better support and service to its customers.

---

## Page 26

Figure 1.1: Business process lifecycle
Overall, the success of a business depends on its ability to understand and meet the expectations of itscustomers. As illustrated in Figure 1.1, with a business process lifecycle and by aligning the businessprocesses with customer expectations, a business can create a positive customer experience and buildlong-term relationships with its customers.
Customer expectations and business processes for automation
Automation can play an important role in meeting customer expectations and optimizing businessprocesses. By automating certain tasks and processes, businesses can improve efficiency, reduce errors,and provide a more consistent experience for customers.
For example, businesses can use automation to: Respond to customer inquiries: By implementing chatbots or virtual assistants, businesses canquickly respond to customer inquiries and provide basic support around the clock.
Order processing: Automating the order processing system can ensure that orders are fulfilledquickly and accurately, with minimal errors.
Inventory management: By automating inventory management, businesses can ensure thatthey always have the right products in stock and can reduce the risk of stockouts or overstocking.
Payment processing: Automating payment processing can reduce the risk of errors and improvethe speed and accuracy of transactions.
Customer feedback: Automated surveys and feedback tools can help businesses gather valuableinsights from customers and improve their products and services accordingly.
Challenges with other automation tools
Workflow rules and Process Builder are both powerful automation tools in Salesforce, but they do havetheir own challenges.
Workflow rules are limited in their capabilities and can only perform certain types of actions, such asupdating fields or sending email alerts. They also have a limited number of rule criteria and actions thatcan be defined, which can make them difficult to use for more complex automation needs.
Process Builder, on the other hand, allows for more complex automation by allowing multiple criteriaand actions to be defined in a single process. However, this complexity can also make it more difficult tocreate and manage processes, especially if there are multiple processes running at the same time.
Some challenges with both workflow rules and Process Builder include:

---

## Page 27

Order of execution: It can be difficult to determine the order of execution for these tools, whichcan impact the accuracy of the automation.
Debugging: Debugging can be challenging with these tools, especially when it comes toidentifying errors or issues that are causing the automation to fail.
Maintenance: As business processes change, it can be difficult to update and maintain existingworkflows and processes, especially if there are a large number of them.
Testing: Testing can be difficult, as there are often multiple scenarios to consider, and it can betime consuming to test all of them thoroughly.
Overall, while workflow rules and Process Builder can be powerful automation tools, they do come withtheir own set of challenges that need to be considered when implementing automation solutions inSalesforce.
Expectations and reality with business logic
Business logic refers to the rules and processes that govern how data is processed and managed withina software application. Expectations and reality with business logic can vary depending on the specificapplication and the complexity of the business logic involved.
Expectations with business logic may include: Consistency: Business logic is expected to ensure consistency and accuracy of data throughoutthe application.
Efficiency: Business logic is expected to perform tasks quickly and efficiently, without causingdelays or errors in the system.
Flexibility: Business logic is expected to be flexible and adaptable to changing businessrequirements, allowing for updates and modifications as needed.
Security: Business logic is expected to protect sensitive data and prevent unauthorized access tothe system.
However, the reality of business logic can sometimes fall short of these expectations, especially if theapplication is complex or poorly designed. Some challenges that can arise with business logic include: Complexity: Business logic can become very complex, making it difficult to maintain and modifyover time.
Inconsistency: Inconsistencies can arise if business logic is not properly implemented or if thereare conflicts between different rules and processes.
Performance issues: Business logic can impact system performance if it is not optimized or ifthere are bottlenecks in the system.
Security vulnerabilities: Business logic can introduce security vulnerabilities if it is not properlydesigned and implemented.
Overall, while business logic can be a powerful tool for managing data and processes within anapplication, it is important to have realistic expectations and to ensure that the business logic is properlydesigned and implemented to avoid potential issues.
Mindset and mapping for automation
Having the right mindset and mapping out a clear plan is crucial for successful automation. Here aresome tips to consider:

---

## Page 28

Embrace change: Embrace the idea that automation is not a threat but a tool that can enhanceproductivity, reduce errors, and streamline processes.
Identify processes: Identify processes that can be automated. Look for repetitive, manual, andtime consuming tasks that can be performed by machines.
Prioritize tasks: Prioritize the processes that will provide the most significant benefits whenautomated. Start with the low-hanging fruits and work your way up to more complex tasks.
Evaluate tools: Evaluate automation tools that will best suit your organization's needs. Considerfactors like cost, compatibility, and ease of use.
Plan for integration: Plan for the integration of automated processes with existing systems.Ensure that the automation tools can integrate seamlessly with other tools and processes.
Communicate and train: Communicate the automation plan to all stakeholders and trainemployees on the new processes. Make sure everyone understands the benefits and how to usethe new tools.
Monitor and optimize: Monitor the automated processes to ensure that they are working asintended. Continuously optimize the processes to improve performance and efficiency.
By adopting the right mindset and mapping out a clear plan, automation can lead to significant benefitsfor your organization.
As illustrated in Figure 1.2, you should also look at these three areas in a task or work process toidentify that it should be automated: Repetitious mind-deadening work, similar to copy/paste and data entry.
Fragile work that sees a lot of mortal error, like typos or forgotten ways.
Timely recreating tasks, similar to monuments and automatic responses.
Figure 1.2: Developing the automation mindset
Developing an automation mindset is essential to unlocking the full potential of automation in yourorganization. Here are some steps you can take to develop an automation mindset: 1. Learn about automation: Educate yourself and your team about automation, its benefits, and itspotential impact on your industry. Read articles, attend webinars, and participate in trainingprograms to understand the various tools and technologies available.

---

## Page 29

2. Identify opportunities: Identify opportunities for automation in your organization by analyzingexisting processes and workflows. Look for tasks that are repetitive, time-consuming, or prone tohuman error.3. Focus on outcomes: Focus on the outcomes of automation rather than the process. Considerhow automation can improve productivity, increase efficiency, and reduce costs.4. Be open to change: Embrace change and be willing to adapt to new ways of working. Encourageyour team to experiment and try new tools and technologies.5. Collaborate: Collaborate with stakeholders across the organization, including IT, finance, andoperations. Work together to identify opportunities for automation and develop a plan forimplementation.6. Measure success: Establish metrics to measure the success of your automation initiatives.Monitor performance and make adjustments as needed to optimize outcomes.7. Continuously learn: Keep up-to-date with new tools, technologies, and trends in automation.Attend conferences, read industry publications, and participate in training programs to stay current.
Developing an automation mindset requires a willingness to change and a commitment to continuouslearning. By embracing automation, you can unlock new levels of productivity and efficiency in yourorganization.
Conclusion
In conclusion, Salesforce automation is becoming increasingly necessary in today's fast paced businessenvironment. It can help organizations improve productivity, reduce errors, and streamline processes.However, adopting an automation mindset and mapping out a clear plan is crucial for successfulimplementation. This involves identifying opportunities, prioritizing tasks, evaluating tools, planning forintegration, communicating and training, and monitoring and optimizing processes.
While the expectations for automation are high, it is important to keep in mind the reality ofimplementing automation with business logic. Automation can only work as well as the business logicand processes it is based on. Thus, it is crucial to align customer expectations with business processesand ensure that automation aligns with the overall business strategy.
Ultimately, successful automation requires a commitment to continuous learning and improvement. Byembracing automation and developing an automation mindset, organizations can gain a competitiveadvantage and achieve their business goals.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 30

CHAPTER 2Introducing Salesforce flow’s Features andCapabilities
Introduction
In this chapter, you will learn flow concepts and deep dive into what flow is and what can be achievedby flow. We dive into the world of workflow, Process Builder, and Salesforce flow within the Salesforceecosystem. In today's dynamic business environment, streamlining processes and automating repetitivetasks are paramount for organizations to stay competitive. This chapter aims to provide acomprehensive introduction to these tools, enabling readers to harness their power and drive efficientbusiness operations.
Structure
The chapter covers the following topics: Workflow and Process Builder
Salesforce flow
Salesforce flow capabilities
Essential feature and potential function of flow
Think like a pro for Salesforce flow
Introduction and start with pre-built automation
Objectives
The objective of this chapter is to provide readers with a comprehensive understanding of workflow,Process Builder, and Salesforce flow, along with insights on how to leverage them effectively within theSalesforce platform. You will explore the breadth of tasks that can be accomplished using Salesforceflow, and you will learn about the key features and functionalities of Salesforce flow.
Workflow and Process Builder
Salesforce offers several tools to automate and streamline business processes, including workflow andProcess Builder.
 
 Note: Salesforce will end support for workflow rules and Process Builder on December 31, 2025. To ensure your
automations stay current, we recommend migrating them to flow Builder by that date. Why the change? Salesforce is
focusing on flow Builder as a unified, low-code automation solution that is both modern and extensible. This shift allows
for more powerful and scalable automation, making flow the primary tool for future development and innovation in
Salesforce.

---

## Page 31

Workflow in Salesforce
Workflow is a tool in Salesforce that allows businesses to automate repetitive tasks and standardizetheir business processes. It provides a simple drag-and-drop interface to create rules that automaticallytrigger actions when specific conditions are met. Workflow rules can be used to update fields, sendemail alerts, create tasks, and even submit approvals.
To create a workflow rule, you first need to define the criteria that will trigger the rule. This can be doneby specifying a set of conditions that must be met for the rule to activate. Once the criteria are defined,you can then specify the actions that should be taken when the rule is triggered.
Scenario: Create a workflow rule that sends an email alert to a sales manager whenever a newopportunity is created with a value of over $100,000. Figure 2.1 shows how the workflow rule iscreated:
Figure 2.1: Workflow rule creation
Workflow rules in Salesforce are powerful, but they do have some limitations. For example, Workflowcannot trigger other workflow rules. Salesforce sets limits on rules and actions you can have, as well aslimits on the number of emails you can send each day and how often time-based triggers can run.
Process Builder in Salesforce
Process Builder is a more advanced tool in Salesforce that allows businesses to automate complexbusiness processes. It provides a visual interface to create rules that can perform multiple actions andupdate multiple records at the same time.
To create a Process Builder rule, you first need to define the criteria that will trigger the rule. This canbe done by specifying a set of conditions that must be met for the rule to activate. Once the criteria aredefined, you can then specify the actions that should be taken when the rule is triggered. Unlikeworkflow rules, Process Builder rules can perform multiple actions, including updating custom fields,creating records, posting to Chatter, and even invoking Apex code.
Consider the following scenario: When the status of a case is updated to Escalated, an email should be sent to the user, and thedescription of the case should be updated to Case is Escalated.
When a case is updated with the Case origin set to Email, the Subject should be updated to Caseorigin is Email.
Figure 2.2 shows how it will be implemented through Process Builder:

---

## Page 32

Figure 2.2: Process Builder with multiple criteria
Process Builder is more flexible and powerful than workflow, but it also requires more expertise to useeffectively. It can be used to automate complex business processes, such as lead qualification, customeronboarding, and contract management.
Key differences between workflow and Process Builder
Workflow is a simple tool that is used to automate basic tasks, while Process Builder is a more advancedtool that is used to automate complex business processes. Let us see the difference between the two ofthem in the following table:
 
 Key variances
 
 Workflow
 
 Process Builder
  
  Complexity
  
  Allows simple automation like sending email
alerts and updating fields.
  
  Allows complex automation like the creation of related records,
calling apex.
  
  Object support
  
  Supports a single object at a time.
  
  Supports multiple objects and their relationships.
  
  Real-time vs.
scheduled
  
  Executes in near real-time.
  
  It can be scheduled to execute at specific times.
  
  Debugging
  
  Has limited debugging capabilities.
  
  Offers better debugging options and allows users to test and
troubleshoot automation processes more easily.
  
  Flexibility
  
  Provides limited access to perform any
action.
  
  Provides more flexibility and can automate a wider range of actions.
  
  Execution order
control
  
  It gives simple control over the order of
execution.
  
  Gives more detailed control over the order of execution.

---

## Page 33

Salesforce initially offered workflow rules for basic automation tasks like field updates and email alerts,and later introduced Process Builder, which enabled more complex, multi-step automations. WithSalesforce flow now consolidating these capabilities, workflow rules and Process Builder have beenretired, as flow offers a more powerful, flexible, and unified approach to automation
Salesforce flow
Salesforce flow is a powerful tool in Salesforce that allows businesses to automate complex businessprocesses. It provides a visual interface to create custom flows that can perform multiple actions,including creating records, updating fields, and sending emails. Figure 2.1 shows a list of availableSalesforce flows in a Salesforce Org:
Figure 2.3: Salesforce flows
Why use Salesforce flow
Salesforce flow is a powerful tool that can help businesses automate complex business processes. Someof the benefits of using Salesforce flow include: Increased productivity: Salesforce flow can automate repetitive and time consuming tasks,allowing your team to focus on more important work.
Improved accuracy: By automating tasks, Salesforce flow can help reduce the risk of errors andinconsistencies.
Customization: Salesforce flow allows businesses to create custom flows that are tailored to theirspecific needs.
Flexibility: Salesforce flow can be used in a variety of different ways, from simple automationtasks to complex business processes.
Functions with Salesforce flow
Salesforce flow allows businesses to create custom flows that can perform a variety of different actions.Some of the most common use cases for Salesforce flow include: Lead qualification: Salesforce flow can be used to automate the lead qualification process,allowing businesses to quickly identify the most promising leads.

---

## Page 34

Customer onboarding: Salesforce flow can be used to automate the customer onboardingprocess, helping new customers get up to speed quickly and efficiently.
Contract management: Salesforce flow can be used to automate the contract managementprocess, helping businesses keep track of contracts and ensure that they are renewed on time.
Approval processes: Salesforce flow can be used to automate approval processes, helpingbusinesses streamline their workflows and improve efficiency.
Using Salesforce flow
To use Salesforce flow, you first need to define the flow's starting point, which is typically a button or alink. Once the starting point is defined, you can then define the flow's logic, which includes theconditions that must be met for the flow to run and the actions that should be taken when the flowruns.
Salesforce flow uses a visual interface to create flows, making it easy to define complex logic andcustomize the flow's behavior. You can also use Apex code to extend the functionality of Salesforce flowand create custom actions.
Salesforce flow capabilities
Salesforce flow is a powerful tool with a wide range of capabilities. Here are some of the key capabilitiesof Salesforce flow: Automating business processes: Salesforce flow can automate a wide range of businessprocesses, from simple to complex. Flows can be designed to automate data entry, data updates,record creation, record deletion, and more.
Integration with external systems: Salesforce flow can be used to integrate with externalsystems, such as web services, to automate data exchange between different systems.
Decision-making: Salesforce flow allows for decision-making within the flow based on specificconditions. The flow can route the data and actions to different paths based on the criteria set.
Loops and iterations: Salesforce flow supports looping and iteration, allowing for the automationof processes that involve multiple records or actions.
User interaction: Salesforce flow can interact with users, allowing them to make choices andinput data as part of the flow.
Data manipulation: flows can manipulate data within Salesforce, including creating, updating,deleting, and querying records, as well as performing calculations and transformations.
Versioning and deployment: flows allow versioning and deployment processes.
Integration with Apex code: Salesforce flow can be extended with Apex code, allowing for evenmore complex business processes to be automated.
Debugging: Salesforce flow provides debugging tools, allowing administrators to troubleshootissues and optimize flows for performance.
Mobile support: Salesforce flow is designed to work seamlessly with the Salesforce mobile app,allowing users to access and run flows on their mobile devices.
Reusability: Salesforce flow can be reused across multiple processes and objects, allowing forgreater efficiency and consistency in business processes.
Essential features and potential functions
In this section, we look at some of the essential features and potential functions of Salesforce flow.
Essential features

---

## Page 35

Salesforce flow offers a variety of capabilities that empower users to create automated processes,streamline data management, and deliver guided user experiences. Here are some of its key features: Visual designer: Salesforce flow provides a visual interface that makes it easy to design andcreate flows. The visual designer allows you to drag and drop elements to create your low, makingit simple to create complex flows with multiple actions and decision points.
Guided processes: Screen flow guides users through a series of screens, providing instructionsand collecting information along the way.
Automation on record changes: Triggered flows are initiated automatically in response torecord changes, such as record creation or modification.
Automation without user interaction: Autolaunched flows are initiated by an external event orprocess, without requiring user interaction.
Scheduled execution: Scheduled flows are triggered at predefined times or intervals, allowing forautomated processing on a schedule.
Data maintenance: Scheduled flows are often used for data maintenance tasks, such asarchiving old records or performing periodic data cleanup.
Potential functions
Salesforce flow can be leveraged for a variety of practical applications to improve efficiency andaccuracy in business operations. Here are some potential functions of Salesforce flow: Data entry automation: Salesforce flow can automate data entry tasks, such as creating newrecords or updating existing records, saving time and reducing errors.
Survey and feedback collection: Salesforce flow can be used to automate survey and feedbackcollection, allowing businesses to gather valuable insights from their customers and stakeholders.
Custom business processes: Salesforce flow can be used to create custom business processesthat are specific to your organization's needs. By using Salesforce flow, businesses can automateand streamline their unique processes, increasing efficiency and productivity.
Guided data entry: Create guided processes for users to input data through a series of screens,ensuring data accuracy and completeness.
Data validation: Validate user input and enforce data integrity rules to prevent errors andinconsistencies in Salesforce records.
Salesforce flow provides a range of capabilities, features and potential functions that can helpbusinesses automate and streamline their processes, making them more efficient and effective.
Think like a pro for Salesforce flow
It is important to utilize the best capabilities and features of Salesforce flow. By following these tips, youcan start thinking like a professional when using Salesforce flow: Define your goals: Before you start designing a flow, it is important to define your goals. Whatdo you want to achieve with the low? What business process do you want to automate? Whatspecific actions do you want the flow to perform? Defining your goals upfront will help you create aflow that is tailored to your needs and will ensure that the flow is designed to meet your specificbusiness requirements.
Identify your process: Once you have defined your goals, identify the specific process that youwant to automate. This will help you understand the flow's inputs, outputs, and logic. Byunderstanding the process, you can design a flow that will automate it efficiently and effectively.

---

## Page 36

Keep it simple: When designing a flow, it is important to keep it simple. Avoid overcomplicatingthe flow with unnecessary steps or logic. Focus on automating the key steps of the process, andmake sure that the flow is easy to understand and use.
Test thoroughly: Before deploying a flow, test it thoroughly to ensure that it works as expected.Test it in different scenarios and with different inputs to make sure that it is robust and reliable.This will help you avoid errors and ensure that the flow performs as expected in real-worldscenarios.
Optimize for performance: When designing a flow, optimize it for performance. This meansdesigning the flow to be efficient and fast, minimizing the number of steps and calculations neededto achieve the desired outcome. By optimizing for performance, you can ensure that the flow runssmoothly and efficiently, saving time and resources.
Leverage best practices: Finally, when designing a flow, leverage best practices and industrystandards. This will help you design a flow that is scalable, maintainable, and easy to use. It willalso ensure that the flow is consistent with other processes and Workflows in your organization.
Introduction and start with pre-built automation
An easy way to get started with Salesforce flow is to use pre-built automation.
Pre-built automation refers to pre-built flows that are available in Salesforce. These pre-built flows canbe used as templates to automate common business processes, such as lead management, opportunitymanagement, and case management.
Using pre-built automation in Salesforce flow can save you time and effort, allowing you to automatecommon business processes quickly and easily. Once you have customized a pre-built flow to fit yourspecific needs, you can deploy it in your organization and start reaping the benefits of automatedworkflows and streamlined processes.
To get started with pre-built automation, navigate to the All + Templates section in Salesforce asshown in Figure 2.4. Here, you will find a range of pre-built flows that can be used to automatedifferent business processes:
Figure 2.4: Flow Template
By using pre-built automation, you can quickly and easily automate common business processes withouthaving to start from scratch. This can save time and resources and help you get up and running withSalesforce flow more quickly.

---

## Page 37

Pre-built automation includes Standard flow Templates and flow Templates from AppExchange. Gettingconfused? No worries, here are some key differentiators to help you get these in an easy way: Pre-built automation: Pre-built automation refers to pre-built flows that are available inSalesforce. These pre-built flows can be used as templates to automate common businessprocesses, such as lead management, opportunity management, and case management. Pre-builtautomation can save time and resources by providing a starting point for your automation needs.
Standard flow Templates: Salesforce provides a range of Standard flow Templates that can beused to automate common business processes. These templates can be found in the flowTemplates section of Salesforce. Standard flow Templates are designed to be customizable and canbe adapted to meet your specific business requirements. Examples of Standard flow Templatesinclude the lead conversion flow and the opportunity management flow.
Flow Templates from AppExchange: In addition to Standard flow Templates, there are alsoflow Templates available from AppExchange. AppExchange is Salesforce's marketplace for third-party applications, including pre-built flow Templates. These templates are created by third-partyvendors and can be used to automate a wide range of business processes. Some flow Templatesfrom AppExchange are free, while others may require a fee.
To use a pre-built flow Template, simply select the template you want to use and customize it to meetyour specific needs. Depending on the template, you may need to modify the flow's inputs, outputs, andlogic to ensure that it meets your specific business requirements.
By using pre-built automation, whether Standard flow Templates or flow Templates from AppExchange,you can save time and resources while still creating effective and efficient automation solutions thatmeet your business needs.
Standard flow Templates and flow Templates from AppExchange both function the same, but standardflows are provided as part of your Salesforce application, and flow Templates can be installed from ourpartners via the AppExchange.
Here are some of the key benefits of using Standard flows and flow Templates: Access industry best practices: Explore how Salesforce and our partners have built seamlessflows and mirror those techniques for your own.
Tailor flows to your specific business needs: Evaluate whether the flows match your exactneeds and further customize them.
Whether you use Standard flows or flow Templates, these pre-built flows allow you to automate withouthesitation.
Conclusion
Salesforce flow offers a more powerful and flexible automation solution than workflow and ProcessBuilder, making it an excellent choice for businesses that require more complex automation capabilities.
Salesforce is starting the process of moving away from workflow rules and Process Builder andtransitioning to feature rich functionality of flow. This transition is set to take place in multiple phases.The first phase began with the Winter ’23 release, wherein the ability to create net-new workflow ruleswas turned off. In the Summer ’23 release, the ability to create net-new processes in Process Builderwas disabled. In the last phase, workflow rules and Process Builder will go away entirely, and anyplatform automation will be leveraging flow only.
It is imperative to mention here that there are tools available to migrate from workflow rules andProcess Builder to flow. One such tool is Migrate to flow.
So, businesses using Salesforce should consider the benefits and capabilities of flow and evaluatewhether it would be a better fit for their automation needs.

---

## Page 38

Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 39

CHAPTER 3Up and Running with Salesforce flow
Introduction
Salesforce flow is a powerful automation tool that enables users to automate complex businessprocesses, integrate with other systems, and streamline their operations. There are several types offlows available, including screen, autolaunched, and scheduled flows. Each type of flow has its own setof features and capabilities, making it easier for users to create custom workflows that meet theirspecific needs.
Data manipulation and management are vital aspects of any automation solution, and Salesforce flowprovides robust capabilities in this regard. This chapter will help you to explore flows data elements,which empower you to access, manipulate, and store data within your flow.
At the end of this chapter, you will have a comprehensive understanding of the key concepts andfunctionalities of Salesforce flow.
Structure
The chapter covers the following topics: Types of Salesforce flow
Flows elements, connectors, and resources
Flows data elements
Assignment and Loop elements
Creating a formula in flow
Decision in flow
Objectives
The objective of this chapter is to provide a comprehensive guide to Salesforce flow, a powerfulautomation tool that allows users to automate business processes and create custom applicationswithout writing code. This chapter covers the types of flow, including flow elements, connectors, andresources, as well as topics such as flows data elements, Assignment, Loop, formula and Decision inflow.
Types of Salesforce flow
There are several types of Salesforce flow, each with its own specific use case and functionality. Asillustrated in Figure 3.1, here are some of the most common types:

---

## Page 40

Figure 3.1: Types of Salesforce flow Screen flow: Screen flow is a type of flow that allows users to create custom screens and formswith the help of the Lightning App Builder. These screens and forms can be used to collect datafrom users or display information to them. Screen flows are ideal for creating custom interfaces forusers that may not be familiar with Salesforce, or for streamlining data entry processes.
Record-triggered flow: Record-triggered flow is a type of flow that is triggered when a specificrecord is created, updated, or deleted. This type of flow is typically used to automate businessprocesses that are tied to specific records. For example, you might use a record-triggered flow toautomatically update the status of an opportunity when it reaches a certain stage in the salesprocess.
Schedule-triggered flow: Schedule-triggered flow is a type of flow that runs at a scheduled timeor interval. This type of flow is typically used to automate tasks like data cleanup or record updates.For example, you might use a schedule-triggered flow to automatically update all of the records ina certain object every night at midnight.
Platform event-triggered flow: Platform event-triggered flow is a type of Salesforce flow thatenables event-driven automation by leveraging Platform Events. It launches when a Platform Eventmessage is received. This autolaunched flow runs in the background.
Autolaunched flow (No Trigger): An autolaunched flow is a flow that can be triggeredautomatically by a process or an Apex trigger. This type of flow is typically used to automatebusiness processes or integrate with other systems. For example, you might use an autolaunchedflow to automatically update a record in Salesforce when a new lead is added to your marketingautomation system.
Record-triggered orchestration: Record-triggered orchestration is a type of Salesforce flow thatallows you to automate and orchestrate complex business processes based on changes or eventsrelated to records in Salesforce. It enables you to define a sequence of actions and conditions thatare triggered when specific record-related events occur, such as record creation, update, ordeletion. Record-triggered orchestration flows provide a powerful tool for streamlining andautomating record-based workflows and business processes within the Salesforce platform. Anorchestration lets you create a multi-step, multi-user process.
These are the most common types of Salesforce flow, and each type has its own specific use case andfunctionality. By understanding the different types of Salesforce flow, you can choose the right type of

---

## Page 41

flow for your specific business needs and automate your processes efficiently.
Subflow
Before we move forward, let us not forget the subflow.
Subflow refers to a modular and reusable unit within a larger flow. It allows you to encapsulate a set ofactions and decisions into a separate flow, which can be called and used within other flows.
Subflow provides several benefits. These are: Reusability: Subflows can be used multiple times within different parent flows, promoting codereuse and reducing redundancy.
Modularity: By breaking down complex flows into smaller, manageable subflows, you can improveflow readability, maintainability, and troubleshooting.
Encapsulation: Subflows encapsulate a specific set of actions, allowing you to abstract andorganize logic in a more structured manner.
Ease of maintenance: When updates or modifications are needed, you can make changes to thesubflow once, and those changes will be reflected in all parent flows using it.
So, a subflow is a flow that can be called from another flow. This type of flow is typically used to breakup complex flows into smaller, more manageable parts. For example, you might use a subflow to handlea specific part of a larger flow, like sending an email or updating a record.
Flows elements, connectors, and resources
In Salesforce flow, there are three key components: elements, connectors, and resources. Let us take alook at them: Elements: Elements are the building blocks of a flow. Each element represents a specific action ordecision point within the flow, such as creating a record, updating a record, or sending an email.Elements can be added to a flow from the flow Designer and can be customized to suit the specificneeds of the flow.
Connectors: Connectors are used to connect elements within a flow. Each connector represents aspecific relationship between two elements and is used to define the flow of data and logic betweenthem. There are two types of connectors in Salesforce flow: input connectors and outputconnectors. Input connectors are used to bring data into an element, while output connectors areused to pass data out of an element.
Resources: Resources are reusable components that can be used across multiple flows. There areseveral types of resources in Salesforce flow, including variables, formulas, and Apex actions.Variables are used to store data that can be used across different elements within a flow, whileformulas are used to perform calculations and manipulate data. Apex actions are used to call Apexcode from within a flow, allowing for greater customization and functionality.
Together, these three components form the foundation of Salesforce flow, allowing users to createcustom workflows, automate business processes, and integrate with other systems. By leveragingelements, connectors, and resources, users can create powerful and flexible flows that can streamlinetheir business operations and increase efficiency.
Flows data elements
In Salesforce flow, data elements are used to manipulate and store data within a flow. There are severaltypes of data elements that can be used in a flow, including:

---

## Page 42

Variables: Variables are used to store data within a flow. There are several types of variables thatcan be used, including text, number, Boolean, date/time, and sObject. Variables can be initializedwith default values or values passed in from other elements within the flow.
Collections: Collections are used to store multiple values within a flow. Several types ofcollections can be used, including lists and maps. Lists are used to store an ordered collection ofvalues, while maps are used to store key-value pairs.
Records: Records are used to represent a single record within Salesforce. Records can be created,updated, or deleted within a flow and can be used to pass data between different elements withinthe flow.
sObjects: sObjects are used to represent a type of record within Salesforce, such as an account,contact, or opportunity. sObjects can be queried, created, updated, or deleted within a flow andcan be used to interact with other records and objects within Salesforce.
Formulas: Formulas are used to manipulate data within a flow. Formulas can be used to performcalculations, manipulate text, or create conditional logic within the flow.
By leveraging these data elements within a flow, users can create powerful and flexible workflows thatcan automate their business processes, streamline their operations, and integrate with other systems.By storing and manipulating data within a flow, users can create custom interfaces, perform complexcalculations, and interact with records and objects within Salesforce.
Assignment and Loop Elements
In Salesforce flow, there are two important elements used to control the flow of the process:Assignment and Loop elements. Let us take a look at them: Assignment element: The Assignment element is used to set values to variables or fields inrecords. It is commonly used to assign values to variables before they are used later in the flow.This element is useful when the user wants to set the value of a variable or field to a specific valueor formula, or when the user wants to store the output of an element in a variable or field. Theassignment element can be configured to perform complex operations, such as concatenation orarithmetic operations. functionality. Assignment element is illustrated in Figure 3.2:
Figure 3.2: Assignment element Loop element: The Loop element is used to iterate over a collection of data and perform anoperation on each item in the collection. The Loop element is useful when the user wants to

---

## Page 43

perform the same operation on multiple items in a collection, such as creating records or updatingfields. Loop element is illustrated in Figure 3.3:
Figure 3.3: Loop element
By leveraging the assignment and loop elements within a flow, users can create powerful and flexibleworkflows that can automate their business processes, streamline their operations, and integrate withother systems. These elements allow users to set values, perform calculations, and iterate overcollections of data within a flow, enabling them to create custom interfaces, perform complexcalculations, and interact with records and objects within Salesforce.
Creating a formula in flow
To create a formula in Salesforce flow, follow these steps: 1. Open the flow Builder by navigating to Setup | Process Automation | flows.2. Create a new flow or open an existing flow to which you want to add a formula.3. Click the New Resource button under Toolbox and choose Formula as a Resource Type asillustrated in Figure 3.4:

---

## Page 44

Figure 3.4: New Resource
4. Give the API Name of your choice and choose Data Type.5. In the Formula editor, you can create your formula using the available functions and operators. Youcan use any of the supported functions and operators in your formula, including arithmetic, logical,and comparison operators.6. Once you have created your formula, click Done to save it.7. You can now use the formula in other elements within the flow, such as an Assignment element ora Decision element.
 
 Note that the syntax for creating a formula in flow is similar to the syntax used in other Salesforce tools, such as formula
fields and validation rules. You can use variables, records, and other data elements in your formula to create powerful
calculations and logic within your flow.
Also, it is important to note that the formula language in flow is slightly different from the formulalanguage used in other Salesforce tools, such as formula fields and validation rules. Make sure to referto the Salesforce documentation for the specific syntax and functions available in flow formulas.
Decision in flow
In Salesforce flow, the Decision element is used to evaluate a condition and direct the flow of theprocess based on the result. The Decision element allows you to specify different paths for the flow tofollow based on the outcome of the evaluation.
To create a Decision element in Salesforce flow, follow these steps: 1. Open the flow Designer by navigating to Setup | Process Automation | flows.2. Create a new flow or open an existing flow that you want to add a Decision element to.3. Click on the Add element icon (+) in the canvas as illustrated in Figure 3.5:

---

## Page 45

Figure 3.5: Add Element
4. Select Decision from Logic elements as illustrated in Figure 3.6:
Figure 3.6: Add Decision element
5. In the Decision element, you can create your condition using the available operators and functions.You can use any of the supported operators and functions to create your condition, includingcomparison operators, logical operators, and functions that evaluate the values of variables orfields.6. Once you have created your condition, you can specify the actions to take based on the outcome ofthe evaluation. You can create multiple outcomes in the Decision element, each with its own set ofactions to take.7. You can now connect the Decision element to other elements in the flow, such as an Assignmentelement or a Loop element, based on the outcome of the evaluation.
The Decision element is useful when you want to create a branch in your process based on a condition.For example, you might use a Decision element to direct the flow of a process based on the value of a

---

## Page 46

variable or field, such as creating a record if the value of a field is greater than a certain threshold orsending an email if a certain condition is met.
By leveraging the Decision element within a flow, users can create powerful and flexible workflows thatcan automate their business processes, streamline their operations, and integrate with other systems.The Decision element allows users to evaluate conditions and direct the flow of the process based onthe outcome, enabling them to create custom interfaces, perform complex calculations, and interactwith records and objects within Salesforce.
Let us analyze a sample flow and subflow to understand the implementation of two key processes. Wewill delve into the details of how to create flow and subflow concepts in the upcoming chapter. Sending an email to a contact upon their creation (Figure 3.7):
Figure 3.7: A flow implementation Executing a subflow for the employee onboarding process, which incorporates department specifictasks using subflow (Figure 3.8)

---

## Page 47

Figure 3.8: Call of subflow
Conclusion
In this chapter, you learned that Salesforce flow is a powerful automation tool that enables users toautomate complex business processes, integrate with other systems, and streamline their operations.There are several types of flows available, including screen, autolaunched, and scheduled flows. Eachtype of flow has its own set of features and capabilities, making it easier for users to create customworkflows that meet their specific needs.
In next chapter, you will learn implementation and debugging of Salesforce flow where you will gaininvaluable insights into leveraging the full potential of the flow Builder, a powerful tool that empowersyou to visually construct your flows.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 48

CHAPTER 4Salesforce flow Implementation and Debugging
Introduction
In this chapter, you will learn how to implement and debug the flows effectively. You will explore flowBuilder. You will understand how to create and configure flows, run them, and troubleshoot any issuesthat may arise. Additionally, you will learn to examine paused and failed flow interviews and learn howto resolve them.
The primary purpose of this chapter is to equip you with the knowledge and skills to effectivelyimplement and debug Salesforce flows. You will learn to create flows, configure their behavior, andhandle common debugging scenarios.
This chapter is intended for Salesforce administrators, developers, and anyone interested in learningabout Salesforce flows. Whether you are new to flow development or looking to enhance your existingskills, this chapter will provide valuable insights and practical guidance for implementing and debuggingflows.
We will provide step-by-step instructions, best practices, and troubleshooting techniques to ensure yoursuccess in implementing Salesforce flows. Let us get started with exploring the flow Builder in the nextsection.
By the end of this chapter, you will have a comprehensive understanding of implementing anddebugging Salesforce flows.
Structure
The chapter covers the following topics: Exploring the flow Builder
Creating your flow
Run your flow and flow versions
Debugging the flow
Troubleshooting flows
Paused and failed flow interviews
Objectives
The objective of this chapter is to help you understand the capabilities and benefits of Salesforce flows.You will also familiarize yourself with the flow Builder interface and know how to create and configureflows to automate business processes. The chapter will also help you to understand the concept of flowversions and how to manage them.
In this chapter, you will also learn techniques for debugging and troubleshooting flows effectively andalso gain knowledge on handling paused and failed flow interviews.

---

## Page 49

Exploring the flow Builder
You have learned that flow Builder is a powerful and intuitive tool provided by Salesforce that allowsadministrators and developers to design and automate business processes without the need for code.With its user friendly interface, the flow Builder simplifies the creation and management of flows,empowering users to build complex workflows efficiently. In this section, we will take an in-depth lookat the various features and components of the flow Builder.
Elements
The flow Builder revolves around the concept of elements, which are the building blocks used toconstruct flows. These elements represent specific actions or decisions within the flow. The followingfigure illustrates some elements:
Figure 4.1: Elements
Figure 4.1 illustrates some of these elements, and some commonly used elements include: Record create: Creates new records in Salesforce objects.
Record update: Updates existing records with new values.
Decision: Evaluates conditions and directs the flow based on the outcomes.
Loop: Iterates over a collection of records or variables.
Screen: Displays a visual interface to collect user input or present information.
Resources
Resources in the flow Builder provide additional functionalities and data for your flows. They can beused to define variables, store values, or perform specific actions.
As illustrated in Figure 4.2, the following are some examples of resources:

---

## Page 50

Figure 4.2: Resources Variable: A variable stores data that can be used throughout the flow. It can hold various datatypes, including text, numbers, dates, and collections.
Constant: A constant represents a fixed value that remains the same throughout the flow.
Formula: A formula resource allows you to perform calculations or manipulate data usingSalesforce formula syntax.
Screens
Screens in the flow Builder are used to create interactive user interfaces within flows. Screens candisplay information, prompt users for input, or present choices. You can design screens using variouscomponents such as text fields, picklists, checkboxes, and radio buttons. Screens provide a seamlessuser experience by allowing users to input data and make decisions directly within the flow. A NewScreen is illustrated in Figure 4.3:
Figure 4.3: Screen

---

## Page 51

Flow logic
The flow Builder enables you to define the logic and flow of your process using various tools. You canincorporate Decision elements to evaluate conditions and determine the next steps based on theoutcomes. By utilizing flow logic effectively, you can create dynamic and adaptive flows that cater todifferent scenarios. Figure 4.4 illustrates a Decision element where you can implement your logic withcondition requirements, outcomes, and resources:
Figure 4.4: Decision logic
Testing and previewing
The flow Builder provides a built-in testing and previewing functionality that allows you to validate andreview your flow before deploying it. You can simulate user interactions, test different scenarios, andevaluate the behavior and outcomes of your flow. This testing capability ensures that your flowfunctions as intended and meets your requirements.
As illustrated in Figure 4.5, the Debug button will help you in understanding the flow's behavior andpreviewing functionality:
Figure 4.5: Buttons in flow
It is important to note that the Debug button will be enabled after you save your changes using theSave button. Likewise, the Save button will be enabled once you make any changes in the flow. In thenext section, you will learn how to utilize Save and Debug buttons.
Let us take a quick look at each button available in Salesforce flow Builder: Run: The Run button allows you to execute the flow and see how it behaves in real-time. It isuseful for testing and validating the logic and functionality of your flow. Clicking on the Run buttonwill trigger the flow and show you the results.

---

## Page 52

Debug: The Debug button is used for troubleshooting and understanding the flow's behaviorduring execution. When you click on the Debug button, it opens the flow Debugger, whichprovides detailed information about the flow's variables, values, and the path followed by the flowelements. It helps you identify any issues or errors in the flow and provides insights into how thedata is flowing through the flow's elements.
Activate: The Activate button is used to make a flow available for use in your SalesforceOrganization. By activating a flow, you make it accessible to users, and they can interact with itbased on the defined entry criteria and configuration. After making any changes to the flow, youneed to activate it for those changes to take effect.
Save As: The Save As button allows you to create a copy of an existing flow. This feature ishandy when you want to create a similar flow based on an existing one but with somemodifications. Clicking on Save As opens a dialog where you can provide a new name anddescription for the copied flow and save it as a new flow in your organization.
Save: The Save button is used to save any changes made to the flow. It allows you to persist themodifications you have made to the flow's elements, properties, and settings. Until you save a flow,the changes you make are only temporary and will be lost if you navigate away or refresh the page.Once saved, the flow becomes available for further editing, activation, and use.
These buttons play essential roles in the flow Builder interface, enabling you to create, modify, test, anddeploy flows within Salesforce.
Creating your flow
Let us walk through with the step-by-step process of setting up and configuring a flow using the flowBuilder to create flows and customize them to suit your specific business needs.
Accessing the flow Builder
Follow the given steps to access the flow Builder: 1. To begin with, navigate to the flow Builder within Salesforce.2. From Setup (Figure 4.6), enter Flows in the Quick Find box:
Figure 4.6: Setup
3. Then select Flows (Figure 4.7):

---

## Page 53

Figure 4.7: flows
Creating a new flow
Follow these steps to create a new flow: 1. To create a new flow, click on the New flow button (Figure 4.7).2. Select Screen flow and click on Create (Figure 4.8):
Figure 4.8: Create flow
Adding elements
Once you have created a new flow, you can start adding elements to define its behavior. Elementsrepresent actions, decisions, and screens within the flow. Follow the given steps: 1. On the flow canvas, on the path after the Start element, hover over Add element and click Addelement icon (+) in the canvas as illustrated in Figure 4.9:

---

## Page 54

Figure 4.9: Add element
2. As illustrated in Figure 4.10, click on Screen. The New Screen window opens:
Figure 4.10: Add screen
3. As illustrated in Figure 4.11, under Screen Properties for Label, enter Hello World.4. The API Name is automatically set to Hello_World.
Figure 4.11: New Screen properties
Configuring screen components
As you are building a screen flow, you will need to design the user interface to collect input or presentinformation. Within the screen element, you can add components such as text fields, picklists,checkboxes, and buttons. Follow the given steps: 1. As illustrated in Figure 4.11, under Components, you can review the available components.

---

## Page 55

Figure 4.12: Screen with display component
2. As illustrated in Figure 4.12, from the Components pane, drag the Display Text onto the screencanvas.3. The properties pane now represents the Display Text output component.4. In the properties pane, for API Name, enter Message.5. In the properties pane, in the text area, enter Congratulations on creating your first Screen flow!.6. Click Done.7. Click Save.8. As illustrated in Figure 4.13, give your flow name by entering the Flow Label of your choice. TheFlow API Name is automatically set. Enter Description so it will be helpful to review your flowsin the future:

---

## Page 56

Figure 4.13: Save the flow
9. Click Save. Your flow should look like Figure 4.14:
Figure 4.14: My First flow
Whenever you add new elements to your flow or make any new changes to it, it is important to saveyour progress. Click on the Save button in the flow Builder to save your changes.
After saving, you can debug the flow, and after verifying your changes, you can activate the flow tomake it available for use.
Activating the flow ensures that it is ready to be triggered manually or by an automated process. Followthese steps: 1. As illustrated in Figure 4.14, click on the Debug button. After clicking on the Debug button, a newtab of the browser will open.2. Keep the default selected checkboxes for Debug Options and click on the Run button.

---

## Page 57

3. Figure 4.15 displays your message from the Display Text component on the screen, and thissimple flow is running as per your expectation:
Figure 4.15: Debug flow
4. Close this new browser tab, and you will be back to your flow as in Figure 4.14.5. Click on the Run button, and you will see the screen as illustrated in Figure 4.16. Please note, thistime Debug Details are not available:
Figure 4.16: Run flow
6. Return back to flow Builder (Figure 4.14) again.7. Click on the Activate button.
Now your first flow is available for use in your Salesforce Organization.
Run your flow and flow versions
Once you have created and configured your Salesforce flow, it is time to execute and run it to automateyour business processes. In this section, we will explore the various methods of running a flow andmanaging different versions of the flow.
Running a flow
There are several ways to run a flow within Salesforce, depending on your requirements and use cases.Let us look at some common methods: Running in the flow Builder: In the flow Builder, you can execute your flow directly for testingand validation purposes. This method is useful during the development and debugging phase,allowing you to simulate user interactions and observe the flow's behavior step by step. We havedemonstrated the steps above in Figure 4.16.
Embedded on a home page: You can embed the above screen flow onto a Salesforce homepage using the Lightning App Builder. This enables users to interact with the flow directly from thehome page. For example, you can create a flow to guide users through a complex process likeonboarding a new customer or submitting a support request from the home page.
Flow versions

---

## Page 58

As you continue to enhance and modify your flows, it is essential to manage different versionseffectively. Salesforce provides version control capabilities to track and manage changes made to a flowover time. Here is how you can handle flow versions: Creating versions: When you make significant changes to a flow, it is a best practice to create anew version. This allows you to preserve the previous version and its functionality while introducingenhancements or modifications in the new version. Each version maintains its own unique identifier,allowing you to differentiate between them. Follow the given steps:
1. Click on the Save As button in the flow builder (Figure 4.17).
2. As illustrated in Figure 4.17, you will have the option to choose A New Version or A NewFlow. A new version: This option allows you to create a new version of an existing flow. Whenyou choose A New Version, you are essentially duplicating the current flow and creatinga new iteration while retaining the previous versions. It helps maintain a history ofchanges and allows for easy comparison between different versions.
A new flow: This option enables you to create an entirely new flow from scratch.Choosing A New Flow means you are starting fresh without any connection orassociation with an existing flow. This option is suitable when you want to create a distinctflow with its own unique logic and functionality. It is not linked to any previous versions orconfigurations and allows you to build a flow from the ground up according to yourspecific requirements. The following figure shows the window:
Figure 4.17: New version of flow
As illustrated in Figure 4.17, keep the option A New Version selected.
You should update the Description. It is good practice to keep track of your all changesfor all versions history.
Click on Save.
Activating versions: Before a flow can be executed, it needs to be activated. You can activate aspecific version of a flow to make it available for use. By activating a version, you ensure that thelatest changes are applied and that users can interact with the flow as intended.

---

## Page 59

You have already learned how to activate a flow by clicking on the Activate button(Figure 4.14). You can click on the Activate button to activate the current version ofthe flow. It will automatically deactivate previous versions of this flow.
Managing version history: Salesforce keeps a history of all the versions created for a flow. Thisversion history allows you to review and compare different versions, roll back to a previous versionif necessary, and track the evolution of your flow over time. It provides visibility and control overthe changes made, promoting transparency and efficient development. Follow the given steps:
1. To go back to the flow definitions page, click on the Back arrow as illustrated in Figure 4.18:
Figure 4.18: Go back to flowdefinitions page
2. From the flow definitions page, you can review all versions of flow after clicking on ViewDetails and Versions, as illustrated in Figure 4.19:
Figure 4.19: flow definitions page
Testing with versioned flows: When making changes to a flow, it is crucial to test the updatedversion thoroughly before activating it. By testing a new version, you can verify that the changeswork as expected and that they do not impact the existing functionality or user experience. Testingensures that your flows are reliable and perform as intended.
Managing flow versions allows you to iteratively improve your flows while maintaining stability andcontrol. It facilitates collaboration among administrators and developers by providing a structuredapproach to development and deployment.
Debugging the flow
Debugging is an essential part of the flow development process, as it helps identify and resolve issuesor unexpected behavior in your Salesforce flows. In this section, we will explore various techniques andtools available for debugging flows effectively: Debug in the flow Builder: flow Builder offers a built-in debugging feature that allows you tointeractively test and analyze your flow's behavior. As already demonstrated in this chapter inFigure 4.15, you have learned how to use the Debug button. With the Debug option, you can stepthrough each element of the flow, view variable values, and identify any issues or unexpected

---

## Page 60

outcomes. This interactive debugging capability facilitates a granular understanding of the flow'sexecution and aids in pinpointing and resolving errors.
Debug logs: Salesforce provides debug logs that capture detailed information about the executionof your flows. By enabling debug logging for the running user or specific users, you can gaininsights into the flow's behavior, variable values, and any errors or exceptions encountered. Debuglogs can be viewed in the developer console or on the setup menu, providing a valuable resourcefor troubleshooting flow related issues.
Error messages and notifications: During flow execution, Salesforce provides error messagesand notifications to indicate any issues encountered. These messages can provide valuable insightsinto the cause of the error, such as incorrect input values or missing configuration. By carefullyreviewing error messages and notifications, you can quickly identify and address flow relatederrors.
Fault connectors: Within flow Builder, you can utilize fault connectors to handle exceptions orerrors gracefully. By adding fault connectors to elements, you can define alternative paths or errorhandling logic when a specific condition fails, or an error occurs. Fault connectors allow you toguide the flow's execution based on different outcomes, providing a robust approach to handlingerrors and unexpected situations.
Testing and validation: Thorough testing and validation of your flow are crucial to ensure itsfunctionality and reliability. By creating test scenarios that cover different use cases and dataconditions, you can verify the expected behavior of your flow and identify any potential issuesbefore deploying it in a production environment. Automated testing tools like Salesforce Apex testclasses can also be utilized to validate the flow's functionality.
Collaborative troubleshooting: In complex flow scenarios, collaboration with otherstakeholders, such as administrators or developers, can be beneficial. Discussing the flow'sbehavior, sharing debug logs, and leveraging the expertise of others can help identify and resolveissues more efficiently. Collaborative troubleshooting promotes knowledge sharing and can lead toinnovative solutions.
Rollback mode in debug: When debugging in Salesforce flow, all changes are saved as if theywere real runs, even if the flow has not been activated yet. These changes remain in place. Toprevent this, you can use rollback mode, which cancels any changes made during debugging.
Remember, if you debug a flow without choosing to run it in rollback mode, the flow performs itsactions, including any DML operations and Apex code execution. Also, closing or restarting a runningflow does not rollback its previously executed actions, callouts, and changes committed to the database.
By utilizing these debugging techniques and tools, you can identify and resolve issues in your Salesforceflows effectively. Debugging flows ensures that they function as intended, delivering automation, andstreamlining business processes.
Troubleshooting flows
Troubleshooting is an essential skill when working with Salesforce flows. Despite careful planning andimplementation, issues can arise during flow execution. In this section, we will explore commontroubleshooting techniques and provide guidance on resolving issues that may occur in your flows: Review flow configuration: Start by reviewing the configuration of your flow. Ensure that allelements, variables, and resources are properly set up. Check if any required fields are missingvalues or if there are any misconfigured assignments or conditions. Reviewing the configuration canhelp identify any errors or omissions that may be causing the issue.
Check flow variables: Verify the values of flow variables during execution. Debug logs and theflow Builder's debug mode can be valuable tools for inspecting variable values and identifying

---

## Page 61

discrepancies. Ensure that the expected values are assigned to variables correctly and that they arebeing used consistently throughout the flow.
Validate formula expressions: If you are using formula expressions within your flow, validatethem carefully. Check for any syntax errors or incorrect field references. Make sure that theformulas correctly evaluate conditions and return the expected results. Debug logs can provideinsights into formula evaluation and help identify any issues.
Handle validation errors: Validation rules on objects or fields can cause flow errors. If your flowencounters validation errors during execution, review the specific error messages to identify thecause. Adjust the flow's logic or data inputs accordingly to comply with the validation rules.
Troubleshoot data related problems: If your flow is interacting with data, ensure that the datais accurate and complete. Check if the required records or fields exist and contain the expectedvalues. Data related issues can occur when working with lookups, record updates, or recordcreations. Verifying the data integrity and correctness can help resolve such problems.
Examine error messages and logs: Error messages and logs are valuable sources of informationfor troubleshooting flow issues. Pay close attention to any error messages encountered during flowexecution. Examine debug logs, system logs, and error notifications to gain insights into the causeof the problem. Look for specific error codes, exception messages, or details that can guide you inresolving the issue.
Test incrementally: If you encounter issues in a complex flow, consider testing it incrementally.Divide the flow into smaller sections or subflows and test each component individually. By isolatingspecific sections, you can pinpoint the problematic area and focus your troubleshooting effortsmore effectively.
Collaborate with others: Do not hesitate to seek assistance from your colleagues, Salesforcesupport, or the broader Salesforce community. Engaging in collaborative troubleshooting can bringfresh perspectives and insights to resolve complex flow issues. Share your flow details, errormessages, and debug logs with others to gain their expertise and suggestions.
Documentation and knowledge sharing: Document the issues you encounter and the solutionsyou implement. Maintain a troubleshooting log to record the problems you faced, the steps taken toresolve them, and the outcomes. This log can serve as a valuable resource for futuretroubleshooting and help others facing similar challenges.
By applying these troubleshooting techniques, you can effectively identify and resolve issues in yourSalesforce flows. Troubleshooting is an iterative process that requires patience and attention to detail.With practice and experience, you will become more proficient at resolving flow related issues.
Paused and failed flow interviews
During the execution of Salesforce flows, you may encounter paused and failed flow interviews. Thesesituations can occur due to various reasons and require specific actions to resolve. In this section, wewill explore paused and failed flow interviews, their causes, and steps to address them effectively.
From Setup, enter Paused in the Quick Find box, then select Paused And Failed Flow Interviews asillustrated in Figure 4.20:

---

## Page 62

Figure 4.20: Paused and failed flow interviews
Paused flow interviews
Paused flow interviews occur when a flow execution is interrupted or suspended, typically due to userinteraction requirements or dependencies on external processes. Here is how to handle paused flowinterviews: 1. Identify paused flow interviews: To identify paused flow interviews, navigate to the flowInterview section in Salesforce Setup. Here, you can view a list of all paused flow interviews.Analyze the details of each paused interview to understand the reasons behind the interruption.2. Resume or terminate paused flow interviews: Once you have identified the paused flowinterviews, you can take appropriate actions to resume or terminate them. Resuming a paused flowinterview allows it to continue from where it left off, while terminating the interview stops itsexecution. Consider the requirements and consequences of each paused flow interview beforedeciding to resume or terminate.
Failed flow interviews
Failed flow interviews occur when a flow execution encounters errors or exceptions that prevent it fromcompleting successfully. It is important to identify and resolve the underlying issues causing the failures.Follow these steps to handle failed flow interviews: 1. Identify failed flow interviews: Similar to paused flow interviews, you can review the flowInterview section in Salesforce Setup to identify failed flow interviews. Analyze the error messagesassociated with each failed interview to understand the causes of the failures.2. Analyze error messages: Examine the error messages and exception details provided for failedflow interviews. Pay attention to any specific error codes, stack traces, or error descriptions.Understanding the root cause of the failure is crucial for implementing appropriate solutions.3. Debug and fix issues: Once you have identified the causes of the failed flow interviews, usedebugging techniques and tools to diagnose the issues. Review the flow's configuration, variables,formulas, and any integration points for potential errors. Make the necessary adjustments toaddress the issues and retest the flow.4. Test and monitor: After fixing the issues, thoroughly test the flow to ensure that the failed flowinterviews are resolved. Create test scenarios that cover the previously failed areas and verify thatthe flow executes successfully without encountering any errors. It is also recommended to monitorthe flow's execution after the fixes to ensure its continued reliability.5. Iterative improvement: If you encounter recurring failed flow interviews, consider a systematicapproach to identify and address the underlying issues. Review the flow's design, dependencies,and error handling mechanisms to improve its stability and error resilience. Documentation andknowledge sharing within your team can aid in iterative improvement.
Handling paused and failed flow interviews effectively is crucial for maintaining the stability andefficiency of your Salesforce flows. Regularly monitor and review flow executions, promptly address anyissues, and continuously improve the flow's performance.
Conclusion
In this chapter you learned the implementation and debugging aspects of Salesforce flows. You learnedhow to create and configure flows using the flow Builder, run and manage flow versions, and effectivelydebug and troubleshoot flows. Understanding these techniques is essential for ensuring smoothautomation of business processes within the Salesforce platform.

---

## Page 63

In the next chapter, you will learn about creating screen flows that will cover a range of topics includingidentifying the need for screen flows and the problem statement, understanding the fundamentals ofscreen flow, collecting information through screen flows, implementing business logic in screen flows,displaying records within screen flows, distributing screen flows, handling errors and fault paths inscreen flows, utilizing subflows and a modular approach, and finally, key learnings from the chapter.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 64

CHAPTER 5Creating Screen flows
Introduction
In this chapter, you will learn the powerful capabilities of Salesforce screen flows and how they can beused to enhance user experiences and streamline business processes. We will dive into thefundamentals of screen flows, where you will learn how to collect information, implement business logic,display records, handle errors, and distribute flows.
Screen flows are powerful tools that allow you to create interactive and guided experiences for users,streamlining processes and improving productivity.
We will begin by exploring the problem statement and identifying the need for screen flows. Byunderstanding common business challenges and pain points, we can effectively leverage screen flows toaddress these issues and optimize processes.
You will learn how to display records dynamically within screen flows, enabling users to interact withrelevant data during the flow's execution.
Next, you will learn distribution of screen flows, ensuring that users can access and benefit from themefficiently. We will explore various methods, such as embedding flows on Lightning Pages, creatingcustom buttons or links, and utilizing URL access.
Error handling and fault path management will also be a key focus in this chapter. We will discusstechniques for effectively handling errors within screen flows, guiding users towards resolution, andensuring a seamless user experience.
Lastly, we will explore the concept of subflows and the modular approach. By creating reusablesubflows, you can design flows that are organized, scalable, and easy to maintain, while promotingefficiency and consistency.
By the end of this chapter, you will have a comprehensive understanding of screen flows and theirapplications.
Structure
This chapter is organized into the following sections: Identifying the need for screen flows
Fundamentals of screen flow
Collecting information with screen flows
Implementing business logic in screen flows
Displaying records in screen flows
Distribution of screen flows
Error handling and fault path in screen flows

---

## Page 65

Subflows and modular approach
Key learnings
Objectives
By the end of this chapter, you will understand the significance of screen flows in enhancing userexperiences and streamlining business processes. You will also learn the fundamentals of screen flows,including their structure, elements, and capabilities. You will gain the knowledge and skills to collectinformation efficiently using screen flows.
The chapter will teach you how to implement business logic within screen flows to automate decisionmaking processes, display records dynamically within screen flows to provide relevant information tousers. You will also learn how to distribute screen flows effectively to users and stakeholders,understand error handling techniques and how to handle faults within screen flows.
With this chapter you will explore the concept of subflows and adopt a modular approach in screen flowdesign, and reflect on the key learnings and best practices for creating effective screen flows.
Identifying the need for screen flows
In today's fast paced business environment, organizations strive to deliver exceptional user experienceswhile streamlining their internal processes. However, many businesses face challenges in achievingthese goals efficiently. Let us explore some common scenarios that highlight the need for Salesforcescreen flows as a powerful solution: Complex data collection: In various business processes, there is often a need to collect multipledata points from users in a structured and user friendly manner. Traditional methods such asmanual data entry or paper based forms can be time consuming, error prone, and hinderproductivity. Screen flows provide a solution by enabling organizations to create intuitive andinteractive interfaces, guiding users step-by-step through data entry, validation, and submissionprocesses.
Guided user experiences: In many industries, especially those involving complex products orservices, guiding users through a predefined set of steps or processes is crucial. Without astructured approach, users may struggle to navigate through complex steps, resulting in frustrationand potential errors. Screen flows offer the ability to present users with guided experiences,ensuring that they follow the correct sequence of actions, provide accurate information, andachieve the desired outcomes.
Decision making and business rules: Businesses often have well defined rules and logic thatgovern their processes. Implementing these rules effectively and ensuring consistent adherence canbe a challenge. Screen flows provide a place to incorporate business logic and decision makingelements. By creating formulas, validation, and Decision elements, organizations can automatecomplex business rules within the flow, reducing manual effort and improving accuracy.
Real time data validation: Data accuracy is critical for businesses to make informed decisionsand maintain high-quality records. However, ensuring data validity in real time can be challengingwhen relying on manual data entry alone. With screen flows, organizations can implementvalidation rules and real-time data checks, instantly alerting users to errors or inconsistencies. Thisimmediate feedback reduces the likelihood of data entry mistakes and improves data integrity.
Enhancing user engagement: User engagement is crucial for driving productivity and ensuringuser adoption of new systems or processes. Screen flows provide an interactive and visuallyappealing interface that engages users, making data entry and process execution more enjoyable.By offering a user friendly experience, organizations can increase user satisfaction and encouragehigher participation in critical business processes.

---

## Page 66

Identifying these challenges and recognizing the need for Salesforce screen flows can help organizationstransform their processes, improve efficiency, and elevate the overall user experience. In the nextsection, we will explore the fundamentals of screen flows, laying the foundation for creating effectiveand impactful flow experiences.
Fundamentals of screen flow
To create effective and impactful screen flows, it is essential to understand the fundamentals of thispowerful Salesforce feature. In this section, we will explore the core components and concepts thatform the building blocks of screen flows: Purpose and structure: At its core, a screen flow is a visual representation of a step-by-stepprocess or workflow within Salesforce. It guides users through a series of screens, capturinginformation, making decisions, and performing actions. The structure of a screen flow consists ofscreens, elements, and connectors that define the flow's flow and logic.
Screen components: Screens are the primary interface elements in a screen flow, where usersinteract and provide information. Salesforce offers various screen components, including inputfields, picklists, radio buttons, checkboxes, and rich text components. These components enableusers to enter data, make selections, and provide the necessary information for the flow'sexecution.
Flow elements: flow elements are the building blocks that define the logic and behavior of ascreen flow. They allow you to perform actions, make decisions, loop through collections, andhandle exceptions. Elements such as Assignment, Decision, Loop, Record Create, and RecordUpdate provide the necessary functionality to create dynamic and interactive flows.
Flow connectors: Connectors establish the logical flow between elements and Screens in a screenflow. They define the sequence in which screens are presented to users and how the flowprogresses based on user input or flow outcomes. Connectors can be used to branch the flow, loopback to previous screens, or navigate to different parts of the flow based on specific conditions.
Variable and resource management: Variables play a crucial role in screen flows, allowing youto store and manipulate data throughout the flow's execution. Variables can capture user input,hold calculated values, or store information retrieved from Salesforce records. Resources, such ascustom labels or images, can be used to provide additional context or enhance the visualexperience within the flow.
Flow Builder: Salesforce provides a powerful and intuitive tool called the flow Builder fordesigning and configuring screen flows. The flow Builder offers a visual interface where you cancreate, modify, and test flows using a drag and drop approach. With its user friendly interface, theflow Builder empowers users with varying levels of technical expertise to design flows without theneed for extensive coding knowledge.
By understanding these fundamental concepts of screen flows, you can begin to design and create flowsthat address specific business requirements. In the upcoming sections, we will explore how to collectinformation, implement business logic, display records, handle errors, and distribute flows effectively.Through this journey, you will gain the skills to build dynamic and user centric screen flows thatoptimize your organization's processes and enhance user experiences.
Collecting information with screen flows
One of the primary purposes of screen flows is to collect information from users in a structured anduser friendly manner. In this section, we will delve into techniques and best practices for effectivelygathering information using screen flows: Designing user friendly screens: When designing screens for information collection, it is crucialto create a user friendly and intuitive interface. Consider organizing fields logically, grouping related

---

## Page 67

information together, and using clear and concise labels. Leverage screen components such asinput fields, picklists, and checkboxes to facilitate data entry and minimize user effort.
Validation and error handling: Implement validation rules and error handling within your screenflows to ensure data accuracy. Validate user inputs in real-time, providing immediate feedback ondata format or mandatory fields. Leverage field validation rules, formula fields, or custom logic toenforce data integrity. Clearly communicate error messages and guide users to correct any invalidor missing information.
Conditional visibility: In certain scenarios, you may need to collect different sets of informationbased on user selections or specific conditions. Use conditional visibility within screen flows to showor hide fields or sections dynamically. This helps simplify the data collection process for users,presenting them with only the relevant fields based on their selections or the flow's context.
Progress indicators and navigation: To enhance user experience and provide a sense ofprogress, incorporate progress indicators within your screen flows. Progress bars, step counters, orvisual cues can help users understand their position within the flow and the remaining steps. Clearnavigation options, such as Next, Previous, or Cancel, provide users with control and flexibility asthey move through the flow.
Prepopulating data: To streamline the data collection process and improve efficiency, considerprepopulating fields with known or default values. Leverage Salesforce's record lookup capabilitiesor custom formulas to automatically retrieve and populate relevant data. Prepopulating fieldsreduces user effort, minimizes errors, and enhances the overall user experience.
Multi step information gathering: For complex data collection scenarios, break the process intomultiple screens or steps within the screen flow. Each step can focus on a specific category ofinformation, allowing users to provide data in a structured and manageable manner. Progressindicators and clear instructions help users navigate through the multi-step flow seamlessly.
Mobile responsiveness: Consider the mobile responsiveness of your screen flows toaccommodate users accessing the flows on mobile devices. Ensure that the Screen components,layout, and navigation are optimized for smaller Screens and touch interactions. Test and validatethe flow's usability on various mobile devices to provide a consistent experience across platforms.
By applying these techniques for collecting information with screen flows, you can create user friendlyand efficient data entry experiences. In the next section, we will explore how to implement businesslogic within screen flows, enabling decision making and process automation.
Implementing business logic in screen flows
Implementing business logic within screen flows enables decision making and process automation,making the flows dynamic and intelligent. In this section, we will explore techniques and best practicesfor incorporating business logic into your screen flows: Decision elements: Decision elements are fundamental building blocks for implementing businesslogic within screen flows. They allow you to evaluate conditions and make branching decisionsbased on user input or data values. By defining criteria and outcomes, you can guide the flow'spath and dynamically adapt the user experience.
Formula fields: Leverage the power of formula fields to perform calculations, manipulate data,and drive decision making within your screen flows. Formula fields enable you to derive values,validate inputs, and automate calculations based on user-entered data or other variables within theflow. Use formula fields to simplify complex logic and provide real-time insights to users.
Variable assignment: Assigning values to variables within your screen flows plays a crucial role inimplementing business logic. Variables allow you to store and manipulate data throughout theflow's execution. Assign values dynamically based on user inputs, formula calculations, or data

---

## Page 68

lookups. By utilizing variables effectively, you can control the flow's behavior and make informeddecisions.
Looping and iteration: In scenarios where repetitive actions or iteration is required, leverageloop elements within your screen flows. Loops enable you to iterate through collections of data orperform actions multiple times based on specific conditions. Use loops to automate repetitive tasks,process multiple records, or present users with dynamic sets of options.
Integration with external systems: Screen flows can integrate with external systems, enablingseamless data exchange and business process automation. Utilize Salesforce Connect or Apexintegration to fetch data from external sources, validate against business rules, or trigger actions inother systems. By integrating with external systems, you can enhance the flow's capabilities andstreamline end-to-end processes.
Custom Apex logic: For complex business logic that goes beyond the capabilities of formula fieldsor flow elements, you can incorporate custom Apex logic within your screen flows. Apex allows youto write custom code to perform calculations, execute complex workflows, or integrate withexternal services. By leveraging Apex, you can extend the capabilities of your screen flows andtailor them to your specific business needs.
Error handling and exception management: Implementing error handling within your screenflows is crucial for providing a seamless user experience. Anticipate potential errors or exceptionsand define fault paths to handle them gracefully. Use Decision elements or conditional branching toguide the flow's execution based on error scenarios. Effective error handling ensures that users arealerted to errors and provided with clear instructions for resolution.
Validation rules: Validate user inputs and enforce business rules using validation rules within yourscreen flows. Ensure that data entered by users meets specific criteria or adheres to predefinedstandards. Validation rules help maintain data integrity and improve the accuracy of processedinformation. Display clear error messages when validation fails, guiding users to correct theirinputs.
By incorporating these techniques, you can create intelligent and dynamic screen flows that automatedecision making, streamline processes, and enhance user experiences. In the next section, we willexplore how to display records dynamically within screen flows, allowing users to interact with relevantdata during the flow's execution.
Displaying records in screen flows
Displaying records dynamically within screen flows enhances the user experience and provides userswith relevant information during the flow's execution. In this section, we will explore techniques andbest practices for effectively displaying records within your screen flows: Record lookup: Utilize the record lookup capability within screen flows to retrieve data fromSalesforce objects dynamically. By querying relevant records based on user input or flow variables,you can populate screen fields with data from Salesforce records. This enables users to view andinteract with existing data during the flow's execution.
Field mapping: When displaying records within screen flows, consider mapping fields fromSalesforce records to screen components. Field mapping ensures that the appropriate data isdisplayed in the correct fields on the screen. By presenting users with relevant information, you canprovide context and facilitate informed decision making.
Conditional display logic: To tailor the display of records based on specific conditions,incorporate conditional display logic within your screen flows. Based on user selections or flowvariables, dynamically determine which records to display and which fields to show or hide.Conditional display logic helps present users with a personalized view of relevant data, enhancingtheir interaction within the flow.

---

## Page 69

Related records and related lists: In scenarios where users need to view related records orrelated lists within the screen flow, leverage Salesforce's relationship fields and related lists.Displaying related records provides a comprehensive view of the data hierarchy and allows users toaccess additional information or perform related actions conveniently.
Visual representation: Consider incorporating visual representations, such as images, charts, orgraphs, within your screen flows to present data in a visually appealing manner. Visualrepresentations can help users quickly grasp complex information, identify trends, or make datadriven decisions. Use images or charts to enhance the visual experience and improve datacomprehension.
Real-time calculations: Display real-time calculations or derived values within your screen flowsto provide users with up-to-date insights. Leverage formula fields or custom calculations to performcalculations based on user inputs or retrieved data. Real-time calculations within the flow can assistusers in making informed decisions and streamline their interaction with the displayed records.
Interactive record actions: Enable users to perform actions on displayed records within thescreen flow itself. Incorporate buttons, links, or custom actions that allow users to edit, delete, orperform specific actions on the displayed records. Interactive record actions streamline userworkflows and reduce the need to navigate to separate pages or screens for record management.
By applying these techniques, you can create engaging and informative screen flows that present userswith relevant records and data. The ability to view and interact with records within the flow enhancesuser productivity, facilitates decision making, and optimizes business processes. In the next section, wewill explore the distribution of screen flows, ensuring that users can access and benefit from themefficiently.
Distribution of screen flows
Effectively distributing screen flows ensures that users can access and benefit from them efficiently. Inthis section, we will explore techniques and best practices for distributing screen flows to the right usersand stakeholders. Let us take a look at them: Embedding screen flows on Lightning Pages: One of the most common ways to distributescreen flows is by embedding them on Lightning Pages. Lightning Pages provide a flexible andcustomizable interface where you can add components, including screen flows. Embedding flows onrelevant pages allows users to access them within the context of their daily work, enhancingproductivity and reducing the need for navigation.
Creating custom buttons or links: Another approach to distributing screen flows is by creatingcustom buttons or links that launch the flow when clicked. You can add these buttons or links onrelevant Salesforce records or related lists, providing users with direct access to the flow. Custombuttons or links simplify the flow's accessibility, allowing users to initiate it seamlessly.
Utilizing URL access: URL access enables you to distribute screen flows by generating URLs thatdirectly open the flow. By leveraging URL parameters, you can prepopulate fields, pass data, or setspecific flow variables dynamically. This method allows you to distribute flows through variouschannels such as emails, chat applications, or external websites.
Including in Lightning App Builder: If you have built custom Lightning Apps using theLightning App Builder, consider adding screen flows as components within the app. This allowsusers to access the flows directly from the app's navigation or home page. Including flows inLightning Apps provides a centralized and cohesive user experience.
Controlling flow visibility: Ensure that the right users have access to the screen flows byleveraging Salesforce's visibility controls. Utilize profiles, permission sets, or sharing rules to controlwho can initiate or view specific flows. This ensures that only authorized users can access sensitiveor critical flows, maintaining data security and privacy.

---

## Page 70

Mobile accessibility: With the increasing usage of Salesforce mobile applications, ensure thatyour screen flows are mobile accessible. Optimize the flow's layout and screen components to bemobile-responsive, adapting to different screen sizes and touch interactions. Test the flow'susability on mobile devices to provide a consistent and seamless experience for mobile users.
User training and documentation: When distributing screen flows, provide clear documentationand training materials to educate users on how to access and utilize the flows effectively. Createuser guides, process documents, or video tutorials that outline the purpose of the flows, theirbenefits, and step-by-step instructions on accessing and interacting with them. This empowersusers to leverage the flows efficiently and reduces the learning curve.
Monitoring and continuous improvement: Regularly monitor the usage and effectiveness ofdistributed screen flows. Gather feedback from users and stakeholders to identify areas forimprovement and gather insights on user satisfaction. Use analytics and user feedback to refine theflow's design, optimize user experiences, and ensure that the distributed flows continue to meetevolving business needs.
By employing these distribution techniques and best practices, you can ensure that screen flows reachthe right users and stakeholders, enabling them to benefit from streamlined processes and enhanceduser experiences. In the next section, we will explore techniques for error handling and fault pathmanagement within screen flows.
Error handling and fault path in screen flows
Error handling is a critical aspect of creating robust and user friendly screen flows. In this section, wewill explore techniques and best practices for effectively handling errors and managing the fault pathwithin your screen flows: Identify potential error scenarios: Start by identifying potential error scenarios within yourscreen flows. Anticipate situations where user inputs may be invalid, required data is missing, orexternal dependencies fail. By understanding these scenarios upfront, you can proactively designerror handling logic to guide users and mitigate potential issues.
Error messaging and notifications: Clearly communicate errors and provide informative errormessages within your screen flows. Display user friendly messages that guide users on how toresolve the error or provide the missing information. Consider using validation rules, field level errormessages, or screen level notifications to effectively communicate errors and guide users towardresolution.
Conditional branching for error handling: Use Decision elements and conditional branchingwithin your screen flows to handle errors and route the flow's execution along the fault path. Bydefining conditions based on error scenarios, you can redirect users to specific screens oralternative paths to address the errors gracefully. Conditional branching ensures that users areguided toward resolution without disrupting the flow's overall progression.
Rollback and recovery: In some cases, errors may require a rollback of previous actions orrecovery to a stable state within the flow. Utilize screen components such as checkboxes orconfirmation screens to confirm critical actions before proceeding. If an error occurs, provide anoption for users to rollback to a previous point or restart the flow to ensure data consistency andminimize potential data corruption.
Logging and error tracking: Implement logging mechanisms within your screen flows to captureerrors and gather data for analysis and troubleshooting. Leverage Salesforce's debug logs orcustom logging techniques to record errors, exception details, and flow execution information.Logging helps identify patterns, diagnose issues, and improve the flow's overall reliability.
User guidance and help resources: When errors occur within your screen flows, provide userswith guidance on how to resolve the issues. Include contextual help text, tooltips, or links toknowledge articles to assist users in troubleshooting errors independently. Empowering users with

---

## Page 71

self-service resources reduces their reliance on support channels and improves their overallexperience.
Error recovery and flow continuity: Design your screen flows with error recovery mechanismsto enable users to resume their progress seamlessly after error resolution. Store user inputs or flowvariables temporarily, allowing users to pick up where they left off. Error recovery ensures thatusers can continue the flow's execution without the need to start from the beginning, providing asmooth and uninterrupted experience.
User testing and feedback: Regularly test your screen flows and gather feedback from users toidentify potential areas of improvement in error handling. Conduct user acceptance testing(UAT) to simulate real-world scenarios and validate error handling mechanisms. Incorporate userfeedback to refine error messages, troubleshoot common issues, and enhance the overall userexperience.
By implementing these error handling techniques and best practices, you can create robust and userfriendly screen flows that gracefully handle errors and guide users towards resolution. In the nextsection, we will explore the concept of subflows and the modular approach, allowing for reusable andefficient flow design.
Subflows and modular approach
In complex screen flow designs, implementing a modular approach with subflows can greatly enhanceefficiency and reusability. In this section, we will explore the concept of subflows and how they can beused to create more organized and scalable screen flows: Understanding subflows: Subflows are self-contained flow components that can be embeddedwithin other flows. They allow you to break down complex flows into smaller, more manageableunits. Subflows encapsulate a specific set of actions or logic, making the overall flow designmodular and easier to maintain.
Modular design benefits: By adopting a modular approach with subflows, you gain severalbenefits. Firstly, it allows for better organization and structure of your screen flows, as each subflowfocuses on a specific task or functionality. Secondly, the modular design promotes reusability, assubflows can be reused across multiple flows or even within the same flow. This saves time andeffort in development and maintenance.
Creating subflows: To create a subflow, identify a set of actions or logic that can be extractedand reused. Extract these actions into a separate flow, configure the necessary input and outputvariables, and define the desired behavior. Once created, the subflow can be invoked andembedded within other flows as a component.
Parameter passing: Subflows can accept input parameters to make them dynamic and adaptableto different contexts. Input parameters allow you to pass values or information from the parentflow to the subflow. This flexibility enables the subflow to perform its actions based on the specificdata or conditions provided by the parent flow.
Reusable components: As you create subflows, identify common actions or logic that can bereused across different flows. These reusable subflows act as building blocks, simplifying flowdesign and reducing duplication of effort. By centralizing the implementation of commonfunctionality, you ensure consistency and maintainability across multiple flows.
Encapsulation of business logic: Subflows provide a means to encapsulate business logic andcomplex decision making processes. By isolating specific logic within a subflow, you can focus on itsdevelopment, testing, and validation independently. This separation of concerns simplifies theoverall flow design and improves the readability and maintainability of the flows.
Promoting scalability: Modular designs with subflows allow for scalability as your flows grow incomplexity and size. Instead of managing a single monolithic flow, you can break it down into

---

## Page 72

smaller, manageable subflows. This promotes easier maintenance, debugging, and enhancementsas the individual subflows can be modified independently without impacting the entire flow.
Documentation and naming conventions: When working with subflows, maintain cleardocumentation and establish naming conventions to ensure clarity and ease of understanding.Document the purpose, functionality, and usage instructions of each subflow. Use consistent andmeaningful names for subflows and their parameters to facilitate easy identification and usagewithin the flows.
Adopting a modular approach with subflows allow you to create more organized, reusable, and scalablescreen flows. The use of subflows improve the overall maintainability and flexibility of your flow designs.In the final section, we will summarize the key learnings from this chapter and highlight importanttakeaways for creating effective screen flows.
Key learnings
Throughout this chapter on Creating Screen flows, we have covered various aspects of designing andimplementing effective screen flows. Let us summarize the key learnings and takeaways from thischapter: Screen flows are powerful tools for enhancing user experiences and streamlining businessprocesses within Salesforce.
Understanding the problem statement and identifying the need for screen flows is crucial inaddressing specific business challenges and improving productivity.
The fundamentals of screen flows include the purpose, structure, screen components, flowelements, connectors, and variable management.
Techniques for collecting information with screen flows involve designing user friendly screens,implementing validation rules, leveraging conditional visibility, and prepopulating data.
Implementing business logic in screen flows allows for decision making, formula calculations,conditional branching, and integration with external systems.
Displaying records within screen flows enhances user interactions, and techniques like recordlookup, field mapping, conditional display logic, and visual representations are valuable.
Effective distribution of screen flows can be achieved through embedding on Lightning Pages,custom buttons or links, URL access, inclusion in Lightning App Builder, and controlling flowvisibility.
Error handling and fault path management are crucial for providing a seamless user experience.Techniques include error messaging, conditional branching, rollback and recovery, logging, and userguidance.
Subflows and the modular approach enable better organization, reusability, and scalability of screenflows. They promote encapsulation of business logic and the creation of reusable components.
Clear documentation, naming conventions, and user training materials are essential for successfullyimplementing and adopting screen flows.
By internalizing these key learnings and incorporating them into your screen flow design practices, youcan create effective and impactful flows that enhance user experiences, optimize processes, and driveproductivity.
In the next chapter, we will explore advanced techniques for customizing and extending screen flowsfurther, empowering you to create even more sophisticated and tailored flow experiences.
Conclusion

---

## Page 73

In this chapter, we explored the creation of screen flows, from understanding their fundamentals toimplementing business logic, displaying records, handling errors, and distributing flows. Screen flowsprovide an interactive and user friendly approach to collecting information and automating processeswithin Salesforce. In the next chapter, we will delve into advanced techniques for customizing andextending screen flows further.
In this chapter, we have delved into the world of screen flows, exploring their capabilities andunderstanding how to create effective and impactful flow experiences. We began by identifying theneed for screen flows, addressing common business challenges and streamlining processes.
Throughout this chapter, we emphasized the significance of user experience, efficiency, andcustomization. By following best practices, incorporating validation rules, leveraging formula fields, andintegrating with external systems, we can create flows that align perfectly with specific businessrequirements.
As we conclude this chapter we encourage you to apply the key learnings and techniques covered inthis chapter. By doing so, you will be able to design and implement screen flows that drive userengagement, streamline processes, and deliver exceptional experiences within your SalesforceOrganization.
In the next chapter, you will learn real-time scenarios to bring the concepts of screen flows to life. Youhave learned the fundamentals and implementation techniques in the current chapter. Now, get readyfor hands-on examples of how screen flows can enhance user experiences, streamline processes, andautomate tasks in Salesforce. These practical use cases will inspire and empower you to adapt andcustomize screen flows to suit your organization's needs. Join us on this journey to revolutionize howyou interact with data and automate processes in Salesforce.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 74

CHAPTER 6Implementing Screen flows
Introduction
In this chapter, let us focus on requirements and use cases, specifically on Salesforce flow.
You will learn real-time scenarios to bring the concepts of screen flows to real use cases. The chapterhas hands-on examples of how screen flows can enhance user experiences, streamline processes, andautomate tasks in Salesforce.
We will begin by creating a screen flow that will act as a gateway for collecting fundamental details,including the candidate’s name, email address, phone number, emergency contact name, emergencycontact number, address, and start date.
Then, we will explain how to create a subflow dedicated to department and role selection. As part of theonboarding journey, we will guide new hires through this screen to help them choose their respectivedepartment and role. Using screen choice components, we will present them with pre-defined options.Whether they use radio buttons or drop-down lists, this stage ensures that new hires are activelyengaged in shaping their journey.
Next, we will create a dedicated screen in the same flow for document uploads. This screen will featurea file upload component, enabling new hires to easily upload identification proofs, certificates, contracts,and other essential documents.
By completing these meticulously designed steps, the employee onboarding process will be transformedinto a guided and efficient journey.
Structure
This chapter is organized into the following sections: Requirement discussion
Creating the employee onboarding flow
Creating subflow and using it
Distributing the screen flow
Objectives
By the end of this chapter, you will be able to understand the purpose and function of Salesforce screenflows. You will learn how to create and utilize subflows within screen flows for managing complexprocesses, how to use file upload components into screen flows for document submissions, andrecognize how screen flows can help you with the common challenges in employee onboarding.
You will be able to design user centric interactions within screen flows to enhance user experiences,efficiently collect the data using screen components, customize onboarding experiences using the

---

## Page 75

flexibility of Salesforce screen flows, and implement practical steps to create an employee onboardingscreen flow.
This chapter will guide users through department and role selection using screen choice components,help to create consistent and efficient onboarding experiences for new employees, and demonstratehow to distribute employee onboarding screen flows effectively to users.
Requirement discussion
As a beginner learning about screen flow in Salesforce, let us explore a practical use case forautomating the employee onboarding process using Salesforce screen flow. Employee onboarding is acritical process that involves welcoming and integrating new employees into an organization, ensuringthey have all the necessary information, resources, and training to become productive team members.Utilizing screen flow in Salesforce, we can create a guided and interactive onboarding experience fornew hires.
The benefits of using Salesforce screen flow for employee onboarding are as follows: User friendly experience: Screen flow provides a guided and interactive onboarding experience,making it easy for new hires to navigate through the process.
Efficient data collection: With screen components, we can efficiently collect and validate data,reducing the risk of errors and omissions during onboarding.
Customizable and scalable: Salesforce screen flow is highly customizable, allowing us to adaptthe onboarding process as the organization grows and changes.
Let us break down the requirements for employee onboarding with Salesforce screen flow in multipleparts, as discussed below: 1. Information collection: The screen flow starts to collect basic information from the newemployee, such as their name, contact details, emergency contact, and other necessaryinformation. We will use screen components like text and input to gather this data: 1. Create the screen flow.
2. The first screen captures essential information, such as Name, Email Address, Phone Number,Emergency Contact Name, Emergency Contact Number, Address, and Start Date.
2. Department and role assignment (subflow): In this section, the screen flow will guide thenew employee through selecting their department and role from predefined pick lists. We will usescreen choice components to present the options: 1. Create a screen flow that will be used as subflow to guide the new hire through selecting theirdepartment and role.
2. Use screen choice components to present the available department and role options.
3. The new hire can choose their department and role using radio buttons or drop down lists.
3. Document upload: The next step includes a screen where the employee can upload importantdocuments, such as identification proofs, certificates, and contracts. We will utilize the file uploadcomponent to facilitate this process: 1. Create a new screen for document uploads.
2. Include a file upload component on this screen, allowing the new hire to upload importantdocuments like identification proofs, certificates, and contracts.
4. Onboarding completion: Once the employee confirms all the details, the screen flow will createtheir record status accordingly in Salesforce.

---

## Page 76

After completing these steps, the new hire's onboarding process will be successfully guided througheach stage of the onboarding journey, capturing essential information, allowing document uploads, andselecting department and role. The use of Salesforce screen flow in this process streamlines theonboarding experience and ensures consistency and efficiency for all new employees joining theorganization.
Creating the employee onboarding flow
Follow the below steps for hands-on in your Salesforce Org:
Please note, before proceeding with the main flow, ensure that the necessary custom fields are created,as we are using custom fields in the example below.
 
 Please note, before proceeding with the main flow, ensure that the necessary custom fields are created, as we are using
custom fields in the example below.
 
1. Login to your Salesforce Org, and click on Setup, as shown in the following figure:
Figure 6.1: Salesforce setup option
2. Search flows in the Quick Find box, as shown:

---

## Page 77

Figure 6.2: Setup Home
3. Click on the New Flow button, as shown in the following screenshot:
Figure 6.3: View all flows
4. Select the Screen Flow type:

---

## Page 78

Figure 6.4: New flow options
5. Click on the Create button.6. Select the Add Element option and select the Screen component, as shown in the followingscreenshot:
Figure 6.5: Add Element
7. Fill in the details in the screen component properties: 1. Label: Employee Onboarding Form
2. API Name: Employee_Onboarding_Form
8. Add the input fields on the Screen Component: 1. Drag the Name from the components list to the screen canvas:1. API Name: Name
2. Click on Done.
2. Drag the Text from the components list to the screen canvas:1. Label Name: Company
2. API Name: Company

---

## Page 79

3. Click on Done.
3. Drag the Email from the components list to the screen canvas:1. Label Name: Email
2. API Name: Email
3. Click on Done.
4. Drag the Number from the components list to the screen canvas:1. Label Name: Phone Number
2. API Name: Phone_Number
3. Click on Done.
5. Drag the Text from the components list to the screen canvas:1. Label Name: Emergency Contact Name
2. API Name: Emergency_Contact_Name
3. Click on Done.
6. Drag the Number from the components list to the screen canvas:1. Label Name: Emergency Contact Number
2. API Name: Emergency_Contact_Number
3. Click on Done.
7. Drag the Date from the components list to the screen canvas:1. Label Name: Start Date
2. API Name: Start_Date
3. Click on Done.
Refer to Figure 6.6:
Figure 6.6: Edit Screen
9. Click Done.10. Add the Create Records element, as shown in the following figure:

---

## Page 80

Figure 6.7: Create Record element
A dialog box will open which will be as shown below:

---

## Page 81

Figure 6.8: Create Record element detail
11. Fill the following details: 1. Label: Create record for Employee Onboarding
2. API Name: Create_record_for_Employee_Onboarding
3. How Many Records to Create:
Select: One
4. How to Set the Record Fields:
Select: Use separate resources, and literal values.
In the Object, select the Lead object.
12. Map your input from the fields shown in the following figure:

---

## Page 82

Figure 6.9: Set field and values
The following table details the values to be filled:
 
 Field
 
 Value
  
Company  
  
  Company
  
Email  
  
  Email
  
Emergency_Contact_Name__c  
  
  Emergency_Contact_Name
  
Emergency_Contact_Number__c  
  
  Emergency_Contact_Number
  
FirstName  
  
  Name.firstName
  
LastName  
  
  Name.lastName
  
MobilePhone  
  
  phone
  
Start_Date__c  
  
  Start_Date
  
Status  
  
  Working – Contacted
Table 6.1: Field and value mapping13. Click on the Done button.14. Save this flow:

---

## Page 83

1. Flow Label: Employee Onboarding Form
2. Flow API Name: Employee_Onboarding
3. Click Save.
Creating subflow and using it
Let us create a new screen flow that will be used as shown below:
We are going to create a Department and Role Assignment Screen subflow. This is a new screenflow that will be used inside a main screen flow, as shown:
Figure 6.10: Subflow
Follow the steps below to create the subflow: 1. Create a new screen flow: In this screen flow, you will add one screen element.
On the screen, you will add two Picklist fields Department and Role as illustrated inFigure 6.11:
Figure 6.11 (a): Screen for department

---

## Page 84

2. Add screen: 1. Label: Department and Role Assignment Screen
2. API Name: Department_and_Role_Assignment_Screen
3. Add Picklist on Screen: 1. Label: Department
2. API Name: Departments
3. Component Type: Picklist
4. Choice: {!department}
4. Add Picklist on Screen: 1. Label: Role
2. API Name: Roles
3. Component Type: Picklist
4. Choice: {!role}
For selecting the appropriate department and role from the options provided, you need to create twochoice resources according to the steps outlined below: 1. Create New Choice Resource.2. Click on Choice field3. Select New Choice Resource as illustrated in Figure 6.11(b):
Figure 6.11(b): Select New Choice Resource
4. Select Resource Type: Picklist Choice Set as illustrated in Figure 6.11(c):

---

## Page 85

Figure 6.11(c): Resource Type
5. Enter the details as below: 1. API Name: department
2. Object: Lead
3. Data Type: Picklist
4. Field: Department__c
6. Click Done as illustrated in Figure 6.11(d):

---

## Page 86

Figure 6.11(d): New Choice Resource department
7. Similarly, create a new resource role as illustrated in Figure 6.11(e):
Figure 6.11(e): New Choice Resource role
8. After selecting the appropriate choices for Department and Role from the picklists, click theDone button, as shown in Figure 6.12:

---

## Page 87

Figure 6.12: Screen for role
9. Create a variable for Lead ID: 1. Create a Lead ID variable that will be accepted in the subflow when the main flow calls thesubflow.
2. For creating Lead ID, click on New Resource.
3. For Resource Type select Variable and create a new resource, as shown:

---

## Page 88

Figure 6.13: New Resource
10. You will have the option to add API Name and add other info as shown:
Figure 6.14: Choose variable resource
11. Enter the details as below: 1. API Name: leadId
2. Data Type: Text
3. Availability Outside the flow: Available for input
(This option will allow this variable to get assigned from main flow, that is, outside of thisflow.)12. Click on Done.

---

## Page 89

Figure 6.15: Create/edit new variable
Refer to the following steps (and Figure 6.15) to create and edit a new variable: 1. Add update record: 1. Label: Update Lead records
2. API Name: Update_Lead_records
3. How To Find Records To Update And Set Their Values:
Select: Specify conditions to identify records, and set fieldsindividually
4. Object: Lead
5. Condition Requirements To Update Records:1. Field: Id
2. Operator: Equals
3. Value: leadId
6. Set Field Values For The Lead Records:1. Field: Department__c Value: Departments
2. Field: Role__c Value: Roles
Click on Done as shown in Figure 6.16:

---

## Page 90

Figure 6.16: Update lead record 1. Save this flow: 1. Flow Label: Department and Role Assignment
2. Flow API Name: Sub_flow_of_Employee_Onboarding_Form
2. Click on the Save button.3. Open flow Employee Onboarding Form (You can go to Setup | flows, and all existing flow will bethere, or you can go back after clicking Back button in the top left corner of the current flowDepartment and Role Assignment)4. Add subflow after creating a record: 1. Click on the + icon, to select a Subflow:

---

## Page 91

Figure 6.17: Add Element
5. Click on Subflow, and the next screen will appear:
Figure 6.18: Calling subflow
6. Configure Subflow: 1. Label: Department and Role Assignment Subflow
2. API Name: Department_and_Role_Assignment_Subflow

---

## Page 92

3. Referenced flow: Department and Role Assignment
4. Set Input Values:
leadid:
{!Create_record_for_Employee_Onboarding}
Follow the given steps to the document upload screen: 1. In the screen flow Employee Onboarding Form, add one more screen element for adding a fileuploading section and, on this screen, add the file upload input components, as shown:
Figure 6.19: New screen for file upload 1. API Name: Upload_Document
2. File Upload Label: Upload Documents
3. Related record ID: {!Create_record_for_Employee_Onboarding}
2. Save and activate this flow by clicking on the Run button.
Distributing the Screen flow
As of now, to keep it simple, let us add your flow on the home page. Follow the given steps: 1. Go on App Launcher and search Sales app.2. Be on the home page, click on Setup and select Edit Page, as shown in the following screenshot:

---

## Page 93

Figure 6.20: Home page
You can see the Lightning App Builder page, as shown:

---

## Page 94

Figure 6.21: Lightning App Builder
3. Drag the flow component in the center.4. On the right side panel, you can select the flow name Employee Onboarding Form, which is the screenflow you want to add on the home page.5. Click on the Save and Activate button, after clicking on the Activate button:

---

## Page 95

Figure 6.22: Activate home page
6. You can assign this as Assign as Org Default and click on the Close button.
Go to the home page now you can use the screen flow from the home page, as shown:
Figure 6.23: flow on home page
After entering the information and following the steps in flow, you can check the new lead record fromthe Leads tab. Lead will have uploaded the document under the Files section.

---

## Page 96

Conclusion
In this chapter, we have started a practical journey into the world of Salesforce screen flows. You havelearned about creating screen flows and subflows with practical steps and why screen flows are usefulfor making things smoother for users and organizations.
You now know how screen flows can change the way new employees join a company, making it easierand more organized. You have learned how to collect information, use subflows for a modular approach,and upload important documents with a file upload component.
As we move ahead, using what we have learned here, we are getting ready for the next part of thejourney of Implementing record-triggered flows. The chapter will help us understand how to automatetasks when records are created, updated, or deleted. We will learn step by step, with real-worldexamples, and expand our skills in using Salesforce for record-based automation.
So, get ready for the next chapter, where we are going to explore more and learn how to make thingshappen automatically in Salesforce by identifying the need for record-triggered flows.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 97

CHAPTER 7Implementing Record-triggered Flows
Introduction
In this chapter, we will dive deep into the world of record-triggered flows and explore their practicalimplementation in Salesforce. Record-triggered flows are a powerful tool that allows you to automateprocesses and perform actions based on specific events or changes within records. By understandingthe fundamentals and mastering the techniques covered in this chapter, you will be able to effectivelyleverage record-triggered flows to streamline your business processes and enhance productivity.
Structure
This chapter is organized into the following sections: Fundamentals of record-triggered flows
Identify the need for record-triggered flows
Insert record-triggered flows
Criteria for the record trigger
Fast Field Updates
Actions and related records
Delete record-triggered flows
Objectives
By the end of this chapter, you will understand the fundamental concepts of record-triggered flows andtheir advantages. You will be able to recognize the scenarios where record-triggered flows are the mostappropriate solution. You will learn to create and configure record-triggered flows with various businessuse cases and with different criteria.
We will explore how to implement fast field updates to automate field value population based onspecific conditions.
In this chapter, you will learn to extend the capabilities of record-triggered flows using actions andrelated records. With an easy example, we will explain how to automate the process when a record isdeleted from Salesforce Org. The goal of this chapter is to familiarize you with flow Trigger Explorer andits usage for analyzing and troubleshooting flows. You will have valuable insights and key learnings forsuccessfully implementing record-triggered flows in your organization.
Fundamentals of record-triggered flows
Record-triggered flows are a type of automation in Salesforce that allows you to perform actions andautomate processes based on changes to specific records. You can perform some actions automatically

---

## Page 98

when a new record is created, when any existing record is getting updated, or when any record isgetting deleted.
To understand the fundamentals of triggered flows, let us explore their purpose, differences from screenflows, and the benefits they provide.
The following are the purposes of record-triggered flows: Record-triggered flows are designed to automate processes and actions based on specific recordchanges or events.
They provide a visual and declarative way to build automation without writing code.
Triggered flows can streamline business processes, reduce manual effort, and enhance productivitywithin your Salesforce Organization.
Following are the differences from screen flows: While screen flows are user-driven and typically initiated by user interactions, record-triggeredflows are initiated automatically based on record changes.
Screen flows focus on guiding users through a series of screens, while record-triggered flows focuson performing actions or tasks in response to record events.
Record-triggered flows are executed in the background and can update records, create relatedrecords, send notifications, and perform various other actions without user involvement.
The following are the benefits of record-triggered flows: Automation: Record-triggered flows allow you to automate repetitive tasks and processes,reducing manual effort and increasing efficiency.
Flexibility: With record-triggered flows, you can implement complex business logic and createsophisticated automation without writing code.
User experience: By automating processes with record-triggered flows, you can provide aseamless and consistent experience for users, ensuring that tasks are completed accurately andefficiently.
Scalability: Record-triggered flows can be designed to handle large volumes of records andevents, making them suitable for organizations of any size.
Maintainability: Record-triggered flows can be easily modified and updated as businessrequirements change, providing agility and adaptability to evolving processes.
Understanding the purpose, differences, and benefits of record-triggered flows is important for utilizingtheir full potential. With the help of record-triggered flows effectively, you can automate processes,improve productivity, and create a more streamlined experience for users within your SalesforceOrganization.
Identify the need for record-triggered flows
Record-triggered flows are designed to address specific business needs and challenges related toautomating processes based on changes to records. Let us explore common scenarios where the needfor record-triggered flows arises and define the problem statement they aim to solve.
Scenario 1: Automated updates and notifications
Problem: Organizations often require automated updates of records and notifications to be triggeredwhen certain fields in any record are changed.

---

## Page 99

Solution: Record-triggered flows can be implemented to automatically update related records, notifystakeholders, or perform additional actions when specific field changes occur.
Scenario 2: Approval processes
Problem: Businesses often have approval processes in place for various operations, such as recordcreation, updates, or changes.
Solution: Record-triggered flows can be used to automate approval processes by evaluating criteriaand executing the necessary approval steps based on the record changes.
Scenario 3: Data integrity
Problem: Maintaining data integrity and enforcing data validation rules is crucial for accurate reportingand reliable data.
Solution: Record-triggered flows can help enforce data validation rules, perform field validations, andensure data integrity by executing specific actions or displaying error messages when data does notmeet the defined criteria.
Scenario 4: Workflow automation
Problem: Organizations often have complex workflows that involve multiple steps and actions based onspecific record events or changes.
Solution: You can migrate these workflows to record-triggered flows and you can automate therequirements by defining the sequence of actions, decision making processes, and related recordupdates based on the changes to specific records.
Insert record-triggered flows
Insert record-triggered flows are designed to perform actions and automate processes immediately aftera new record is created in Salesforce. By leveraging insert record-triggered flows, you can streamlineworkflows, automate tasks, and ensure data consistency from the moment a record is inserted.
Let us explore the steps to implement insert record-triggered flows effectively: 1. Define the objective: Clearly define the objective or purpose of your Insert record-triggered flow.Then, identify the specific actions or tasks that need to be performed upon record creation.2. Create a new flow: Access the Salesforce flow Builder and create a new flow specifically for theInsert record-triggered flow. Then, define the flow properties, such as name, API name,description, and any other relevant details.3. Set the flow trigger: Within the flow, set the trigger to be fired when a record is inserted. Then,specify the object and the criteria that determine when the flow should be triggered upon recordcreation.4. Design the flow logic: Design the flow's logic by adding and configuring the necessary flowelements, such as record lookups, Decision elements, actions, and screens. Then, use the flowelements to perform actions or tasks based on the newly created record.5. Configure actions and tasks: Determine the actions or tasks that need to be executed uponrecord creation. Examples of actions can include updating related records, sending notifications,creating tasks, or assigning ownership.6. Handle exceptions and errors: Implement error handling and exception management within theflow.7. Activate and test the flow: Activate the Insert record-triggered flow to make it available for use.After activating, you need to test the flow by creating new records and verifying that the desiredactions are performed as expected.

---

## Page 100

8. Monitor and optimize: Monitor the flow's performance and make any necessary optimizations orimprovements based on user feedback or changes in business requirements.
By following these steps, you can successfully implement Insert record-triggered flows in Salesforce.
Criteria for the record trigger
When implementing record-triggered flows, defining the criteria that determine when the flow should betriggered is crucial. By setting specific criteria, you can control the flow's execution and ensure that itonly runs when the desired conditions are met. Let us explore the steps to define the specifics of thetrigger criteria effectively: 1. Identify triggering conditions: 1. Determine the specific conditions or criteria that need to be met for the flow to be triggered.
2. Consider the fields, values, and relationships that should be evaluated to determine if thetrigger should be activated.
2. Access flow Builder: 1. Access the Salesforce flow Builder and locate the Insert record-triggered flow you are workingon.
2. Navigate to the element that represents the trigger or the point where the criteria will beevaluated.
3. Add Decision element: 1. Add a Decision element to the flow to evaluate the triggering conditions.
2. Configure the Decision element with the necessary criteria to determine if the flow shouldcontinue.
4. Define criteria: 1. Specify the criteria within the Decision element by setting conditions based on field values,formulas, or logical expressions.
2. Use comparison operators, logical operators (AND, OR), and functions to define the criteriaprecisely.
5. Set outcome connectors: 1. Configure the outcome connectors of the Decision element to route the flow's execution basedon the evaluation of the criteria.
2. Define the different paths or actions to be taken depending on whether the criteria are met ornot.
6. Implement actions: 1. Within each outcome connector, add the necessary actions or tasks to be executed based onthe evaluation of the criteria.
2. Actions can include updating records, sending notifications, creating tasks, or invoking othersubflows.
7. Test the trigger criteria:

---

## Page 101

1. Save and test the flow to ensure that the trigger criteria are properly evaluated and the flow'sexecution follows the desired path.
2. Create or update records that meet or do not meet the criteria and verify that the flow behavesas expected.
8. Refine and adjust criteria: 1. Continuously refine and adjust the trigger criteria as needed based on user feedback, changingbusiness requirements, or process optimizations.
By defining the specifics of the trigger criteria, you can control when record-triggered flows areactivated and ensure that they execute only when the defined conditions are met. This allows forprecise automation and streamlines processes within your Salesforce Organization.
Fast Field Updates
Fast Field Updates are a powerful feature in record-triggered flows that allow you to efficiently updatefields. With Fast Field Updates, you can perform multiple updates in a single operation, reducing thenumber of database transactions and improving performance.
Let us do hands-on for one basic business need.
Requirement: When a contact record is created without an associated Account ID, the system shouldautomatically assign an Account ID by matching the organization name with an existing Account inSalesforce.
To fulfill this requirement, we will create a Salesforce record-triggered flow. This flow will verify whetherthe Account field is empty when a new contact record is being created in Salesforce. If the Account fieldis empty, the flow will automatically assign an Account ID by searching for an existing Account with amatching organization name.
In Salesforce, when you navigate to Setup | Company Information Page, you will see your organizationname.
 
 Note: For successful implementation demo, please navigate to the Account tab in Salesforce and create a new account
record with the account name matching the organization name.
Now, follow the steps below to create a new insert record-triggered flow. We are creating this before-insert record-triggered flow because we need to update the Account ID on the contact record, which isavailable on the same record that triggers the flow.
Follow the below steps for hands-on in your Salesforce Org for practical learning: 1. Login to your Salesforce Org, and click on Setup, as shown in the following figure:

---

## Page 102

Figure 7.1: Salesforce setup option
2. Search flows in the Quick Find box, as shown:3. Click on flows, as shown in the following figure:
Figure 7.2: Setup Home
4. Click on the New flow button, as shown in the following figure:
Figure 7.3: View all flows
5. Select the Record-Triggered Flow type.6. Click on the Create button, as shown:

---

## Page 103

Figure 7.4: New flow options
7. Fill the following details: 1. In the Object, select the Contact object.
2. Trigger the flow When:
Select: A record is created
3. Define the first condition:1. Field: Department
2. Operator: is Null
3. Value: False
4. Define the first condition:1. Field: AccountId
2. Operator: is Null
3. Value: True
5. Optimize the flow for:
Select Fast Field Updates
8. Click on the Done button, as shown:

---

## Page 104

Figure 7.5: Create Record Element Detail
9. Select the Add Element option and select the Get Records component, as shown in the followingfigure:
Figure 7.6: Get Record Element
A dialog box will open, as shown in Figure 7.7.

---

## Page 105

10. Fill the following details: 1. Label: Get Account
2. API Name: Get_Account
3. In the Object, select the Account object.
4. Condition Requirements:
Select: All Conditions Are Met (AND)
5. Define the condition:1. Field: Name
2. Operator: Equals
3. Value: {!$Organization.Name}
6. How Many Records to Store:
Select: Only the first record
7. How to Store Record Data:
Select: Automatically store all fields.
11. Click on the Done button.
Figure 7.7: Get Record Element
12. Select the Add Element option and select the Update Records component, as shown in thefollowing figure:

---

## Page 106

Figure 7.8: Update Record Element
A dialog box will open, as shown in Figure 7.9.13. Fill the following details: 1. Label: Update Account Id
2. API Name: Update_Account_Id
3. How to Find Records to Update and Set Their Values:
Select: Use the contact record that triggered the flow
4. Set Field Values for the Contact Record
AccountId equals {!Get_Account.Id}
Here, AccountId is field, and {!Get_Account.Id} is value
14. Click on the Done button.15. Click on the Save button.

---

## Page 107

Figure 7.9: Update Record Element
16. Fill the following details: 1. Label: Update account on Contact
2. API Name: Update_account_on_Contact
3. Click on the Save button, as shown:
Figure 7.10: Save flow
17. Click on Activate button:

---

## Page 108

Figure 7.11: Activate flow
Now test the flow:18. Click on App Launcher: 1. In Quick Find box search Contact:
Figure 7.12: App Launcher
2. Click on Contacts:
Figure 7.13: Show all contact record
3. Click on New button.
4. Leave the Account blank and choose any value for Department.
5. Click on Save Button, as shown:

---

## Page 109

Figure 7.14: Create new record
You will notice that Account Name is auto populated:
Figure 7.15: Record details
Actions and related records

---

## Page 110

In record-triggered flows, you can leverage actions to perform additional tasks and updates on relatedrecords. Actions allow you to extend the automation beyond the initial record trigger and make updatesto associated records based on specific conditions. Let us explore the steps to implement actions andupdate related records effectively: 1. Identify related records: 1. Determine the related records that need to be updated or modified based on the conditions orcriteria in your flow.
2. These related records can be child records, parent records, or records linked through lookup ormaster-detail relationships.
2. Access flow Builder: 1. Access the Salesforce flow Builder and locate the record-triggered flow you are working on.
2. Identify the point in the flow where the related record updates need to be performed, typicallyafter a Decision element or based on certain conditions.
3. Add Action element: 1. Add an Action element to the flow at the appropriate location.
2. Configure the Action element to specify the type of action you want to perform on the relatedrecords.
4. Select Action type: 1. Choose the appropriate Action type based on your requirements. Some common action typesinclude Update Records, Delete Records, and Send Email.
2. Configure the action with the necessary details, such as the target records, field values, emailtemplates, etc.
5. Define Action criteria: 1. Set up the criteria or conditions for the action to be executed on the related records.
2. You can use Decision elements or formula-based criteria to control the flow of the action.
6. Map fields: 1. Map the fields from the Action element to the corresponding fields on the related records.
2. Ensure that the field mappings are accurate and align with the data model of the relatedrecords.
7. Test and validate: 1. Save the flow and test it by triggering the conditions that activate the action on the relatedrecords.
2. Verify that the related records are updated, created, or deleted as expected.
8. Monitor and refine: 1. Continuously monitor the flow's performance and the impact on related records.
2. Gather user feedback and refine the action criteria or configuration as necessary to ensuredesired outcomes.

---

## Page 111

By incorporating actions in your record-triggered flows, you can extend the automation to updaterelated records based on specific conditions or criteria. This allows you to maintain data consistency,trigger additional actions, and streamline complex business processes within Salesforce.
Let us do a hands-on for a use case:
When a contact's status is changed to Customer, send a welcome email with onboarding instructions: 1. Create a custom field on Contact:
Setup | Object Manager 1. Quick Find search contact.
2. Select Contact, as shown:
Figure 7.16: Search Contact in Quick Find box
3. Select Fields & Relationships.
4. Click on New button.
5. Select picklist data type:1. Field Name: Status
2. Enter values as shown in Figure 7.17 to add picklist value.
3. Values:
Customer
Partner
Figure 7.17: Create new field
6. Click on Next | Next | Save Button.

---

## Page 112

2. Create a flow following the given steps: 1. Quick Find box search flows.
2. Click on flows.
3. Click on New flow Button.
4. Select Record-Triggered Flow type.
5. Click on the Create button.
6. A dialog box will open, as shown in Figure 7.17.
3. Fill the following details: 1. In the Object, select the Contact object.
2. Trigger the flow When:
Select: A record is updated
3. Condition Requirements:
All Condition Are Met (AND)
4. Define the condition: 1. Field: Status__c
2. Operator: Equals
3. Value: Customer
4. When to Run the flow for Updated Records:
Select: Every time a record is updated and meets the conditionrequirements
5. Optimize the flow for:
Select: Actions and Related Records
6. Click on the Done button, as shown:

---

## Page 113

Figure 7.18: Get contact record
5. Create a New Resource: 1. Click on the New Resource button, as shown in the following figure:
Figure 7.19: New Resource
2. Open a new popup.
3. Select Resource Type: Text Template
4. API Name: OnboardingEmail
5. Body: Body content will be depending on requirement.
6. Click on Done button, as shown:

---

## Page 114

Figure 7.20: Create new resource
6. Select the Add Element option and select the Action component, as shown in the followingfigure:
Figure 7.21: Add element
7. Fill the following details: 1. Label: Send email to Contact

---

## Page 115

2. API Name: Send_email_to_Contact
3. Set Input Values for the Selected Action:1. Body: {!OnboardingEmail}
2. Recipient Address List: {!$Record.Email}
3. Rich-Text-Formatted Body: {!$GlobalConstant.True}
4. Sender Email Address: {!$Record.Owner.Email}
5. Subject: Onboarding
4. Click on the Done Button, as shown:
Figure 7.22: Add value in Action
8. Click on the Save button:
Figure 7.23: flow Save

---

## Page 116

1. Label: Welcome email with onboarding instructions
2. API Name: Welcome_email_with_onboarding_instructions
3. Click on Save Button, as shown:
Figure 7.24: flow name
9. Click on the Activate button. 1. Testing steps: Click on App Launcher
2. Search Contact.
3. Click on Contacts:
Figure 7.25: App launcher
10. Click on any contact Name from list of record, as demonstrated in Figure 7.26 to go to contactdetails page:

---

## Page 117

Figure 7.26: All contact record
11. Make sure a valid email is there on Contact. You can update the Email on the contact record ifthe Email is blank on Contact.12. Change the Status to Customer
Figure 7.27: Update record status
After clicking on Save, an email will automatically go to the contact’s email.
Delete record-triggered flows
Deleting record-triggered flows are designed to perform actions and automate processes immediatelyafter a record is deleted in Salesforce. By leveraging delete record-triggered flows, you can streamlineworkflows, automate tasks, and ensure data integrity when records are deleted.
Let us explore the steps to implement delete record-triggered flows effectively: 1. Define the objective: Clearly define the objective or purpose of your delete record-triggeredflow. Identify the specific actions or tasks that need to be performed upon record deletion.2. Create a new flow: 1. Access the Salesforce flow Builder and create a new flow specifically for the delete record-triggered flow.
2. Define the flow properties, such as name, API name, description, and any other relevantdetails.
3. Set the flow trigger: 1. Within the flow, set the trigger to be fired when a record is deleted.
2. Specify the object and any additional criteria that determine when the flow should be triggeredupon record deletion.

---

## Page 118

4. Design the flow logic: 1. Design the flow's logic by adding and configuring the necessary flow elements, such as recordlookups, Decision elements, actions, and screens.
2. Use the flow elements to perform actions or tasks based on the deleted record and its relatedrecords, if necessary.
5. Configure actions and tasks: 1. Determine the actions or tasks that need to be executed upon record deletion.
2. Examples of actions can include updating related records, sending notifications, creating tasks,or archiving data.
6. Handle exceptions and errors: Implement error handling and exception management within theflow to handle any potential errors or unexpected scenarios that may occur during the flow'sexecution.7. Activate and test the flow: 1. Activate the delete record-triggered flow to make it available for use.
2. Test the flow by deleting records and verifying that the desired actions are performed asexpected.
8. Monitor and optimize: Continuously monitor the flow's performance and make any necessaryoptimizations or improvements based on user feedback or changes in business requirements.
By following these steps, you can successfully implement delete record-triggered flows in Salesforce.These flows allow you to automate actions, enforce data integrity, and streamline processes whenrecords are deleted. With delete record-triggered flows, you can enhance efficiency, maintain dataconsistency, and ensure that necessary actions are taken upon record deletion within your SalesforceOrganization.
Let us implement a use case to ensure that all cases associated with a contact are automatically deletedwhenever the contact is deleted from the system.
Create a new flow with following the given steps: 1. From Setup, enter flows in the Quick Find box, then select flows.2. Click New flow.3. Make sure Start From Scratch is selected.4. Click on the Next button, as shown in Figure 7.28:
Figure 7.28:New flow
5. Select Record-Triggered Flow.

---

## Page 119

6. Click on the Create button, as shown in Figure 7.29:
Figure 7.29: Select type
7. Fill the following details: 1. Select Object as the Contact.
2. Trigger the flow When, select A record is deleted.
3. Click on the close (x) icon, as shown in Figure 7.30:
Figure 7.30: Select object and configure trigger
8. Add element: 1. On the flow canvas, on the path after the Start element, click on the Add Element (+).
2. Scroll down to the data section and click Delete Records as shown in Figure 7.31:

---

## Page 120

Figure 7.31: Add Element
The Delete Records window will open, as shown in Figure 7.32.9. Fill the details as given below: 1. Label: Delete Related Cases of Contact
2. API Name (It will be auto populated): Delete_Related_Cases_of_Contact
3. How to Find Records to Delete:1. Select Specify conditions radio button
4. Delete Records of This Object Type:1. Object: Choose Case
The object type specified here is Case, which means the flow willdelete records from the Case object that meet the specified criteria.
5. Filter Case Records:1. Condition Requirements for Records to Delete: All Conditions Are Met (AND)
This condition type ensures that all specified criteria must be metfor Case records to be deleted.
6. Conditions: (Configure the conditions using the details below. (Refer to Figure 7.32 forguidance)1. Field: ContactId
2. Operator: Equals
3. Value: {$Record.Id} (You can type Record in the text box and select Contact Id from thedropdown).

---

## Page 121

Figure 7.32: Delete records
10. Save and debug: 1. Click on the Save button.
2. For flow Label, enter Delete related Cases Contact
3. The flow API Name field will be automatically updated to Delete_related_Cases_Contact.
4. Click Save, as shown in Figure 7.33:
Figure 7.33: Save the flow
11. Activate flow: Click the Activate button to activate this flow as shown in Figure 7.34:

---

## Page 122

Figure 7.34: Activate flow
Test instructions: Verify the deletion of related cases when contact record will be deleted. Follow thegiven steps: 1. Navigate to the Contacts tab in your Salesforce Org to open a contact record (You need to goback from flow Builder).2. Select any contact record from the list (You can create a new contact and an associated case fortesting this flow).3. Verify that there are one or more cases associated with the contact.4. Note the case details (e.g., Case Number, Subject) to confirm its existence before proceeding (Youcan open an associated case record in a new tab to verify it later if this is deleted when contactrecord deleted).5. Click on the Delete button on the contact record page. Check that the contact has beensuccessfully deleted from the system. All cases that were associated with the deleted contactshould also be deleted automatically.
 
 Note: The flow assumes that there are cases associated with the contact. To prevent the flow from failing when no cases
are associated with the contact, add a condition to check for the presence of cases before the delete element.
Conclusion
In this chapter, we explored the implementation of record-triggered flows and learned how to automateprocesses and perform actions based on changes to specific records in Salesforce. We began byunderstanding the purpose and benefits of record-triggered flows, including their flexibility, scalability,and maintainability.
We delved into how to insert record-triggered flows, where we learned how to define triggers based onrecord creation and perform actions immediately after a new record is inserted. We also discussed theimportance of setting criteria to control the flow's execution and explored techniques for efficient fieldupdates using fast field updates.
Furthermore, we explored actions and their role in updating related records and performing additionaltasks based on specific conditions. We understood how actions extend the automation beyond the initialrecord trigger and enable us to maintain data consistency and streamline processes.

---

## Page 123

In addition, we covered deleting record-triggered flows, which allow us to automate actions and ensuredata integrity when records are deleted. We learned how to define triggers based on record deletionand perform tasks such as updating related records or sending notifications.
By mastering the concepts and techniques covered in this chapter, you now have the knowledge andskills to create effective record-triggered flows that automate processes, maintain data integrity, andimprove efficiency within your Salesforce Organization.
In the next chapter, Scheduling Triggered flows, we will dive into another powerful aspect of flowautomation. scheduling triggered flows allow you to automate processes at specific time intervals orbased on predetermined schedules. We will explore the capabilities of scheduling flows, setting upscheduled triggers, and designing efficient and effective scheduled automation.
Key learnings Record-triggered flows: Record-triggered flows allow you to automate processes and performactions based on changes to specific records. They provide a visual and declarative way to buildautomation without writing code.
Purpose and benefits: Record-triggered flows streamline workflows, automate tasks, andenhance productivity. They offer flexibility, scalability, and maintainability within your SalesforceOrganization.
Insert record-triggered flows: Insert record-triggered flows are triggered when new recordsare created. They allow you to perform actions immediately after record creation, automateapprovals, enforce validation rules, and ensure data accuracy.
Criteria for triggers: Defining specific criteria is essential to control when a record-triggered flowshould be executed. The criteria are based on field values, formulas, or logical expressions.
Fast Field Updates: Fast Field Updates enable you to efficiently update fields on related recordswithin a single operation. They reduce the number of database transactions and improveperformance.
Actions and related records: Actions in record-triggered flows allow you to perform additionaltasks and update related records based on specific conditions. You can update, create, or deleterelated records and send notifications to stakeholders.
Delete record-triggered flows: Delete record-triggered flows and perform actions upon recorddeletion. They enable you to automate tasks, update related records, and maintain data integritywhen records are deleted.
Flow Trigger Explorer: flow Trigger Explorer is a tool that helps manage and understand thebehavior of record-triggered flows. It provides insights into flow executions, troubleshootingcapabilities, and performance monitoring.

---

## Page 124

CHAPTER 8Scheduling Triggered flows
Introduction
In today’s fast paced world, automation is key to staying ahead. One powerful tool for Salesforceprofessionals is scheduling flows to run automatically at set times. This chapter is your hands-on guideto creating schedule-triggered flows, which allow you to automate tasks and processes with precision.
We will walk through how to build these flows step by step, helping you automate tasks like updatingrecords, sending reminders, or managing data—exactly when you need them. We will also explore real-life examples, from improving customer service in retail to streamlining operations in manufacturing,showing how scheduled flows can make a difference in various industries.
Structure
This chapter covers the following topics: Business need for the schedule-triggered flows
Configure schedule-triggered flow
Behaviors of schedule-triggered flow
Schedule-triggered flows for batches of records
Monitor schedule-triggered flows
Objectives
We will begin this chapter by examining the fundamental business needs that necessitate the use ofschedule-triggered flows. By highlighting common problem statements, we aim to help you understandwhy these automation mechanisms are essential for various industries.
Through detailed, practical guidance, we will equip you with the knowledge and skills required toconfigure schedule-triggered flows. this empowers you to tailor these flows to your specific operationalrequirements, regardless of your industry.
To master the art of schedule-triggered flows, it is crucial to comprehend how they behave underdifferent conditions and scenarios. We will explore the nuances and intricacies involved in thefunctioning of these flows to ensure seamless integration into your business processes.
For organizations dealing with large volumes of data, processing records individually can be inefficient.We will show you how to harness schedule-triggered flows to process batches of records, allowing yourautomation to scale efficiently to meet the demands of your growing operation.
Effective management of automation requires real-time visibility. This chapter guides you in establishingmonitoring and alerting mechanisms for schedule-triggered flows. By doing so, you will have the tools toensure your automated processes run smoothly and reliably.

---

## Page 125

This chapter is designed to leave you well-prepared to harness the power of schedule-triggered flows.Whether you are looking to streamline your operations, optimize your workflow, or implement industryspecific use cases, the insights and knowledge gained from this chapter will be invaluable in achievingyour automation goals.
Business need for the schedule-triggered flows
In the ever-evolving landscape of modern business, the quest for efficiency, productivity, and timely taskexecution has become increasingly paramount. To address this challenge, organizations are turning toautomation as a cornerstone of their operations. A key facet of this automation strategy is the use ofschedule-triggered flows.
Problem statement
In every industry, businesses grapple with the need to execute tasks at specific times, in response toparticular events, or at regular intervals. These tasks may vary widely, from sending automated emailreminders to customers, processing payroll on a designated date, or updating inventory levels duringnon-peak hours.
Common business needs include: Time-sensitive actions: Many business operations require actions to be taken at precise times.For instance, a financial institution might need to execute daily batch processes for fund transfersor settlements, or an e-commerce platform may need to schedule product updates.
Recurring data processing: Data-driven decisions often necessitate processing vast amounts ofinformation at regular intervals. This could include generating monthly sales reports, conductinginventory checks, or calculating monthly bills for utility services.
Customer engagement: Schedule-triggered flows are invaluable for maintaining customerrelationships. Sending out timely reminders, birthday greetings, or notifications of upcoming eventsis crucial for engagement and retention.
Optimizing resource allocation: In manufacturing and supply chain operations, schedulingtriggers can be used to optimize production schedules and resource allocation. This helps inreducing downtime and ensuring efficient use of resources.
Compliance and governance: Many industries are bound by regulations that require actions tobe taken at specific intervals. This might include archiving records, conducting safety checks, orgenerating compliance reports.
Role of schedule-triggered flows
Schedule-triggered flows come into play as a solution to address these pressing business needs. Theyallow organizations to automate these time-dependent actions with precision and reliability. By settingup scheduled flows, businesses can ensure that tasks are executed at the right time, reducing the riskof human error, and ensuring operational efficiency.
Imagine that you want to enhance your customer engagement by sending personalized birthdaygreetings to your contacts from Salesforce. Sending these greetings on time is critical to showing yourclients that you value their business and care about their special day. However, manually sending thesegreetings daily can be time consuming and prone to errors. This is one basic example where schedule-triggered flows come to the rescue.
In today's highly competitive market, fostering strong customer relationships is paramount. Sendingpersonalized birthday greetings is a simple yet effective way to show your customers that youappreciate them, ultimately increasing customer loyalty.
Schedule-triggered flows allow you to automate sending birthday greetings to your contacts. Here ishow it works:

---

## Page 126

1. Data collection: First, you will need to collect and maintain customer data, including contactdetails and birthdates, in your CRM system. This data will serve as the foundation for yourautomated birthday greeting campaign.2. Flow configuration: With schedule-triggered flows, you can configure the system to check thecontact database daily for upcoming birthdays.3. Message personalization: Your flow can be designed to pull the contact's name and otherrelevant information and generate a personalized birthday message.4. Email delivery: The schedule-triggered flow can then trigger the automated delivery of thesemessages, ensuring that they reach the recipient's inbox on their birthday.5. Error handling: By using scheduled flows, you can also set up error handling and monitoringmechanisms to ensure that messages are sent as intended. This includes managing cases where anemail address is missing or an email delivery fails.
The benefits are as follows: Efficiency and consistency: Automation ensures that every birthday greeting is sent promptlyand consistently. This not only saves time but also eliminates the possibility of human error insending greetings.
Improved customer relationships: Your customers will appreciate the thoughtfulness andpersonal touch of receiving birthday greetings. This contributes to building stronger and long-lasting customer relationships.
Time and resource savings: Automating this process reduces the manual effort required to sendgreetings daily, freeing up your team's time for more strategic tasks.
Scalability: As your contact list grows, the system can easily scale to accommodate morebirthdays without requiring additional manual effort.
This use case exemplifies the power of schedule-triggered flows in addressing specific business needs.In the following sections of this chapter, we will guide you through configuring and managing theseflows, offering practical insights for achieving automation like this and much more.
Configure schedule-triggered flow
Follow the given steps for hands-on in your Salesforce Org for sending personalized birthday greetingsto your contacts from Salesforce: 1. Login to your Salesforce Org, and click on Setup, as shown in the following figure:

---

## Page 127

Figure 8.1: Salesforce Setup
2. Search flows in the Quick Find box, as shown:3. Click on flows, as shown in the following figure:
Figure 8.2: Setup Home
4. Click on the New flow button, as shown in the Figure 8.3:
Figure 8.3: Select flows
5. Select the Schedule-Triggered Flow.6. Click on the Create button, as shown in the following figure:

---

## Page 128

Figure 8.4: New flow options
7. Fill in the following details: 1. Start Date: Specify the starting date for this scheduled flow. Indicate the date from which youintend to begin sending emails to contacts.
2. Start Time: Select a preferred time for sending birthday greetings email.
3. Frequency: Determine the operational frequency for the scheduled flow. In this case, sincewe are sending birthday greetings, selecting Daily ensures that this schedule flow functions ona daily basis.
8. Click on the Done Button, as shown in the following figure:
Figure 8.5: Date and time
9. Create a New Resource: 1. Click on New Resource button:

---

## Page 129

Figure 8.6: New resource
It will open a new popup.
2. Select resource type Formula
3. API Name: TodayDate
4. Data Type: Date
5. Formula: Today()
10. Click on the Done Button:
Figure 8.7: Create new resource
11. Select the Add Element option and select the Get Records component, as shown in the Figure8.8:

---

## Page 130

Figure 8.8: Add get records element
A dialog box will open as shown in Figure 8.9.12. Fill the following details: 1. Label: Get Contact Record
2. API Name: Get_Contact_Record
3. In the Object, select the Contact object.
4. Condition Requirements:
Select: All Conditions Are Met (AND)
5. Define the first condition:1. Field: Birthdate
2. Operator: Equals
3. Value: TodayDate
6. Define the second condition:1. Field: Email
2. Operator: is Null
3. Value: False
7. How Many Records to Store:
Select: All record
8. How to Store Record Data:
Select: Automatically store all fields

---

## Page 131

Figure 8.9: Get record element
13. Select the Add Element option and select the Loop component, as shown in the followingscreenshot:
Figure 8.10: Add Loop
A dialog box will open as shown in Figure 8.11.14. Fill the following details: 1. Label: Loop on get Contact
2. API Name: Loop_on_get_Contact
3. Collection Variable: {!Get_Contact_Record}
4. Direction: First item to last item.

---

## Page 132

15. Click on the Done button:
Figure 8.11: Loop element
16. Create a New Resource as shown in Figure 8.12: 1. Click on New Resource button.
Figure 8.12: New Resource
Open a new popup.
2. Select resource type Text.
3. API Name: Email
4. Data Type: Text
17. Click on the Done button:

---

## Page 133

Figure 8.13: Email resource 1. Click on the New Resource button
2. Open a new popup.
3. Select resource type Text.
4. API Name: ListOfEmail
5. Data Type: Text
6. Allow Multiple Value: True
18. Click on the Done button:
Figure 8.14: Variable
19. Select the Add Element option and select the Assignment component, as shown in the followingscreenshot:

---

## Page 134

Figure 8.15: Add Assignment
A dialog box will open which will be as shown in Figure 8.16.20. Fill the following details: 1. Label: Assign Email
2. API Name: Assign_Email
3. Set Variable Values:
First Condition1. Variable: Email
2. Operator: Equals
3. Value: {!Loop_on_get_Contact.Email}
Second Condition:1. Variable: ListOfEmail
2. Operator: Add
3. Value: Email
21. Click on the Done button:

---

## Page 135

Figure 8.16: Assignment element
22. Select the Add Element option and select the Decision component, as shown in Figure 8.17:
Figure 8.17: Add Decision element
23. Fill the following details: 1. Label: Check List of Email
2. API Name: Check_List_of_Email
3. OUTCOME DETAILS:1. Label: Check Email List

---

## Page 136

2. Outcome API Name: Check_Email_List
3. Condition Requirements to Execute Outcome
Select: All Condition Are Met(AND)
4. Resource: {!ListofEmail}
5. Operator: is Null
6. Value: False
24. Click on the Done button:
Figure 8.18: Decision element details
25. Select the Add Element option and select the Action component, as shown in Figure 8.19:

---

## Page 137

Figure 8.19: Add Action element
26. Fill in the following details: 1. Action: Send Email
2. Label: Send Email
3. API Name: Send_Email
4. Body: Happy Birthday
5. Recipient Address Collection: {!ListofEmail}
6. Rech-Text-Formatted Body : true
7. Subject: Happy Birthday
27. Click on the Done button:

---

## Page 138

Figure 8.20: Action element details
28. Click on the Save button and activate the flow: 1. Flow Label: Happy Birthday Send Email to Contact
2. Flow API Name: Happy_Birthday_Send_Email_to_Contact

---

## Page 139

Figure 8.21: Save flow
Behaviors of schedule-triggered flow
Schedule-triggered flows are a powerful tool for automating actions at specific times or frequencies.Understanding their behaviors under different scenarios is crucial for their successful implementation.Here, we will explore the key behaviors of schedule-triggered flows to help you navigate potentialchallenges and make the most of their capabilities: Precision in timing: Schedule-triggered flows are designed to execute tasks precisely. Theyadhere to the specified time and frequency, ensuring that actions occur at the exact moments youintend. This precision is invaluable when timeliness is critical, such as sending birthday greetings,as discussed in our earlier use case.
Reliability: These flows are known for their reliability. Once configured, they consistently performtasks as scheduled, reducing the risk of errors and ensuring the reliable execution of yourautomated processes.
Error handling: Schedule-triggered flows can be set up to handle errors gracefully. For instance,in the context of sending birthday greetings, you can implement error handling mechanisms tomanage situations where contact data is missing or email deliveries fail. This proactive errorhandling enhances the robustness of your automation.
Resource efficiency: By automating tasks with schedule-triggered flows, you can optimizeresource allocation. Instead of having staff dedicate time to manual processes, you can redirectresources to more strategic and value-added activities. This improves overall resource efficiency.
Scalability: One of the remarkable features of schedule-triggered flows is their scalability. As yourorganization grows and the volume of tasks increases, these flows can easily accommodate theadditional workload without requiring substantial changes to the configuration.
Event logging and monitoring: Schedule-triggered flows often come equipped with eventlogging and monitoring features. This enables you to keep a close eye on the performance of yourautomated processes. Monitoring tools can help identify issues or bottlenecks in the flow, allowingfor timely intervention and adjustments.
Compliance and governance: For industries that must adhere to strict regulations or compliancerequirements, schedule-triggered flows offer a way to ensure that necessary actions are takenwithin the prescribed timeframes. This supports your organization in meeting its complianceobligations.
Event queue management: In cases where there is a high volume of scheduled events, such asa large number of birthday greetings to send daily, schedule-triggered flows may interact with anevent queue. Understanding the queuing and prioritization system is important to ensure timelyand efficient execution.
Schedule-triggered flow for batches of records
While scheduling flows for individual records can be immensely beneficial, there are scenarios whereyou need to process data in larger batches. This is particularly important when dealing with highvolumes of data, making it impractical to execute actions on a record-by-record basis. In this section,we will explore how to harness the power of schedule-triggered flows to process batches of recordsefficiently.
Batch processing definition
Batch processing involves the execution of a specific task or action on a group of records, rather thanprocessing them individually. This approach is especially useful in scenarios where you have hundreds orthousands of records to process simultaneously.

---

## Page 140

Use cases
Let us take a look at the use cases: Sales order processing: In the retail industry, businesses often receive a high volume of salesorders daily. Scheduling flows to process these orders in batches can streamline the fulfillmentprocess.
Inventory management: For manufacturing and supply chain operations, periodic batchprocessing can be used to update inventory levels, ensuring real-time visibility into stock quantities.
Customer communications: Sending out newsletters, promotional emails, or announcements toa large subscriber base can be managed efficiently by scheduling flows to handle email dispatch inbatches.
Configuration for batch processing
To implement schedule-triggered flows for batch processing, you need to consider several key factors: Batch size: Determine the ideal batch size based on your system's capacity and performance. Thisdictates how many records are processed in each batch.
Frequency: Decide on the frequency at which batches are processed. For example, you mightschedule batch processing every hour or daily.
Data segmentation: Ensure that records are segmented logically. For instance, in sales orderprocessing, you may batch records by order creation date or location.
Error handling: Implement robust error handling mechanisms to manage exceptions that mayoccur during batch processing, such as incomplete records or processing failures.
Benefits of batch processing
Following are the benefits of batch processing: Efficiency: Batch processing significantly reduces the time and effort required to process largevolumes of data. It allows for the efficient use of resources, particularly in resource-intensive tasks.
Scalability: As your organization grows and data volumes increase, batch processing can scaleseamlessly, accommodating a higher workload without substantial changes to the configuration.
Consistency: It ensures uniform processing across the batch, reducing the risk of inconsistenciesand errors.
Resource optimization: By automating batch processing, you can allocate your team's resourcesto other critical tasks, contributing to resource optimization.
Performance management: Batch processing can be monitored and managed to ensure optimalperformance, which is essential for maintaining data integrity and timely execution.
In the subsequent sections of this chapter, we will provide you with practical insights and guidance onconfiguring schedule-triggered flows for batch processing. Whether you are managing large-scale dataprocessing or optimizing your operations, these principles will help you harness the power ofautomation and scheduling triggers for batch oriented tasks.
Monitor schedule-triggered flows
Effective automation does not end with the configuration and setup of schedule-triggered flows.Continuous monitoring is essential to ensure that your flows are functioning as intended and topromptly address any issues that may arise. In this section, we will explore how to monitor schedule-

---

## Page 141

triggered flows in Salesforce, enabling you to maintain the reliability and efficiency of your automatedprocesses.
Monitoring tools in Salesforce
If you have created a scheduled flow and want to ensure it is running smoothly, here are the steps tomonitor it. You will learn how to check when your flow last ran, when it is scheduled to run next, and ifthere were any issues during its execution.
Follow the steps below to ensure your scheduled flows are running properly: 1. Log into Salesforce2. Click on the gear icon (Setup)3. Type Scheduled Jobs in the Quick Find box4. Click on Scheduled Jobs (refer to Figure 8.22)
Figure 8.22: Find scheduled jobs
On this Scheduled Jobs page (refer to Figure 8.23), you will see the following: 1. Type (Type scheduled flow means that the listed job is a flow configured to run automatically atspecified times or intervals)
2. When the flow last ran
3. When it will run next
4. Option to delete the scheduled jobs
Figure 8.23: View scheduled jobs
To delete a schedule job, find your flow in the list, click the Delete button next to it, and note that thisonly removes the schedule, not the flow itself.

---

## Page 142

To restart a schedule, go to your flow, make it inactive (turn it off) as shown in Figure 8.24, and thenmake it active again (turn it on); this will reset the schedule to start fresh.
Figure 8.24: Activate/deactivate flow
Follow the steps below if you need to check for errors or if your flow has failed: 1. Go to Setup2. Search for Paused and Failed flow Interviews.
3. Click on it.4. Look for your flow in the list as shown in Figure 8.25.5. Click on the flow to see why it failed.
Figure 8.25: Paused and failed flow interviews
Debug logs provide in-depth information about how your flow is executed, helping you identify anyerrors or issues. These logs are essential for troubleshooting and gaining detailed insights into flowperformance.
You can create and check a debug log by navigating to Setup, typing Debug Logs into the Quick Findbox, and then clicking on Debug Logs.
Error handling and alerts
Schedule-triggered flows may encounter errors, such as issues with data sources, email deliveryfailures, or system unavailability. It is crucial to set up error handling and alerts to proactively managethese situations: Error logs: Maintain logs of errors encountered during flow execution. These logs should capturedetails about the error, including the affected records and the nature of the issue.
Alerts and notifications: Configure alerts and notifications to inform administrators or relevantpersonnel when errors occur. This allows for immediate action to rectify issues and preventdisruptions to automated processes.

---

## Page 143

Performance optimization
Monitoring is not solely about error detection. It also involves performance optimization to ensure thatyour flows run efficiently and in a timely manner: Performance metrics: Track key performance metrics, such as execution time, to identifypotential bottlenecks or areas for improvement. This can help you fine-tune your flows for optimalperformance.
Resource utilization: Monitor resource utilization, including CPU and memory usage, to ensurethat your automated processes do not place an undue burden on your Salesforce environment.
Scaling and capacity planning
As your organization grows, the demands on your scheduled flows may increase. Monitoring helps youplan for scalability: Capacity planning: Continuously assess whether your Salesforce environment can handle theincreasing load. This includes evaluating the need for additional resources or scaling your existinginfrastructure.
Regular reviews and audits
Schedule-triggered flows are not static. Regular reviews and audits are essential to ensure that theyremain aligned with your organization's evolving needs and objectives. Periodic audits: Conduct periodic audits to review the relevance and efficiency of your scheduledflows. This may involve updating flow logic, adding new triggers, or retiring flows that are no longerneeded.
By proactively monitoring your schedule-triggered flows in Salesforce, you can ensure that yourautomated processes operate smoothly, efficiently, and in line with your business goals. This monitoringand management are integral to maintaining a well-functioning Salesforce environment, deliveringreliability, and optimizing performance.
Conclusion
In this chapter, we explored the journey of the world of automation, and exploring the crucial conceptof scheduling triggered flows. The chapter provided a comprehensive guide on how to create schedule-triggered flows, enabling functionality at specified times and frequencies for each record in a batch. Itdelved into the versatility of these flows, catering to real-time and industry-specific use cases.
We established why schedule-triggered flows are vital by recognizing common problem statementsacross industries, emphasizing the need for automation to drive efficiency and productivity.
The chapter equipped you with the necessary knowledge and skills to configure schedule-triggeredflows, making them adaptable to your organization's unique operational requirements.
We explored the nuanced behaviors of schedule-triggered flows under varying conditions, ensuring yourautomation remains seamless and effective.
For organizations managing large volumes of data, the chapter demonstrated how schedule-triggeredflows can efficiently process batches of records, enabling scalability for your growing operation.
We highlighted the importance of real-time monitoring and guided you in setting up monitoring andalerting mechanisms for these flows, ensuring their reliability.
The insights gained from this chapter have equipped you with the knowledge and skills to leverageschedule-triggered flows effectively. Whether you are striving for streamlined operations, workflow

---

## Page 144

optimization, or industry specific use cases, the chapter has provided you with the tools to achieve yourautomation goals.
As you move forward in your journey to master automation, this chapter will serve as a foundationalstepping stone, enabling you to orchestrate tasks, streamline processes, and drive efficiency in yourorganization. The principles learned here will be instrumental in harnessing the potential of schedule-triggered flows.
In the upcoming chapter, we will delve into another aspect of automation within Salesforce, exploringplatform event-triggered flows.

---

## Page 145

CHAPTER 9Platform event-triggered Flow
Introduction
In this chapter, we will explore the powerful combination of platform events and flows in Salesforce. Youwill learn how to create platform event-triggered flows, enabling your organization to respond to real-time events and streamline business processes. We will cover the key concepts, implementation steps,and use cases for this dynamic duo, where we embark on a journey into the dynamic world of platformevents and flows in Salesforce. This chapter is your gateway to understanding and harnessing thepower of real-time event-driven automation within the Salesforce ecosystem. Platform events are arevolutionary feature, introducing a publish/subscribe model that facilitates seamless communicationbetween different components of your Salesforce environment. On the other hand, flows empower youto design powerful workflows with a user friendly visual interface. In this chapter, we will explore thesynergy between platform events and flows, specifically focusing on platform event-triggered flows. Thispowerful combination allows you to create applications that respond to real-time events, automatingprocesses and ensuring your Salesforce environment stays agile and responsive.
Structure
This chapter is organized into the following sections: Platform events overview
Platform event-triggered flow
Publish event messages with flows
Subscribe to platform event messages with flows
Business use cases for platform events and flows
Objectives
We will begin by examining the fundamental business needs that necessitate the use of schedule-triggered flows. This chapter delves into the seamless integration of platform events and flows inSalesforce, illuminating their collective potential in driving real-time automation. Through a step-by-stepapproach, we will guide you in creating platform event-triggered flows, empowering your organizationto swiftly respond to unfolding events and optimize operational efficiencies. We will navigate throughessential concepts, implementation procedures, and practical use cases, providing you with acomprehensive understanding of this dynamic duo's capabilities. By the chapter's end, you will have afirm grasp on leveraging the platform event’s publish-subscribe model and flows' intuitive designinterface to craft responsive applications tailored to your business needs. Through structuredexploration, we will uncover the symbiotic relationship between platform events and flows, spotlightingtheir role in ensuring the agility and responsiveness of your Salesforce environment. Get ready toembark on a journey into the realm of real-time event-driven automation, where the fusion of platformevents and flows propels your organization towards heightened productivity and innovation.

---

## Page 146

Platform events overview
Platform events are a way to send and receive real-time event messages in Salesforce. These eventmessages represent changes or occurrences within the platform or can even be triggered by externalsystems integrated with Salesforce. They offer a means of communication between different parts ofyour Salesforce environment or with external applications.
Its key concepts and features are as follows: Publish-subscribe model: Platform events follow a publish-subscribe pattern, allowing one partof the system (the publisher) to send event messages, which can be consumed by any interestedparties (subscribers). This decouples different components, promoting modularity andresponsiveness.
Loose coupling: Platform events foster loose coupling, meaning changes in one part of thesystem do not tightly affect other parts. This promotes flexibility and maintainability in yourapplication architecture.
Event schema: Each platform event has a defined schema, specifying the structure of the eventmessage. This ensures consistency in event data and facilitates understanding among subscribers.
Event delivery: Salesforce ensures reliable delivery of platform events with built-in persistenceand replay capabilities. Even if a subscriber fails to process an event, it can catch up when it is backonline.
Event triggers: Platform events can trigger specific actions. Subscribers can define event triggersto specify what should happen when a particular event occurs. This might include running customApex code, updating records, or invoking external integrations.
Streaming API: Platform events are used in conjunction with the Streaming API, a mechanism forreal-time communication between Salesforce and external systems. Subscribers can use theStreaming API to listen for and receive platform events.
Scalability and performance: Platform events are highly scalable, making them suitable forlarge enterprise level applications. Salesforce handles the underlying infrastructure, ensuring robustperformance and reliability.
Security and permissions: Access to platform events is controlled by Salesforce's robust securitymodel. Administrators can define who can publish, subscribe to, and trigger events, safeguardingdata privacy and security.
Use cases
Platform events are versatile and find applications in various scenarios, including: Process automation: Automate business processes based on real-time events.
Monitoring and alerting: Set up real-time notifications for critical events.
Integration: Connect with external systems and services.
Real-time reporting and dashboards: Create dynamic dashboards and analytics.
Internet of Things (IoT) integration: Communicate with IoT devices.
Custom applications: Build real-time, responsive applications.
Platform event-triggered flow
A platform event-triggered flow is a workflow automation that gets activated when a specific platformevent is received in Salesforce. It harnesses the capabilities of both platform events and flow to create adynamic, event-driven system. When a platform event message is published, the associated platformevent-triggered flow can respond to the event and execute predefined actions.

---

## Page 147

Its key components and implementation are listed as follows: Platform event definition: Before creating a platform event-triggered flow, you must have aplatform event defined in your Salesforce Org. The platform event defines the structure of theevent message, including the data fields it contains.
Flow Builder: Platform event-triggered flows are built using the flow Builder in Salesforce. Theflow Builder provides a user-friendly interface to design the flow's logic and actions.
Flow elements: Within the flow Builder, you can use various flow elements to design yourplatform event-triggered flow. Common flow elements include: Platform event: To specify the platform event you want to trigger the flow.
Conditions: To define when the flow should be executed based on event data.
Record updates: To update records in response to the event.
Email alerts: To send email notifications.
Assignment: To assign values to variables and fields.
Activation: Once your platform event-triggered flow is designed, you must activate it to make itoperational. You can set it to run automatically in response to the platform event or trigger itmanually.
Event publishers: Platform events are published by various processes, which can include Apexcode, external integrations, or other flows. The flow is triggered when the relevant platform eventis published.
Testing and monitoring: It is essential to thoroughly test your platform event-triggered flow toensure it responds correctly to incoming events. You can monitor its performance and makeadjustments as needed.
Use cases
Platform event-triggered flows can be applied to a variety of use cases, such as: Real-time notifications: Instantly notify users or systems about critical events.
Automated record updates: Update records based on incoming event data.
Integration: Trigger external system actions in response to platform events.
Dynamic approval processes: Streamline multi-step approval workflows.
IoT data processing: React to data from IoT devices.
Platform event-triggered flows are a versatile tool for making your Salesforce processes and applicationsmore responsive, automated, and efficient. They enable organizations to stay agile and take immediateaction in response to real-time events.
In the following sections, we will walk through the steps to create and configure platform event-triggered flows, providing practical insights and examples to help you implement this powerful feature inyour Salesforce environment.
Publish event messages with flows
In Salesforce, you have the capability to publish event messages using flows, allowing you to triggerreal-time events known as platform events. This section explores how to create flows that generate andpublish event messages, enabling you to communicate important changes and updates efficiently.
Before you can publish event messages with flows, it is essential to grasp the underlying process andcomponents involved:

---

## Page 148

Platform event definition: To publish an event message, you must have a platform eventdefined in your Salesforce Org. This event includes a schema that specifies the structure of theevent message, including the data fields it can contain.
Flow Builder: flows are designed and created using the flow Builder in Salesforce. The flowBuilder provides an intuitive visual interface for building workflows and automation.
Designing the flow: Within the flow Builder, design your flow to collect the necessary data thatyou want to include in the event message. This can involve user input through screen elements,querying records to extract information, or any other data collection process.
Create Records element: To create a new record as part of the flow, you will add a CreateRecords element to the flow canvas. In this case, you will create a record of the platform eventobject.
Mapping fields: In the configuration of the Create Records element, map the fields from your flowvariables or other data sources to the corresponding fields in the platform event schema. Thisensures that the data collected in the flow is included in the event message.
Activation: After designing and configuring your flow, activate it to make it ready for execution.
Publishing the event message: Event messages are typically published when certain conditionsare met. These conditions can vary, but they often involve specific events or triggers within yourSalesforce environment. The flow can be triggered manually, automatically, or as part of a largerprocess.
Publishing event messages with flows can be applied to various real-world use cases, such as: Notifying users or systems about specific events.
Integrating with external systems or services.
Automating data enrichment or validation processes.
Managing inventory and stock levels in real-time.
Supporting appointment and scheduling systems.
Flows provide a flexible and user-friendly way to generate and publish event messages, enabling yourorganization to maintain real-time communication and automation, ultimately improving responsivenessand efficiency.
Subscribe to platform event messages with flows
Subscribing to platform event messages with flows in Salesforce is a powerful method to automateresponses to real-time events, creating dynamic and responsive applications. In this section, we willexplore the process of setting up flows to subscribe to platform event messages and take actions basedon the incoming event data.
Before diving into the implementation, it is important to understand the core components and conceptsassociated with subscribing to platform event messages with flows: Platform event definition: To subscribe to platform event messages, you must have a platformevent defined in your Salesforce Org. This event includes a schema that defines the structure of theevent message and specifies the data fields it contains.
Flow Builder: The flow Builder in Salesforce is the tool you will use to create flows that subscribeto platform event messages. It provides a visual, user-friendly interface for designing workflowautomation.
Designing the flow: Within the flow Builder, design your flow to specify the actions you want totake in response to the incoming platform event message. This can include tasks such as updatingrecords, sending emails, or executing custom logic.

---

## Page 149

Platform Event element: To subscribe to the platform event message, you will add a PlatformEvent element to your flow canvas. This element is specifically designed for subscribing to events.
Configuring the Platform Event element: In the configuration of the Platform Event element,select the platform event that you want to subscribe to. You can specify conditions for when theflow should be triggered based on event data.
Activation: Once your flow is designed, you must activate it to make it operational. You can set itto run automatically when the relevant platform event is published or trigger it manually.
Event publishers: Platform events are typically published by various processes, which can includeApex code, external integrations, other flows, or even external systems integrated with Salesforce.the flow is triggered when the specified platform event is published.
Subscribing to platform event messages with flows can be applied to a variety of real-world use cases,including: Real-time notifications for critical events.
Integration with external systems or services.
Data enrichment and validation in real-time.
Inventory and stock management.
IoT device integration.
The following are some of the best practices and considerations for subscribing to platform events: When subscribing to platform event messages, ensure that your flow handles event data gracefullyand efficiently, especially if you expect a high volume of events.
Regularly monitor your flow's performance and test it under various conditions to validate itsreliability.
Be mindful of the potential impact of event-triggered flows on your organization's limits, such asdaily limits and governor limits.
Business use cases for platform events and flows
Platform events and flows in Salesforce offer a dynamic and versatile combination for automatingprocesses, enabling real-time communication, and streamlining operations. In this section, we willexplore various business use cases that leverage platform events and flows to enhance efficiency,responsiveness, and decision making within your organization: Real-time notifications and alerts: Use case: When a high-priority support case is created, a platform event triggers a flow thatnotifies the support team in real-time.
Benefits: Timely responses to critical customer issues, enhancing customer satisfaction.
Integration with external systems: Use case: An external e-commerce platform sends order updates via platform events. Asubscribing flow updates Salesforce records in response to these events.
Benefits: Seamless data synchronization between Salesforce and external systems, reducingmanual data entry.
Automated process automation:

---

## Page 150

Use case: Platform events trigger flows to automate multi-step approval processes forpurchase requests.
Benefits: Efficient and error-free approval workflows, reducing processing time.
Data enrichment and validation: Use case: When a new lead is created, a platform event triggers a flow that queries externaldata sources and updates the lead record with additional information.
Benefits: Improved data accuracy and enriched customer profiles.
Inventory and stock management: Use case: Platform events are published when inventory levels fall below a threshold.Subscribing flows generate purchase orders and notify suppliers in real-time.
Benefits: Prevent stockouts, optimize inventory levels, and improve supply chain efficiency.
Appointment and scheduling systems: Use case: An appointment scheduling system uses platform events to trigger flows that checkappointment availability and schedule appointments.
Benefits: Real-time scheduling and efficient appointment management.
IoT integration: Use case: IoT devices send data via platform events. Flows subscribe to these events, triggeralerts, and take actions based on device data.
Benefits: Real-time insights into IoT device status and proactive issue resolution.
Customer support and case management: Use case: Platform events notify support agents when high-priority cases are created.Subscribing flows assign cases, send notifications, and track response times.
Benefits: Rapid response to critical support issues and improved case resolution times.
Complex approval workflows: Use case: Platform events trigger flows to manage multi-step approval processes for complexprojects or purchases.
Benefits: Streamlined and efficient approval workflows, ensuring compliance and governance.
Employee onboarding and offboarding: Use case: Platform events notify HR systems when new employees are hired or whenemployees leave the company. Flows automate the onboarding and offboarding processes.
Benefits: Streamlined and error-free employee lifecycle management.
Real-time analytics and dashboards: Use case: Platform events update real-time dashboards and analytics based on incomingevents. Flows ensure that data is up-to-the-minute, providing insights for faster decisionmaking.
Benefits: Accurate and current data for informed business decisions.
These business use cases illustrate the versatility of platform events and flows in enhancing businessprocesses, automating workflows, and improving overall productivity. The combination of real-timeevent-driven communication and automation empowers organizations to adapt to changing conditionsand provide exceptional customer experiences.

---

## Page 151

Let us delve into the practical implementation of these use cases, providing examples and step-by-stepinstructions to help you apply platform events and flows effectively in your specific business scenarios.
In this practical scenario, we will create a platform event-triggered flow to automatically log errorsencountered during flow execution using the flow Execution Error Event. When errors occur, thisstandard platform event will trigger the creation of an error log record in a custom object named errorlog. This log will contain details about the error, making it easier to understand its cause and facilitatingprompt resolution. This setup ensures efficient error tracking and troubleshooting within the Salesforceplatform.
 
 Note: A fault path is recommended for error handling in screen flows; however, we are omitting it for the demonstration
of the platform event-triggered flow.
To implement this, we will first set up a custom object and a custom field to store the error details. Twoflows will be developed: one that generates an error during execution and another that publishes theplatform event to log the error.
Our goal is to design a screen flow within Salesforce to facilitate the creation of an account. If anyerrors arise during the execution of this flow, they will be captured and stored in the error log customobject.
Now, we will proceed with the practical implementation through the following hands-on steps: 1. Log in to your Salesforce Org and create the necessary custom objects and fields as a prerequisitefor this implementation.Create a custom object Error Log: Go to SetupSelect Object ManagerClick Create and then select Custom ObjectLabel: Error Log
Plural Label: Error Logs
Object Name: Error_Log (auto populate)Record Name: Error Log Name (auto populate)Data Type: Text (auto populate)Search Status: Allow Search
Object Creation Options (Available only when the custom object is firstcreated) Checked on the Add Notes and Attachments related list to default pagelayoutChecked on the Launch New Custom Tab Wizard after saving this customobject
Click Save (refer to Figure 9.1)

---

## Page 152

Figure 9.1: Create custom object
2. Create custom fields for object Error Log:Click on the Field & Relationships tab in the left menu, then click New. As shown in Figure 9.2 create Field Error_Details__c with the following details: Field Type: Long Text AreaField Label: Error Details
Length: 32,768 charactersField Name: Error_Details (auto populate)Visible Lines: 3
Label: Error Details (refer to Figure 9.2)
Figure 9.2: Create custom field
3. Go to Setup, search flows in the Quick Find box, click on flows, and click on New flow. Makesure Start from Scratch is selected.

---

## Page 153

4. Click the Next button and create Platform Event—Triggered Flow (refer to Figure 9.3).
Figure 9.3: Create new flow (platform event-triggered flow)
5. Click on the Create button.6. Select Platform Event as flow Execution Error Event(it is a standard platform event) (refer to Figure9.4).
Figure 9.4: Select standard platform event
7. Select the Add Element option and select the Create Records element, (refer to Figure 9.5).
Figure 9.5: Add create records element
8. Fill the following details: (refer to Figure 9.6):

---

## Page 154

1. Label: Create Error Log
2. API Name: Create_Error_Log
Note: The API Name will auto-populate.
3. How to set record field values: Manually
4. Create a Record of This Object as shown:
 
 Object
 
 Field
 
 Value
  
Error_Log  
  
Error_Details__c  
  
  {!$Record.ErrorMessa
      
Name  
  
  {!$Record.FlowApiNam
Table 9.1: Field and Value for Create Record Element
Figure 9.6: Create error log record
9. Save the flow with the following details and click on the Save button as shown in Figure 9.7: 1. Label: Create Error Log
2. API Name: Create_Error_Log

---

## Page 155

Figure 9.7: Save the flow
10. Activate the flow: Create another flow to create an account using a Screen flow. (refer toFigure 9.8). You can refer to any existing flow as well, which might throw an error duringexecution.
Figure 9.8: Create new screen flow(account creation)
11. Select the Add Element option and select the Screen element. (refer to Figure 9.9).
Figure 9.9: Add element

---

## Page 156

12. Add two components on the screen and fill in the following details: 1. Component: Text
2. Label: Account Name
3. API Name: Account_Name
 
 Note: The API Name will auto-populate.
Please refer to Figure 9.10:
Figure 9.10: Add text component
4. Component: PickList
5. Label: Industry
6. API Name: Industry
 
 Note: The API Name will auto-populate.
7. Create a new resource for picklist choice
8. Resource Type: Picklist Choice Set (generate a set of choices by using the values of a picklist ormulti-select picklist field) (refer to Figure 9.11).
Figure 9.11: Create a new resource for picklist choice

---

## Page 157

13. Fill in the following details as shown in Figure 9.12 for creating the choices for the Industry field: 1. Resource Type: Picklist Choice Set
2. API Name: Industry
 
 Note: The API Name will auto-populate.
3. Object: Account
4. Data Type: Picklist
5. Field: Industry
Figure 9.12: New resource fields
14. You will have a final screen, as shown below in Figure 9.13:
Figure 9.13: Screen after adding components
15. Click Done.

---

## Page 158

16. Select the Add Element option, select the Create Records element, and fill in the followingdetails (refer to Figure 9.14): 1. Label: Create Account
2. API Name: Create_Account
 
 Note: The API Name will auto-populate.
3. How to set record field values: Manually
4. Create a Record of This Object
 
 Object
 
 Field
 
 Value
  
  Account
  
  Account Name
  
  Account_Name
      
  Industry
  
  Industry
Table 9.2: Field and Value for Create Record Element
Figure 9.14: Create new record
17. Add a new screen element to show a success message when the record is created successfully(refer to Figure 9.15).

---

## Page 159

Figure 9.15: Screen with success message
The final flow implementation will look like Figure 9.16:
Figure 9.16: Simple screen flow
18. Save the flow with the following details and click on the Save button (refer to Figure 9.17): 1. Label: Create Account
2. API Name: Create_Account

---

## Page 160

Figure 9.17: Save the flow
19. Activate the flow: Add the Account Create screen flow to any record page layout or the homepage for demonstration purposes, then save and activate the page (see Figure 9.18).
Figure 9.18: Add flow on page
Select Industry from the picklist and leave the Account Name field empty, as shown in Figure 9.19.
 
 Note: The Account Name is a mandatory field on the account object; however, we are intentionally omitting it to
generate an error for this demonstration. Therefore, it is not marked as required in the flow screens.
Figure 9.19: Create an account using a screen flow

---

## Page 161

Click the Next button, and an error will be displayed (see Figure 9.20):
Figure 9.20: An error occurred
As mentioned earlier, if an error occurs, a record will be created in the Error Log object by the platformevent-triggered flow we set up before creating the screen flow. You can check the error log bynavigating to the object. Figure 9.21 shows the created error log.
 
 Note: While a fault path is typically advisable for error handling in screen flows, it has been intentionally excluded in this
demonstration of the platform event-triggered flow.
Figure 9.21: A record is created on error log object
Conclusion
This chapter has been a journey into the dynamic synergy of platform events and flows in Salesforce.From understanding the fundamentals to exploring real-world use cases, we have witnessed the powerof real-time event-driven automation.
As you reflect on the key concepts presented in this chapter, you will be equipped with the knowledgeto create responsive applications, automate processes, and elevate the efficiency of your Salesforceenvironment.

---

## Page 162

In the next chapter, we will delve into autolaunching flows, further expanding your capabilities tostreamline processes and enhance user experiences within the Salesforce platform.
Stay tuned for the next chapter as we continue to navigate the world of Salesforce automation.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 163

CHAPTER 10Autolaunched Flows
Introduction
Welcome to the chapter Autolaunched flows—an innovative way to automate tasks effortlessly withinSalesforce. This chapter is your guide to understanding what autolaunched flows are, how they work,and the many ways you can use them to streamline your processes.
In essence, autolaunched flows are like behind-the-scenes choreographers for your Salesforce tasks.They kick into action without needing users to click buttons or make decisions. Unlike other types offlows, they do not involve screens or local actions, focusing instead on smooth, background operationsusing Lightning components.
In this journey through autolaunched flows, you will encounter familiar types like schedule-triggeredflows, record-triggered flows, platform event-triggered flows, and versatile subflows. Schedule-triggeredflows stick to a set schedule, doing their work without bothering users with screens or local actions.Record-triggered flows react when records are created, updated, or deleted. Platform event-triggeredflows thrive on real-time data, responding to events as they happen. Subflows, acting like flowsidekicks, can be both autolaunched and screen flows, triggered by other flows or orchestrations.
However, there is more to autolaunched flows. We will explore a unique category—autolaunched flowswithout triggers. These silent performers start with custom buttons, links, Apex classes, REST APIs, andother behind-the-scenes triggers, quietly shaping processes without user interfaces stealing thespotlight. Even the versatile subflow finds its place in this mysterious subset of autolaunched flows.
As we journey through the upcoming chapters, we will dive deep into the world of autolaunched flows,discovering their practical applications and giving you the tools to make the most of this automatedorchestration in your Salesforce experience. Let us unlock the full potential of autolaunched flowstogether!
Structure
This chapter is organized into the following sections: Business requirements for autolaunched flow
Creating autolaunched flow
Calling autolaunched flow from record-triggered flow
Calling autolaunched flow from Apex
Calling autolaunched flow from the REST API
Autolaunched flow versus record-triggered flows
Objectives

---

## Page 164

This chapter will explain why autolaunched flows are so crucial in everyday business situations. Bylooking at common challenges, we will show you why autolaunched flows are the go-to solution. Then,we will get our hands dirty and guide you step-by-step in creating these flows. We will also share thebest ways to design autolaunched flows that work well and grow with your business.
The chapter will explore how autolaunched flows can be called from another flow, making automationeven more powerful. We will guide you on using code (Apex) to trigger autolaunched flows and howmixing the tech with the simpler, point-and-click side can be a game changer.
We will take autolaunched flows beyond Salesforce. You will see how they can play well with othersystems using the REST API, opening up possibilities for even more connections. Lastly, we will compareautolaunched flows with another Salesforce tool, record-triggered flows. Think of it as helping youchoose the right tool for the job.
By the end of this chapter, you will not just understand autolaunched flows – you will know how to usethem effectively. Whether you are looking to solve business problems, make work smoother, or handlespecific tasks in your unique industry, this chapter will give you the know-how to make autolaunchedflows your Salesforce superheroes.
Business requirements for autolaunched flow
In this section, we will start a journey to dissect the business requirements that underscore theadoption of autolaunched flows. Understanding these fundamental needs is paramount as we lay thegroundwork for the effective utilization of this automation tool within the Salesforce ecosystem.
Addressing key use cases involves the following: Streamlining multi-flow operations: Autolaunched flows shine in scenarios where standardizedautomated steps are necessary across various workflows. The demand for building and maintainingthese steps only once resonates with businesses aiming for process efficiency and consistency.
User initiated seamless actions: Businesses benefit from autolaunched flows when users caneffortlessly trigger complex actions with a single click. Behind the scenes, records are manipulated,and additional tasks like email notifications or task creation are seamlessly executed, reducingmanual intervention.
Dynamic responses to platform events: Autolaunched flows prove their worth in respondingdynamically to platform events. Whether it involves creating or updating records, sending emailnotifications, or executing predefined tasks, this feature enhances real-time responsiveness inSalesforce environments.
Efficient user deactivation cleanup: In user management, especially during deactivation,autolaunched flows efficiently handle cleanup tasks. This includes removing users from queues andpublic groups and managing permission sets and licenses, ensuring accuracy in user management.
The challenges would involve manual overhead and process consistency, as detailed: Manual overhead in repetitive tasks: A recurring challenge faced by businesses is the manualoverhead in executing repetitive tasks across workflows. Autolaunched flows offer a solution byautomating these tasks, reducing manual effort, and ensuring consistency in process execution.
Adaptability in dynamic environments: Businesses operate in dynamic environments, andstatic solutions often fall short in adapting to evolving requirements. Autolaunched flows providethe required flexibility to modify and extend automation strategies as business needs change overtime.
Ensuring compliance and accuracy: Stricter compliance standards in certain industries pose arisk to manual processes. Autolaunched flows can be configured to enforce compliance, minimizingthe risk of regulatory issues and ensuring adherence to industry standards.

---

## Page 165

Efficient user management: Particularly in scenarios of user deactivation, businesses face thechallenge of efficiently managing user memberships across various entities. Autolaunched flowsprovide a systematic approach to address this, ensuring accuracy in user management.
The guidelines for success are as follows: Strategic pre-construction analysis: Before delving into the construction of autolaunchedflows, a strategic pre-construction analysis is essential. This involves understanding requirements,sketching out workflows, and validating processes with key stakeholders.
Paper-based planning for clarity: Utilize paper-based planning to sketch out the process map,providing a clear visualization of the workflow before entering Salesforce setup. This paper-basedapproach simplifies logic validation and facilitates more efficient adjustments.
Consideration of user decision points: Given the automation of manual steps, carefulconsideration of user decision points is vital. Delve into scenarios, thinking about the actions userswould take, forming the basis for constructing the logic within the autolaunched flows.
As we progress through this chapter, we will delve deeper into these business requirements, providingpractical insights and examples to empower you in harnessing the full potential of autolaunched flows inyour Salesforce environment. Stay tuned for a comprehensive exploration of this powerful automationtool.
Creating autolaunched flow
Let us look into the practical aspects of creating autolaunched flows to automate the dynamic updatingof related records within Salesforce. The hands-on scenario focuses on streamlining the customerengagement process and sales pipeline management by automatically updating related contact recordswhen the account is updated.
Scenario overview
To better understand the practical application, let us explore the scenario: Automate the update of the Other Phone field for associated Contacts within the Account, ensuringthat if this field is blank on the Contact, it is synchronized with the corresponding Phone field onthe Account.
This flow aims to enhance customer engagement and streamline sales pipeline management byeliminating the need for manual record updating.
The hands-on steps are as follows: 1. Logging into your Salesforce Org: 1. Open your web browser and navigate to your Salesforce Org.
2. Log in with your credentials.
2. Accessing setup: 1. Once logged in, locate and click on the Setup option.
The following steps will guide you through the practical implementation of the scenario: 1. Click on Setup, as shown in Figure 10.1:

---

## Page 166

Figure 10.1: Salesforce Setup option
2. Search flows in the Quick Find box, as shown in Figure 10.2, and click on flows:
Figure 10.2: Setup home
3. Click on the New flow button, as shown in Figure 10.3:
Figure 10.3: View all flows
4. Select the Autolaunched flow (No Trigger) as shown in Figure 10.4:

---

## Page 167

Figure 10.4: New flow options
5. Click on the Create button.6. Create New Resource variable: 1. Click on New Resource button as shown in Figure 10.5:
Figure 10.5: New Resource
2. Resource Type: Variable as shown in Figure 10.6:

---

## Page 168

Figure 10.6: New Resource options
7. Fill the following details as shown in Figure 10.7: 1. Resource Type: Variable
2. API Name: accountRecord
3. Data Type: Record
4. Object: Account
5. Availability Outside the flow: Available for input (Checkbox is checked)
Figure 10.7: New Resource details
8. Click on the Done button.
 
 Note: In this example above, we have created the resource Data Type Record for object Account that will
hold full Account record using the accountRecord variable. However, depending on your specific use case,
you can create the variable recordId of Text Data Type.
Both approaches have their advantages:

---

## Page 169

Holding the full record is useful when you need to access multiple fields directly within theflow.Creating the recordId to hold ID can be more efficient when you only need the record's IDwithin the flow.
To create the recordId variable resource within the flow, follow the given steps: 1. Create a variable called recordId of type Text.
2. When invoking this subflow from another flow or component, ensure you pass the recordId asan input variable to the flow.
3. Within the flow, use the recordId to fetch the corresponding Account record as needed.
Consider your scenario and choose the approach that best fits your needs.9. Select the Add Element option and select the Update Records component as shown in Figure10.8:
Figure 10.8: Add element
10. Fill the following details as shown in Figure 10.9: 1. New Update Records:
Label: Update Contact's Other Phone
2. API Name: Update_Contact_s_Other_Phone
(Note: API Name will come automatically)
3. Description: (optional but always great to have it)
4. How to Find Records to Update and Set Their Values:
Specify conditions to identify records, and set fields individually(choose option)
5. Update Records of This Object Type: Contact
6. Filter Contact Records:

---

## Page 170

Condition Requirements to Update Records: All conditions Are Met(AND)
 
 Field
 
 Operator
 
 Value
  
  AccountId
  
  Equals
  
  accountRecord.Id
  
  OtherPhone
  
  Is Null
  
  $GlobalConstant.True
Table 10.1: Field and value for condition
 
 Note: Account ID has not been assigned yet, that we will be assigned later.
 Set Field Values for the Contact Records:
 
 Field
 
 Value
  
OtherPhone  
  
  accountRecord.Phone
Table 10.2: Field and value assignment
Figure 10.9: Related contact record updation (other phone field if blank)

---

## Page 171

11. Save the flow with the following details as shown in Figure 10.10: 1. Flow Label: Update Contact’s Other Phone
2. Flow API Name: Update_Contact’s_Other_Phone
Figure 10.10: Save the flow
12. Activate the flow by clicking on the Active button as shown in Figure 10.11:
Figure 10.11: Activate the flow
Calling autolaunched flow from record-triggered flow
In Salesforce, record-triggered flows automate business processes triggered by record changes. A keyfeature is the ability to call an autolaunched flow, promoting a modular approach to automation andenhancing reusability across different processes.
Integrating autolaunched flows into your record-triggered flows offers a declarative and user-friendlyway to handle complex logic and interactions without extensive Apex code.

---

## Page 172

Now, let us explore the steps to call the autolaunched flow we just created in the previous hands-onsection: 1. Create record-trigger flow to call above created autolaunched flow named UpdateContact’s Other Phone. 1. Select the record-triggered flow type and click on the Create button as shown in Figure10.12:
Figure 10.12: New flow (Record- Triggered flow)
2. Fill the following details as shown in Figure 10.13: 1. Select Object:
Object: Account
2. Configure Trigger:
Trigger the flow When: A record is updated
3. Set Entry Conditions:
Condition Requirements: All Conditions Are Met
 
 Field
 
 Operator
 
 Value
  
  Phone
  
  isChanged
  
  $GlobalConstant.True
4. When to Run the flow for Updated Record:
Every time a record is updated and meets the conditionrequirements
5. Select Actions and Related Records

---

## Page 173

Figure 10.13: Autolaunched flow start (entry form)
3. Select the Add Element option and select the Subflow component, as shown in the as shown inFigure 10.14:
Figure 10.14: Add subflow
4. Select Update Contact’s Other Phone flow from the list.5. Click on the Done button as shown in Figure 10.15:

---

## Page 174

Figure 10.15: Referenced flow
6. Fill the following details as shown in Figure 10.16: 1. Label: Update Contact
2. API Name: Update_Contact
3. Description:
Optional
4. Referenced flow:
Update Contact’s Other Phone
5. Include: Enabled
6. Set Input Values:
accountRecord: $Record

---

## Page 175

Figure 10.16: Subflow (fill details)
7. Save the flow with the following details as shown in Figure 10.17: 1. Flow Label: Update Contact : After
2. Flow API Name: Update_Contact_After
Figure 10.17: Save the flow
8. Click on the Save button.9. Activate the flow as shown in Figure 10.18:

---

## Page 176

Figure 10.18: Activate the flow
Follow the steps below for testing the above flow with test records: 1. Create a test account: 1. Navigate to the Accounts tab in Salesforce.
2. Click New to create a new account.
2. Enter required details: 1. Account Name: Test flow Account (Give your preferred Name)
2. Phone: 1234567890
3. Click Save.4. Create a Related Contact: 1. Open the newly created Account Record.
2. Go to the Related tab.
3. Scroll down to the Contacts section and click New Contact.
5. Enter required details: 1. First Name: Test
2. Last Name: Person
3. Other Phone: Leave this field empty
6. Click Save.7. Verify initial setup: 1. Open the Account Record and confirm the Phone field shows the value 1234567890.
2. Open the Related Contact and ensure the Other Phone field is empty.
8. Update the account phone: 1. Go to the Accounts tab and open the test account, you just created Test flow Account.
2. Click Edit and change the Phone field to a new value (for example, 5555544444).
9. Click Save.10. Verify contact update: 1. Return to the Related tab on the Account Record.
2. Open the Related Contact, you created above as name Test Person.
3. Verify that the Other Phone field now has the updated phone number from the Account(e.g., 5555544444).
Calling autolaunched flow from Apex

---

## Page 177

In the previous section, we discussed calling the Update_Contact_s_Other_Phone autolaunchedflow from the process builder. Now, let us explore how to trigger this flow from Apex code.
Invoking the autolaunched flow
To execute the Update_Contact_s_Other_Phone flow from Apex, we can utilize the flow.Interview
class. The sample code below demonstrates how to create a map of parameters and initiate the flow:
Figure 10.19: Invoke the flow from Apex
Let us take a look at the explanation of the code: Parameter map creation: A map named parameter is created to store the input parametersrequired by the flow. In this example, the flow expects an accountId parameter.
Account query: We query the database to retrieve an account with a non-null phone number. Thequery result is stored in the lstAccount list.
Flow invocation: If an account with a valid phone number is found, we proceed to populate theparameters and initiate the flow interview. The start() method is called to execute the flow.
The adjustments and considerations are as follows: Query criteria: Ensure that the account query criteria align with your specific requirements.
Error handling: Implement appropriate error handling mechanisms to handle scenarios where theflow execution may fail.
Flow design: The success of this approach depends on the design of the autolaunched flow andits ability to handle incoming parameters.
By incorporating this Apex code into your Salesforce implementation, you can seamlessly integrate theexecution of autolaunched flows, automating processes and enhancing the efficiency of your Salesforceapplication.
Verifying the updated phone on contact

---

## Page 178

After initiating the flow interview, you can verify the updated phone number on a contact recordassociated with the specified account. To do this, go to the contact record in Salesforce and inspect thephone field to confirm the changes.
Calling autolaunched flow from the REST API
In addition to invoking autolaunched flows from Apex, Salesforce provides the flexibility to trigger flowsthrough the REST API. This capability allows external systems or applications to integrate seamlesslywith Salesforce processes. In this section, we will explore the steps involved in calling an autolaunchedflow using the REST API: 1. Obtain flow URL: Before making a REST API call, you need to obtain the URL of theautolaunched flow. This URL is unique to each flow and can be obtained from the flow definition inSalesforce. 1. Navigate to flow Builder: In your Salesforce environment, go to the App Launcher andsearch for flow Builder. Click on flow Builder to open the flow Builder interface.
2. find the autolaunched flow: In flow Builder, locate the autolaunched flowUpdate_Contact_s_Other_Phone. You can find your existing flows listed in the flow Builderinterface.
3. Access flow details: Click on the autolaunched flow to open its details.
4. Retrieve the flow URL: In the flow details, look for the Details tab or a section thatprovides information about the flow, including its URL.
5. Copy the flow URL: Copy the entire URL. It usually looks like this:https://yourinstance.salesforce.com/flow/Update_Contact_s_Other_Phone.
By following these steps, you will successfully obtain the URL for our existingautolaunched flow, which you are going for making API calls.
2. Prepare request payload: Create a JSON payload that includes any necessary input parametersfor the flow. These parameters should match the expected inputs defined in the flow. In thisexample, the account parameter is used:
Figure 10.20: Sample JSON
3. Make REST API call: Use your preferred tool or programming language to make a POST request tothe flow URL with the prepared JSON payload. Ensure that you include the necessaryauthentication headers in the request.
An example using curl is as follows:

---

## Page 179

Figure 10.21: Rest API call
4. Verify execution: After making the REST API call, verify the execution of the autolaunched flowby checking the Salesforce platform or logs. Monitor the intended records to confirm that the flowhas been executed successfully.
Some tips and considerations are as follows: Authentication: Ensure that the REST API request includes the necessary authentication, typicallythrough OAuth 2.0 or other Salesforce-supported authentication methods.
Input parameters: Double check that the input parameters in the JSON payload match theexpected inputs of the autolaunched flow.
Error handling: Implement robust error handling mechanisms to handle any issues that may ariseduring the REST API call.
By following these steps, you can seamlessly integrate autolaunched flows into your externalapplications or systems, extending the reach of your Salesforce processes beyond the platform.
Autolaunched flow vs record triggered flows
As we have explored already, Salesforce provides a powerful automation toolkit, including two distincttypes of flows: autolaunched flows and record-triggered flows. Each type serves different purposes andexcels in specific scenarios. In this section, we will explore the characteristics and use cases of bothautolaunched flows and record-triggered flows.
Autolaunched flows
Autolaunched flows are designed to be initiated manually or through external processes, such as Apexcode or the REST API. These flows are typically started by a user or an external system and are notdirectly tied to specific record changes.
The key characteristics are as follows: Manual initiation: Autolaunched flows are initiated explicitly by users or external systems,making them ideal for scenarios where human intervention or external events trigger a process.
External system integration: They can be easily integrated into external applications or systemsusing APIs, allowing for seamless communication between Salesforce and other platforms.
Independence from record changes: Autolaunched flows do not depend on record changesand are not tied to specific objects. This independence makes them versatile for a wide range ofuse cases.
The common use cases are as follows: Integration with external systems: Autolaunched flows are suitable for integrating Salesforceprocesses with external applications, allowing for coordinated workflows.
Bulk record updates: When you need to perform updates on a large set of records without beingdependent on record changes, autolaunched flows provide an efficient solution.

---

## Page 180

Record-triggered flows
Record-triggered flows are designed to respond automatically to changes in records. They are initiatedby specific events, such as record creation, modification, or deletion.
Their key characteristics are as follows: Event-driven: Record-triggered flows are triggered by events related to records, such as thecreation or updating of records, providing a way to automate processes based on data changes.
Tied to specific objects: These flows are closely associated with specific objects and respond tochanges in the records of those objects. They are excellent for scenarios where actions are directlytied to data modifications.
Implicit execution: Record-triggered flows execute automatically when the defined event occurs,eliminating the need for manual initiation.
The common use cases are as follows: Field updates: When you need to update fields on a record based on changes in other fields orrelated records, record-triggered flows provide a declarative way to implement such logic.
Automated processes on record changes: For scenarios where business logic needs to beexecuted automatically in response to record changes, such as sending notifications or creatingrelated records.
Integrating autolaunched flows with record-triggered flows
In certain scenarios, you may find the need to call an autolaunched flow from within a record-triggeredflow. This integration allows you to leverage the strengths of both flow types. For example, you mighthave a complex business process triggered by a record change, and within that process, you may wantto initiate a specific user-driven interaction or external system integration using an autolaunched flow.
Consider a situation where a record update triggers a record-triggered flow. As part of this flow, youmay call an autolaunched flow to interact with an external system or involve user input for specificdecision making steps.
Choosing between autolaunched flows and record-triggered flows requires the following considerations: Nature of trigger: Consider whether the process is triggered explicitly by external systems orusers (autolaunched flow) or automatically in response to record changes (record-triggered flow).
Integration requirements: If integration with external systems is a key requirement,autolaunched flows are more suitable. For processes tightly linked to record changes, record-triggered flows are preferable.
Complexity of logic: Record-triggered flows may be preferred for complex logic that depends onreal-time data changes, while autolaunched flows offer more flexibility for diverse use cases.
By understanding the distinctions between autolaunched flows and record-triggered flows, and theirpotential integration, you can choose the most appropriate tool for your specific automation needswithin the Salesforce platform.
Conclusion
In this chapter, we explored autolaunched flows and their important role in automating businessprocesses without requiring user input. We started by identifying the key business needs that makeautolaunched flows essential, ensuring your automation strategies align with your organization’s goals.
You learned how to create autolaunched flows, giving you the skills to improve efficiency and streamlineoperations. We discussed different ways to call these flows, including using record-triggered flows,

---

## Page 181

Apex, and the REST API. This flexibility allows you to integrate autolaunched flows smoothly into yourexisting Salesforce setup.
We also compared autolaunched flows with record-triggered flows, explaining their unique features andwhen to use each one. This comparison helps you decide which type of flow is best for yourorganization’s needs.
By the end of this chapter, you have gained valuable knowledge and practical skills to use autolaunchedflows effectively. Whether you want to automate routine tasks, improve data handling, or enhanceoverall efficiency, the insights you have learned here will help you reach your automation goals.
As we conclude this chapter, we look ahead to Chapter 11, where we will embark on a journey intorecord-triggered orchestration. Next chapter is a comprehensive guide to creating multi-step and multi-user processes triggered when a record is created or updated. We will explore the intricacies of flowOrchestration, covering topics such as orchestrations overview, types of flow Orchestration,orchestration anatomy, and a deep dive into the orchestration run.
Get ready to expand your automation toolkit and elevate your Salesforce processes to new heights. Thenext chapter is your roadmap to mastering flow Orchestration, and by the end, you'll be equipped withthe knowledge to architect complex, yet streamlined, processes within the Salesforce platform.

---

## Page 182

CHAPTER 11Record-triggered Orchestration
Introduction
In Salesforce, automation is essential for simplifying and streamlining business processes. One powerfultool that enhances automation is record-triggered orchestration, which allows you to trigger andmanage complex workflows when actions are performed on records. This chapter explores howorchestrations can help automate multi-step processes, ensuring everything happens in the right order.
Whether you are a Salesforce administrator, developer, or user, record-triggered orchestration offers asolution for optimizing workflows and improving productivity. We will walk you through whatorchestration is, explain how it works, and demonstrate why it is valuable within the Salesforceecosystem. As we dive deeper, you will gain a clear understanding of the different types oforchestrations and the key components that make them effective.
You will also discover the differences between flow Builder and flow Orchestration, learning when to useeach to meet your specific needs. Finally, we will explain how orchestrations run in real-world scenarios,giving you the knowledge to design and implement efficient, automated workflows for your businessprocesses.
Whether you are new to Salesforce or an experienced professional, this chapter will provide you withpractical insights into using record-triggered orchestration to build smoother, more efficient workflowsthat align with your organizational goals.
Structure
This chapter is organized into the following sections: Orchestrations overview
Types of flow Orchestration
Orchestration anatomy
Difference between flow Builder and flow Orchestration
Orchestration run
Hands-on example with record-triggered orchestration
Objectives
This chapter is designed for Salesforce administrators, developers, and users to gain a solidunderstanding of record-triggered orchestration. By the end, you will know how orchestration canimprove workflows and automate key processes in Salesforce.
We will start by building a strong foundation, helping you understand the different types of floworchestration and how to choose the right one for your needs. You will learn how the key componentsof orchestration work together to ensure smooth and efficient processes in Salesforce.

---

## Page 183

Next, we will compare Salesforce flow Builder and flow Orchestration, highlighting their unique featuresso you can confidently decide which tool is best suited for your automation tasks.
Additionally, we will explore the orchestration run process in Salesforce, providing insights to help youtroubleshoot, optimize, and implement workflows successfully. Real-world examples and use cases willshow how record-triggered orchestration can be applied in various scenarios.
By the end of this chapter, you will have the knowledge and confidence to design and implementautomated workflows that meet your organization’s needs, making your Salesforce projects moreefficient and successful.
Orchestrations overview
Orchestrations in Salesforce flow help automate complex business processes by coordinating multipletasks and actions across different teams or users. Think of it like managing a project where every taskhas to be done in a specific order to achieve the desired outcome. Salesforce flow Orchestrator ensuresthat each step is executed at the right time and by the right person, without confusion or delays.
Salesforce flow Orchestrator enables you to connect and manage multiple flows, creating a seamlessprocess that allows tasks to flow efficiently, even when they involve various teams or approvals. Insteadof handling each task individually, orchestrator brings everything together in a well-structured andautomated manner.
The key components of flow Orchestration are: Stages: Represent different phases in a process, each containing multiple steps.
Steps: Individual actions or tasks that are carried out within a stage. These steps can beperformed in a specific sequence or simultaneously, depending on the requirements. Each step canbe: A background step which runs automatically.
An interactive step where a user or group must complete an action.
A Mulesoft step for integrating external processes.
Orchestrations start when a record is created or updated in Salesforce, automatically triggering theseries of steps. Tasks can be assigned to specific users or groups, and notifications are sent to ensuretimely action. This keeps everyone involved and ensures that processes are completed efficiently.
Types of flow Orchestration
Salesforce flow offers two primary types of orchestrations: autolaunched orchestration and record-triggered orchestration. Each type has its own unique features, triggering methods, and use cases, asshown in Figure 11.1.

---

## Page 184

Figure 11.1: Types of flow Orchestration
Autolaunched orchestration
Autolaunched orchestrations are triggered automatically but are not tied to specific record changes.They can be initiated through different mechanisms like Apex code, REST API calls, or scheduledprocesses. These orchestrations are perfect when you need flexibility in how and when your flows arestarted.
For example, you could start an autolaunched orchestration with a custom button in the UI, a scheduledjob, or an external system that triggers it via a REST API call. The flexibility makes autolaunchedorchestrations ideal for tasks that do not rely on specific records but still need to be automated ortriggered programmatically.
Record-triggered orchestration
Record-triggered orchestrations are initiated when specific record events occur, such as when a record iscreated or updated. This type of orchestration is perfect for automating processes that depend onchanges in Salesforce records.
For instance, you might have a record-triggered orchestration that sends a confirmation email everytime a new customer record is added. The orchestration automatically responds to record changes,ensuring that your workflow is executed in response to specific events in Salesforce.
In summary, here is how autolaunched and record-triggered orchestrations differ: Record-triggered: Automatically starts when a record is created or updated. Ideal for processestied to changes in Salesforce data.
Autolaunched: Can be triggered manually or programmatically using Apex, API calls, or othermethods. Provides more flexibility and is not tied to specific records.
Orchestration anatomy
In Salesforce flow, the anatomy of record-triggered orchestration consists of various elements,connectors, stages, and resources working together to create seamless workflows. Let us break downthe key components that make up this dynamic orchestration in the following figure:

---

## Page 185

Figure 11.21: Anatomy of an orchestration
As shown in Figure 11.2: Elements—Actions in harmony (1): Each element in the orchestration represents a specificaction the flow can perform. These actions contribute to the overall workflow, similar to musicalnotes in a composition. Orchestrations use specialized stage and Decision elements, enablingadministrators and developers to design the flow's performance with precision.
Connectors—Pathways of progression (2): Connectors define the routes the orchestration cantake during execution. Just like transitions between musical movements, connectors guide the flowthrough different stages and steps, ensuring a logical and coherent progression.
Stages and steps—The choreography (3): Stages serve as the foundational structure of theorchestration, with each stage comprising one or more steps. Steps represent individual actionsexecuted in sequence, much like dance steps in a choreographed routine. Together, stages andsteps create a well-organized and coordinated flow.
Resources—Values in concert (4): Resources represent values that can be referencedthroughout the stages, steps, or decisions. Similar to musical motifs that repeat, resources provideconsistency and coherence, allowing dynamic referencing of values as the orchestration unfolds.
As administrators and developers integrate these elements, connectors, stages, and resources, theycreate orchestrations tailored to their Salesforce workflows. The analogy of orchestration as a musicalcomposition highlights how these components harmonize to produce a seamless flow.
In the following sections, we will explore practical applications, use cases, and best practices,empowering you to leverage record-triggered orchestration as a powerful tool for creating customizedworkflows within the Salesforce ecosystem.

---

## Page 186

Difference between flow Builder and flow Orchestration
Flow Builder and flow Orchestration are both essential features within Salesforce, but they serve distinctpurposes. Understanding their differences is crucial for creating efficient, user-centric workflows inSalesforce processes. Let us explore these differences.
Flow Builder
Flow Builder is a user friendly, point-and-click tool for creating flows that automate various businessprocesses. Here are its key characteristics: Purpose: flow Builder is designed to create individual flows, which automate tasks within theSalesforce Organization or external systems.
Record-centric: flows created in flow Builder are inherently record-centric. While they can interactwith multiple objects, they are not tied to any specific object, providing versatility in processautomation.
Visual interface: The tool features a visual interface that guides users through the designprocess, making it easy to collect and manipulate data. Flow Builder also allows for the inclusion ofscreens, enhancing user interaction.
Flow Orchestration
In contrast, flow Orchestration focuses on managing complex business processes by coordinatingmultiple flows. Here are its key features: User-centric: flow Orchestration is inherently user-centric, allowing administrators to manageprocesses that involve different users and organizational segments through a single orchestration.
Coordination of flows: It serves as a framework for orchestrating a series of flows, providing aholistic view of operations. This enables streamlined coordination and improved efficiency.
Monitoring and control: flow Orchestration not only unifies flows but also offers tools formonitoring operations, fostering greater visibility and control over processes.
In summary, while flow Builder is the tool for creating individual flows, flow Orchestration acts as theconductor, unifying and managing multiple flows to create a comprehensive and streamlinedperformance. The following sections will discuss practical applications and scenarios for effectivelyleveraging both flow Builder and flow Orchestration within the Salesforce ecosystem.
Orchestration run
An orchestration run is created for each instance of an orchestration, which is an application built byyour admin that utilizes stages, steps, and decisions to organize complex business processes. Eachorchestration run represents a running instance of an orchestration, with its context dependent on theorchestration type. You can also specify a context using the How to Run the Orchestration advancedoption.
The orchestration run lifecycle is described as follows: 1. Initiation and triggering: The orchestration run commences with a triggering event, such as thecreation of a specific record or another predefined condition. This initiation sets the orchestrationinto active motion.2. Flow coordination: As the orchestration run progresses, it skillfully coordinates multiple flowswithin the orchestrated sequence. Each flow contributes its unique role, seamlessly integrating intothe overall performance.

---

## Page 187

3. Real-time monitoring: Real-time monitoring capabilities empower administrators to track theprogress of each flow. This visibility fosters a proactive approach, allowing for quick interventions ifany issues arise during the orchestration run.4. Error handling and resilience: Sophisticated error handling mechanisms come into play duringthe orchestration run, ensuring resilience in the face of unexpected challenges. These mechanismsmaintain the robustness of the orchestration, minimizing disruptions.
Running context of an orchestration
The running context defines the access an orchestration has to Salesforce data and determines how itresumes if paused, with the default context being the Automated Process User in system context. ForAPI version 60.0 and later, both autolaunched and record-triggered orchestrations launch and resume inthis system context. In earlier API versions, the context can vary depending on how the orchestration isinitiated and what triggers its resumption.
Hands-on example with record-triggered orchestration
Now that you understand the concept, it is time to roll up your sleeves and dive into a practicalexample! In this section, we will create a record-triggered orchestration designed to streamlineworkflows in Salesforce. Orchestration flows allow us to implement multi-step processes, triggeringvarious actions based on user input, system events, or other defined criteria.
Use case
We want to guide the user through an interactive process to capture additional information for allaccount types. The account's rating will automatically update to Hot if the account type is Prospectafter the user completes the process. Follow the given steps: 1. Create a screen flow: Design a screen flow that displays a custom message or set of instructionsfor the user.2. Create an autolaunched flow: Develop an autolaunched flow that automatically updates theaccount's rating field to Hot if the account type is Prospect. This flow will execute after the userinteraction is complete.3. Set up a record-triggered orchestration: Use flow Orchestration to coordinate the entireprocess. This orchestration will trigger when any account record is created or updated. It will firstlaunch the screen flow to guide the user through the interactive process. After the user completesthis process, the orchestration will automatically invoke the autolaunched flow to update theaccount's rating to Hot if the account type is set to Prospect.
Create a screen flow
Follow these steps to create a screen flow: 1. Log into your Salesforce Org, then go to Setup, enter flows in the Quick Find box, select flows,click New flow, choose Start from Scratch, and click Next. (Refer to Figure 11.3)

---

## Page 188

Figure 11.3: New flow
2. Select Screen flow.3. Click Create. (Refer to Figure 11.4)
Figure 11.4: Select flow type
4. To display the first screen on the flow canvas, click Add Element on the path after the Startelement. (Refer to Figure 11.5)
Figure 11.5: Add element
5. Select Screen. (Refer to Figure 11.6)6. Set the Label to First Screen.7. Drag a Display Text field from the Input section into the screen. (Give an API Name)8. Add a message such as, This account is classified as a 'Prospect.' The system will automatically update the
'Rating' to 'Hot' to indicate its strong potential for business growth.
9. Click Done.

---

## Page 189

Note: In this example, we are using simple screens with messages, but you should enhance these
screens by adding action items such as input fields, buttons, or conditional logic to guide the user
through more complex interactions.
Figure 11.6: New Screen
10. After the first screen, add another screen for confirmation, click Add Element again and selectScreen.11. Set the Label to Confirmation.12. Drag a Display Text field from the Input section into the screen. (Give an API Name)13. Add a message such as, Thank you!
14. Click Done.
Save and activate your screen flow. (Flow Label: Prospect Account Help Step).
Click Back to exit the flow canvas and return to the main flows page.
Create an autolaunched flow
Follow the given steps: 1. Click New flow, choose Start from Scratch, and click Next.2. Select Autolaunched flow (No Trigger).3. Click Create. (Refer to Figure 11.7)

---

## Page 190

Figure 11.7: Select type
4. First, create a new Resource Type: Variable
5. Name it recordId, set the data type to Text, and make it available for input. (Refer to Figure 11.8)
Figure 11.8: New resource
6. Add an Update element to update the Account rating.7. On the flow canvas, after the Start element, hover over Add Element and click it.8. Select Update Records. (Refer to Figure 11.9)

---

## Page 191

Figure 11.9: Add element
9. Fill in the following details as shown in Figure 11.10: 1. Name the element Update Account Rating. The API Name will be automatically generated(for example, Update_Account_Rating).
2. Choose the option Specify conditions to identify records and set fields individually.
10. Select the Account Object and set the following conditions for Field and Value as shown in Figure11.10: 1. Id Equals recordId (the variable you created)
2. Type Equals Prospect
11. Set the Field Value for the Account record: 1. Set Rating to Hot.

---

## Page 192

Figure 11.10: Update record
12. Save and Activate your autolaunched flow. (Flow Label: Update Account)13. Click Back to exit the flow canvas and return to the main flows page.
Create a record-triggered orchestration
Follow the given steps: 1. Click New flow, choose Start from Scratch, and click Next.2. Choose Record-Triggered Orchestration flow and click Create. (Refer to Figure 11.11)
Figure 11.11: Select type
3. Fill in the following details as shown in Figure 11.12: 1. Select Object as the Account.
2. To trigger the flow, select A record is created or updated.
3. Set Entry Conditions to None.

---

## Page 193

4. Click Done.
Figure 11.12: Configure start
4. Add a background Stage to the orchestration as shown in Figure 11.13.5. Add element Stage to include a new stage in the orchestration.
Figure 11.13: Add element
6. Label: Name this stage (for example, Initial) (Refer to Figure 11.14).7. API Name: Initial
8. Select When to Complete the Stage: 1. Condition: When all steps have been marked Completed, the stage is marked Completed

---

## Page 194

Figure 11.14: Stage
9. Add an interactive step: 1. Click Add Step, choose Interactive Step, (Refer to Figure 11.15)
Figure 11.15: Add step
10. Label the step Guided Screen The API Name will auto-populate as Guided_Screen
11. Select When to Start the Step: 1. Condition: When the stage starts, the step starts
12. Select an Action to Run: Prospect Account Help Step (the screen flow you created). Refer to Figure11.16:

---

## Page 195

Figure 11.16: Step
13. Choose the User or Group to display the step to. (Refer to Figure 11.17)14. Select the Triggering Account's ID to Related Record ID.15. Select When to Complete the Step: When the assigned user has completed the screen flow, the step is marked
Completed
Figure 11.17: Step setup
16. Click Add Step again and choose Background Step to add a Background Step. (Refer toFigure 11.18)17. Label this step (for example, Update Rating). The API Name will auto-populate as Update_Rating.18. Select When to Start the Step: When another step is marked Completed, the step starts
19. Choose the Step Name: Guided Screen
20. Select Action: Update Account (the autolaunched flow you created).21. Select the Triggering Account ID to assign to recordId under Set Input Values for theSelected Action22. Select Who to Run the Action As: 1. User Type: Automated Process User

---

## Page 196

Figure 11.18: Background step
23. Save the orchestration with the label: Prospect Engagement Rating Automation.24. Activate the orchestration flow. (Refer to Figure 11.19)25. Click Back to exit the flow canvas.
Figure 11.19: Orchestration flow
26. Add the orchestration to the Account page: 1. Open any Account record page from Account tab, click the Settings icon (upper-rightcorner), and select Edit Page as shown in Figure 11.20:

---

## Page 197

Figure 11.20: Account record
2. In the Lightning App Builder, search for flow Orchestration Work Guide and drag itonto the canvas, as shown in Figure 11.21:
Figure 11.21: Lightning App Builder
27. Save the changes.28. Manage the activation of the account record page if prompted.29. Click the Back icon button to return to the previous screen.
Testing of the use case
Follow the given steps: 1. Create a new Account with the following values: 1. Name: Enter any name (e.g., Demo Account as an example)
2. Type: Prospect
2. Click Save: You will be redirected to the Account details page.3. Check the Work Guide section. Your screen flow will display your custom message, as shown inFigure 11.22:

---

## Page 198

Figure 11.22: Account details
4. Click Next to follow your screen flow steps as shown in Figure 11.23:
Figure 11.23: Work guide
5. Click Finish as shown in Figure 11.24 and refresh the page.
Figure 11.24: Work guide 2nd screen
6. You will see that the Account Rating has been updated to Hot.
This is just the beginning of a very simple hands-on! By implementing this flow Orchestration, you havetaken the first step toward creating a more interactive and guided experience for your users. But do notstop here—there is much more to discover!
Figure 11.25 illustrates the Decision and Condition stages within the flow Orchestration process,showcasing how these elements interact to guide user actions and automate workflows based on

---

## Page 199

specific criteria:
Figure 11.25: Orchestration flow
The following details highlight how to effectively utilize these features within your orchestration: Explore Decision elements in orchestration: Add decision points in your orchestration to routeusers down different paths based on criteria like account type, user input, or other businessconditions. This allows for more tailored and dynamic processes.
Configure conditional stages: Set up stages and steps that only execute under certainconditions. For example, you can trigger different actions for accounts with varying ratings orautomatically skip steps based on previous inputs.
Leverage parallel processes: Take advantage of running multiple flows in parallel within anorchestration. You can guide users through different processes simultaneously or chain stepstogether to optimize workflows.
Enhance automation with background steps: Automate even more of your business processesby adding background steps that perform actions like record updates, email alerts, or task creationwithout user intervention, all within your orchestration.
Conclusion
In conclusion, this chapter has provided an in-depth exploration of record-triggered orchestration withinSalesforce. You have progressed from grasping fundamental concepts to unravelling the intricacies oforchestration types and their anatomy, equipping yourself with valuable insights to orchestrateworkflows effectively.
As you reflect on this chapter, remember that orchestration is more than just a workflow automator; it isa powerful tool for enhancing efficiency and fostering collaboration within Salesforce processes.Whether you are a seasoned professional or a newcomer, the knowledge you have gained here lays astrong foundation for mastering Salesforce automation.
Your orchestration journey is just beginning, and the expertise you have acquired will be invaluable asyou navigate Salesforce’s dynamic landscape. This chapter marks not an end but a significant milestonein your ongoing adventure of mastering Salesforce automation.
Looking ahead, the next chapter will dive into the integration of Apex and Lightning Web Components,revealing advanced dimensions of automation and customization.

---

## Page 200

1 (Image credit: https://help.salesforce.com/s/articleView?id=platform.orchestrator_concepts_orchestration_anatomy.htm&type=5)
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 201

CHAPTER 12Apex Actions and Lightning Web Components
Introduction
In this chapter, we are exploring Apex actions and Lightning Web Components (LWC), which playan important role in enhancing the functionality and performance of your Salesforce flows. These toolsempower developers to create powerful and efficient solutions within the Salesforce ecosystem. First off,we will tackle Apex actions. It is essentially a way for developers to add special powers to flows. We willstart with the basics of Apex, which is the language flows and Salesforce speak when they want to dosomething special. We will explore the invocable methods, which are shortcuts that make it easy forflows to talk to Apex. We will see how they help flows and Apex work together seamlessly.
Next, we will learn about executing Apex actions. They can be thought of as custom moves that helpflows tackle tough challenges and connect with other systems. It is all about making Salesforce doexactly what you need.
We will also be exploring LWC, which are special web tools that can be part of your flows. They makethings look pretty and work smoothly.
Lastly, we will discover how to put flows right inside your custom LWC. It is like combining yourfavourite tools to create something amazing.
Structure
This chapter is organized into the following sections: Create your custom action
Basics of Apex
Invocable method annotation
Execute Apex actions
Using a custom Lightning Web Component
Embed a flow in the custom Lightning Web Component
Objectives
In this chapter, we will explore how to create and use custom Apex actions. We will guide you throughthe basics of Apex programming, making it easy to understand even if you are new to coding.
Discover the power of the @InvocableMethod annotation and learn how it can enhance your automationcapabilities. You will learn to execute Apex actions inflows, ensuring your automation processes are bothsmooth and efficient.
This chapter will also teach you how to integrate custom LWSs into your Salesforce flows. See how toseamlessly embed flows within these components, creating a user-friendly interface that combines thebest of both worlds.

---

## Page 202

By the end of this chapter, you will not only grasp the fundamentals of Apex actions and LWCs but alsogain the skills to apply them in real-world scenarios. So, let us get started and make the most out ofSalesforce automation.
Create your custom action
As learnt in the previous chapters, Salesforce flows offer a fantastic way to automate businessprocesses visually and without coding, making them popular among admins and developers. However,there are situations where flows may not cover every need. In such cases, we turn to the flexibility ofApex classes. By passing data from Salesforce flow to an invocable Apex class, we can perform complextasks like data manipulation. The processed information is then returned to the flow, allowing it tocontinue smoothly based on the refined output from the Apex class.
Imagine you have a task, but there is no readymade tool in flow for it. This is where creating yourcustom Apex action comes in handy. A custom Apex action is your special tool created using Apexprogramming language. This tool acts like a superpower for your flow, enabling developers to handlemore complex logic, integrate with external systems, and perform actions not available throughstandard flow elements. As demonstrated in Figure 12.1, you can call the Apex action from flow.
Figure 12.1: Apex action
Custom Apex actions add extra power to your Salesforce toolkit, letting developers bring in personalizedlogic using Apex code. Let us look at some real-world situations where custom Apex actions really shine: Tackling tricky business logic: Solving complex business challenges that regular tools likeProcess Builder or flow cannot handle. With custom Apex actions, you can weave advanced logicseamlessly into your automated processes.
Connecting to external systems: Making Salesforce talk to other systems or online servicesoften requires special handling. Custom Apex actions act as the communication link, helpingtransform and validate data as it moves between Salesforce and the outside world.
Cleaning up and transforming data: Sometimes data needs a little makeover. Custom Apexactions are your data stylists, making sure everything is tidy and ready for action.
Crafting your own validation rules: When standard validation rules is not enough, custom Apexactions steps in. They allow you to define and enforce more complex validation rules, tailored to

---

## Page 203

your unique needs.
Smart decision making: When your process has a bunch of choices and conditions, custom Apexactions play the role of decision making wizards. They help your process make smart decisions andsmoothly move forward.
Working across different objects: Custom Apex actions make it possible to create custom logicthat spans across related records, offering a more complete solution.
Handling big batches of data: When you have a ton of records to process, custom Apex actionscan be used. They are designed to efficiently handle large sets of data, making bulk dataoperations a breeze.
Updating records dynamically: Custom Apex actions can change records on the fly based oncertain conditions. They update records dynamically as your process unfolds.
Personalized email magic: Crafting emails with a personal touch or adding special attachmentsis easy with custom Apex actions. They help you create custom email content or attachmentsbefore hitting the send button.
Custom error handling tricks: Custom Apex actions deal with errors in a way that suits yourneeds. They catch specific errors, keep a record, and take action based on what went wrong.
Custom Apex actions can be used to solve unique challenges. In short, a custom Apex action goesbeyond what standard flow elements can do. Combining an invocable Apex class with Salesforce flowmakes the solution even more powerful. To understand this combination, consider the following: Flows: flow can be explained as a recipe with steps (elements) to follow.
Custom Apex action: Sometimes, the recipe lacks specific ingredients, so you create your ownspecial ingredient (Apex action).
Programming language (Apex): Apex, as a programming language, enables you to developcustom functionality. It is like providing clear instructions that help your flow effectively utilize thespecialized features you have developed.
The invocable method or Apex class is introduced to overcome specific flow limits. Some of these limitsinclude: Salesforce Object Query Language (SOQL) query limits: Capped at 100, similar to a singletransaction in asynchronous apex. Users are limited to using a maximum of 100 data elements forretrieving information.
Data manipulation language (DML) statement limits: A maximum of 150 DML statementscan be issued, including subflows. Note that this limit applies to data elements modifying records,with the count multiplying if within a loop.
Records retrieved by SOQL queries: Limited to 50,000, ensuring efficient data querying.
Maximum CPU time on Salesforce servers: Allocated at 10,000 milliseconds, equivalent to 10seconds. CPU time represents the duration servers use to process a given solution.
Duplicate updates in one batch: In a single batch, a maximum of 12 duplicate updates isallowed for the same record, managing the frequency of updates within a batch process.
Map<Key, Value>: Not supported in Salesforce flow, limiting flexibility in associating a particularaccount ID with the number of contacts or opportunities.
Date operation: Operations like adding days, adding years, or converting dates are not supportedin Salesforce flow.
The integration of Salesforce flow with custom Apex actions open new possibilities and addresseslimitations in standard flow elements. In the upcoming sections, we will look at the basics of Apex and

---

## Page 204

how to implement InvocableMethods to enhance your Salesforce flows.
Basics of Apex
Salesforce flows are fantastic for visually automating business processes, but they sometimes havelimitations. This is where the role of Apex actions comes in. Now, let us look at Apex language, a toolkitfor creating custom actions in Salesforce.
Apex is a powerful, object oriented programming (OOPs) language designed specifically for theSalesforce platform. It acts as a tool to customize and enhance Salesforce, making it work perfectly foreach business. Some key features of the Apex language are as follows: Syntax: It is similar to Java and acts like a database stored procedure.
Execution: It happens on the server, known as the Lightning Platform.
Object oriented: It follows OOPs concepts, allowing you to work with classes, interfaces, andinheritance.
Integration: It works closely with Salesforce's API, enabling communication with other systemsand services.
Developers write Apex code using tools like the Salesforce Developer Console or Visual Studio Code.Once written, the code becomes a set of instructions waiting to be triggered.
Let us start with a straightforward Hello World example. In Apex, we utilize the System.debug() statementfor logging. In this Apex class, there is a method that prints the sentence Welcome to Apex World! in thedebug log. This serves as your initial exposure to Apex classes and methods:
public class Welcome {
    public static void sayHello() {
        System.debug('Welcome to Apex World!');
    }
Variables
In Apex, variables store and manipulate data. Unlike some other languages, Apex is strongly typed,meaning the data type of a variable needs to be declared.
Let us illustrate this with an example where we assign values to two variables and print the debug log:
String firstName = 'Om, ';
String lastName = 'Prakash';
System.debug(firstName + ‘  ‘ +lastName);
In this snippet, we declare two variables, firstName and lastName, both of type String, and concatenate thembefore printing the result in the debug log.
Conditions: If-else
In Apex, conditional statements empower you to make decisions in your code based on specificconditions. Let us look at an example:
Integer firstNumber = 10;
if (firstNumber > 0) {
    System.debug('The number is positive');
} else if (firstNumber < 0) {
    System.debug('The number is negative');

---

## Page 205

} else {
    System.debug('The number is zero');
}
In this code snippet, we declare a variable firstNumber and use conditional statements to check whether itis positive, negative, or zero. The corresponding message is then printed in the debug log.
Loops
Loops in Apex provide a mechanism to repeat a block of code. Let us explore this concept with anexample of a for loop:
for (Integer loopCounter = 0; loopCounter < 10; loopCounter++) {
    System.debug('Count: ' + loopCounter);
}
In this snippet, we use a for loop to iterate from 0 to 9. During each iteration, the code within the loopprints the current count in the debug log. This illustrates how loops efficiently execute a set of instructionsrepeatedly.
Lists, sets, and maps: Collections
In Apex, collections play a crucial role in managing groups of data efficiently.
List:
List<String> techClouds = new List<String>{'Sales Cloud', 'Service Cloud', 'Experience Cloud'};
System.debug('Tech Clouds: ' + techClouds);
Set:
Set<String> uniqueProductNames = new Set<String>();
uniqueProductNames.add('Laptop');
uniqueProductNames.add('Phone');
uniqueProductNames.add('Tablet');
System.debug('Unique Product Names: ' + uniqueProductNames);
Map:
Map<String, Integer> employeePerformance = new Map<String, Integer>();
employeePerformance.put('Satya', 90);
employeePerformance.put('Ved', 85);
System.debug('Employee Performance: ' + employeePerformance);
In these examples, we have used different types of collections: List: Illustrates a list of Salesforce related terms, such as different cloud offerings. In this snippet,we declare a techClouds list, containing values like Sales Cloud, Service Cloud, and Experience Cloud. The debug
log then displays those elements.
Set: Demonstrates a set, ensuring unique entries, in this case, product names. Here, we initialize a
uniqueProductNames set and add various product names to it. The debug log exhibits the unique productnames, highlighting the set’s ability to eliminate duplicates.
Map: Depicts a map, associating employee names with their respective performance scores. The
employeePerformance map stores performance scores for employees Satya and Ved. The debug log showcasesthe entire map, showcasing how maps facilitate key-value pair storage for effective datarepresentation.

---

## Page 206

In each snippet, we declare and manipulate a specific collection type, and the subsequent debug logstatement displays the outcome of those operations. This emphasizes how these collection typesefficiently manage and organize data within Apex.
Apex classes and methods
In Apex, classes, and methods provide a structured way to encapsulate and execute custom logic. Letus look at an example:
public class ArithmeticOperations {
    public Integer add(Integer firstNumber, Integer secondNumber) {
        return firstNumber + secondNumber;
    }
}
ArithmeticOperations math = new ArithmeticOperations();
Integer result = math.add(5, 3);
System.debug('Result: ' + result);
Let us look at the details of the above code: Class declaration: We declare a class named ArithmeticOperations. The public keyword makes theclass accessible outside its own namespace.
Method declaration: Inside the class, we define a method named add that takes two integerparameters (firstNumber and secondNumber). The method returns the sum of these numbers.
Class instantiation: We create an instance of the ArithmeticOperations class named math. This instanceallows us to access the methods within the class.
Method invocation: We call the add method on the math instance, passing values 5 and 3. Themethod calculates the sum and returns the result.
Debug log: The debug log statement prints the result of the addition operation, which is thendisplayed in the debug logs.
This example demonstrates how classes and methods in Apex facilitate modular and reusable code. The
ArithmeticOperations class encapsulates the logic for addition, and by creating an instance (math), we caninvoke its methods to perform specific operations. The result is then utilized in the debug log formonitoring and debugging purposes.
In the upcoming sections, we will explore more advanced concepts like how to integrate Apex withSalesforce flow to create powerful custom actions.
Invocable method annotation
After grasping the basics of Apex, let us explore the concept of invocable methods in Apex andunderstand how they can be leveraged. An invocable method is a method marked with the @InvocableMethod
annotation, allowing it to be called by the Process Builder or flow.
The properties of an invocable method are as follows: The method must be static, public, or global.
It should belong to the outer class.
Only one method in a class can have the @InvocableMethod annotation.
Triggers cannot reference invocable methods.
Invocable methods accept only one argument.

---

## Page 207

When a flow invokes an Apex class, the running user must have the necessary permissions enabledfor the Apex class, either at the profile level or through a permission set.
Let us create a new class to explore the invocable method detail: 1. Create a simple Apex class: 1. Begin by crafting a straightforward new Apex class with name OpportunityActionHandler.
public class OpportunityUpdateAction {
       // Add your InvocableMethod and other logic here
2. Add your InvocableMethod and other logic: 1. Extend your Apex class by adding the invocable method. In this example, we will use the
OpportunityActionHandler class created above. This class will contain an invocable method named
updateDescriptionField, which updates the standard description field on opportunity records.
public class OpportunityUpdateAction {
          /**
           * Invocable method to perform a custom action on Opportunityrecords.
           * Updates the standard Description field based on specifiedconditions.
           * @param opportunityIds The Ids of the Opportunity recordsto process.
           */
          @InvocableMethod(label='Update Description'description='Updates the standard Description field on Opportunityrecords')
          public static void updateDescriptionField(List<Id>opportunityIds) {
              try {
                  // Placeholder logic: Update the standard Descriptionfield on Opportunity records
                  List<Opportunity> opportunitiesToUpdate = [SELECT Id,Amount, StageName, Description FROM Opportunity WHERE Id IN:opportunityIds];
                  for (Opportunity opportunity : opportunitiesToUpdate){
                      // Your business logic to update the standardDescription field based on Amount and Stage
                      if (opportunity.Amount > 10000 &&opportunity.StageName.equals('Closed Won')) {
                          opportunity.Description = 'High ValueOpportunity - Closed Won';
                      }

---

## Page 208

}
                  // Update the records
                  update opportunitiesToUpdate;
                  System.debug('Description Field Updated forOpportunities: ' + opportunityIds);
              } catch (Exception e) {
                  System.debug('Error updating Description field: ' +e.getMessage());
                  // You can handle the exception or log it as needed
              }
          }
  }
2. This invocable method within OpportunityUpdateAction demonstrates how to update the standarddescription field on opportunity records based on specified conditions.
3. Use the invocable method in a flow: 1. Now that you have your invocable method within the Apex class, you can seamlessly use it in aflow. Open or create a flow in Salesforce Setup, add an Apex Action element, and select theOpportunityUpdateAction and the updateDescriptionField method. Map the requiredinput parameters, and your flow is set to invoke the custom action. Let us learn it in nextsection in details.
Execute Apex actions
For executing the Apex action, the first step is to create a flow in Salesforce. Follow the steps given tointegrate the previously created OpportunityUpdateAction into a flow: 1. Navigate to flow Builder: 1. In Salesforce Setup, go to the flow section.
2. Click on New flow to start building a new flow.
2. Select flow type: 1. Choose the type of flow you want to create.
3. Drag and drop elements: 1. In the flow Builder interface, drag and drop elements to define your flow's logic. Use elementslike Record Lookup, Assignment, or any other required elements to prepare list ofopportunity ID in a collection variable.
4. Add Apex action:
To include the previously created Apex action: 1. Click on Add Element and select Action as shown in Figure 12.2:

---

## Page 209

Figure 12.2: Add action
Choose the Filter By Type then Apex Action element as shown in Figure12.3:
Figure 12.3: Apex action
2. In the Action, choose the Apex class (OpportunityUpdateAction). Map the input parametersopportunityIds from the flow to the Apex action.
3. As per implementation of Apex action, for each input parameter required by the Apex action,configure the source. This might include specifying a constant value, using a variable from theflow, or mapping it from a record field.

---

## Page 210

5. Connect flow elements: 1. Connect the elements of your flow to define the order of execution. Ensure that the Apexaction is placed at the appropriate point in the flow where you want the custom action tooccur.
6. Save and activate the flow: 1. Once you have configured the flow, save it, and then activate it to make it available forexecution.
7. Execute the flow: 1. Run the flow by triggering it manually or through an automated process, depending on theflow's setup you have configured.
8. Monitor debug logs: 1. Check the debug logs in Salesforce to monitor the execution of the Apex action. Debug logsprovide insights into the actions performed by the Apex code.
You have successfully created a flow incorporating the custom Apex action (OpportunityUpdateAction).The flow can now be triggered to execute the specified logic on opportunity records using the invocablemethod.
Using a custom Lightning Web Component
In Salesforce flows, LWC bring a whole new level of customization and interactivity. By integratingcustom LWCs into flow screens, you can create dynamic and personalized user experiences. Thiscapability allows you to extend the functionality of your flows beyond the standard components, offeringa tailored solution to meet specific business needs.
The custom LWCs can be used in the flow screens for the following reasons: Enhanced user interaction: Custom LWCs empower you to build visually appealing and user-friendly interfaces within flow screens, elevating the overall user experience.
Tailored functionality: Leverage the power of LWCs to introduce bespoke features andfunctionalities that might not be achievable with standard flow elements alone.
Seamless integration: Integrating custom components ensures a seamless blend with the overallSalesforce Lightning Experience, maintaining consistency across the platform.
Dynamic data handling: With custom input fields and configurable properties, LWCs allowdynamic handling of data, providing a more flexible and adaptive approach in your flows.
Configuration steps
Now, let us explore the step-by-step process of integrating a custom LWCs into a flow screen to harnessits full potential. The steps are as follows: 1. Update the configuration file: 1. To make your LWC compatible with a flow screen, you need to update its configuration file.The lightning__FlowScreen target should be added to declare its usability in flow screens. Let usillustrate these concepts with an example using a LWC named EnhancedUserDetails.
<!-- EnhancedUserDetails.js-meta.xml -->
<targets>

---

## Page 211

<target>lightning__FlowScreen</target>
</targets>
2. Define input fields: 1. Specify the input fields for your LWC by adding targetConfig properties. These propertiesestablish the communication between the flow screen and the component.
<!-- EnhancedUserDetails.js-meta.xml -->
<targets>
    <target>lightning__FlowScreen</target>
    <targetConfigs>
        <targetConfig targets="lightning__FlowScreen">
            <objects>
                <!-- Specify objects if needed -->
            </objects>
            <properties>
                <!-- Specify properties for interaction -->
            </properties>
        </targetConfig>
    </targetConfigs>
</targets>
3. Property role restrictions: 1. Customize the behaviour of properties by using the role attribute. This attribute helps controlwhether a property is set as input-only, output-only, or both.
<!-- EnhancedUserDetails.js-meta.xml -->
<targets>
    <target>lightning__FlowScreen</target>
    <targetConfigs>
        <targetConfig targets="lightning__FlowScreen">
            <objects>
                <!-- Specify objects if needed -->
            </objects>
            <properties>
                <!-- Restrict a property to output-only -->
                <name>propertyName</name>
                <type>String</type>
                <label>Property Label</label>
                <role>OutputOnly</role>

---

## Page 212

</properties>
        </targetConfig>
    </targetConfigs>
</targets>
2. Here is an example where the EnhancedUserDetails component is configured to accept a userId asinput and provide additional user details as output on the flow screen.
<!-- EnhancedUserDetails.js-meta.xml -->
<targets>
    <target>lightning__FlowScreen</target>
    <targetConfigs>
        <targetConfig targets="lightning__FlowScreen">
            <objects>
                <object>*</object>
            </objects>
            <properties>
                <name>userId</name>
                <type>String</type>
                <label>User ID</label>
                <role>InputOutput</role>
            </properties>
        </targetConfig>
    </targetConfigs>
</targets>
4. Use in flow: 1. Locate and add your custom LWC, in this case, EnhancedUserDetails.
2. Configure the input fields as needed, providing dynamic values or variables.
3. Save and activate the flow.
By following these steps, you can seamlessly integrate your custom LWC into a flow screen, unlocking aworld of possibilities for personalized and efficient user interactions within your Salesforce processes.
Embed a flow in the custom Lightning Web Component
In Salesforce, combining flows and LWCs enables developers to create dynamic and interactive userexperiences. Embedding a flow within a custom LWC offers additional flexibility and control, allowing forhighly tailored and engaging user journeys.
Significance of embedding flow in LWC
Flows are essential for guiding users through Salesforce processes. Embedding a flow within a customLWC enhances the user experience by seamlessly combining declarative and programmatic techniques.

---

## Page 213

This integration allows for the creation of personalized, dynamic interactions and custom functionalitynot supported by standard flows, providing a powerful tool for Salesforce users.
A quick guide to embed a flow
Here are the steps to help you embed a flow in LWC. 1. Create the LWC: 1. Start by developing a custom LWC that serves as the container for your embedded flow. Craftthe component using HTML, JavaScript, and CSS to match your design requirements:
<!-- YourComponent.html -->
      <template>
        <!-- Add your custom styling and structure here -->
        <lightning-flow flow-api-name="Your_Flow_API_Name"></lightning-flow>
      </template>
2. Optional- Pass input values to the flow: 1. If your flow requires initial input values, set the flow-input-variables attribute in your LWC'sJavaScript file. This allows dynamic configuration based on the component's context.
// Component.js
import { LightningElement } from "lwc";
export default class YourComponent extends LightningElement {
  get inputVariables() {
    return [
      {
       name: "VariableName",
        type: "String",
        value: "InitialValue",
      },
      // Add more variables if needed
    ];
  }
}
Considerations for success
Always keep the following points in mind: Ensure that the lightning-flow component supports active flows for the flow-api-name attribute.
You can provide initial inputs for the flow interview by setting the flow-input-variables attribute.
Use the onstatuschange event to handle changes in the flow interview status for additional actions.

---

## Page 214

By following these steps, developers can seamlessly integrate Salesforce flows into custom LWCs,providing users with a highly customized and engaging experience.
Conclusion
In this chapter, you learned how to create your personal custom Apex actions and explored the basics ofApex programming.
The power of the @InvocableMethod annotation was looked at, allowing you to improve your automationskills. Executing Apex actions in flows is simplified, providing a seamless and efficient way to enhanceyour processes.
We also looked at LWCs, discovering how to use them in flow screens and embed flows within them.The combination of these tools opens endless possibilities for creating dynamic and user-friendlyexperiences.
The skills you acquire will help you in unlocking new levels of customization and efficiency in Salesforce.Whether you are a beginner or an experienced user, the knowledge gained here sets the stage for yoursuccess in Salesforce automation.
In the upcoming chapter, you will explore industry standard best practices, uncover the art oftroubleshooting, and discover ways to enhance your flow logic to steer clear of governor limits. Beprepared to learn how to design your flows with utmost efficiency, addressing common issues andconsidering vital aspects such as flow limits, data considerations, and optimizing for the Lightningruntime.
We will also cover topics like mastering the art of fixing flow issues, leveraging debug logs for runningflows, and understanding the nuances of flow Lightning runtime.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 215

CHAPTER 13Best Practices and Troubleshooting Measures
Introduction
In this chapter, we will explore the critical aspects of Salesforce flow, focusing on best practices,understanding limitations, and troubleshooting common issues. By delving into these areas, you willgain valuable insights into effective flow design and execution. As we navigate through this chapter, youwill learn how to identify and address common flow issues, adopt industry best practices, andunderstand the limitations of Salesforce flow to enhance your processes.
By the end of this chapter, you will be equipped with the skills needed to optimize your flowimplementations, ensuring that your processes are not only functional but also efficient and robust. Thisholistic view of flow's potential will empower you to create seamless user experiences while leveragingthe full capabilities of Salesforce.
Structure
This chapter is organized into the following sections: Flow limits and considerations
Flow best practices
Bulkify your flow
Mastering to fix common issues in flow
Considerations for flow data
Debug log for running flow
Considerations for flow Lightning runtime
Objectives
In this chapter, our primary goal is to provide a comprehensive understanding of Salesforce flow,catering to both beginners and advanced users. We aim to explore industry standard best practices andtroubleshooting measures to optimize the design and execution of flows. Throughout this chapter, wewill look at the flow limits, emphasizing on topics essential for working within Salesforce multitenantenvironment. Our objectives extend to mastering debugging techniques using flow Builder andleveraging debug logs for real-time insights into flow execution. We will also focus on the Lightningruntime for flows, looking at considerations, limitations, and testing scenarios. By the end of thischapter, you will gain valuable insights and skills to proficiently navigate Salesforce flow, ensuringefficient and robust automation.
Flow limits and considerations

---

## Page 216

In the expansive landscape of Salesforce, where numerous organizations share the same resources,understanding the limitations placed on flows is essential. These limits act as protective guardrails,ensuring that no single entity monopolizes too much of the shared capacity, which could potentially leadto performance degradation for all users. Salesforce operates within a multitenant environment,meaning that multiple organizations utilize the same resources within a single instance. The limitationsimposed on flows are crucial for maintaining system stability and performance, preventing any oneorganization from overwhelming the system and ensuring fair usage for all.
Limits for Salesforce flows
Salesforce flows operate within defined limits to ensure optimal performance and stability.Understanding these limits is essential for effective flow design and execution. The primary categoriesof limits include Query Limits, Data Change Limits, and Performance Limits: Query Limits: SOQL queries: Each flow can execute a maximum of 100 SOQL queries per transaction. Thislimit is designed to prevent excessive data retrieval that can slow down system performance. Example: If a flow is designed to pull account details for processing, it must bestructured to gather data efficiently, perhaps by consolidating multiple criteria into a singlequery to stay within the limit.
Records retrieved: You can retrieve up to 50,000 records per SOQL query. This means thatwhen querying for large datasets, you should ensure that the query is well-optimized toretrieve only the necessary records. Example: In a scenario where you need to fetch customer records based on specificcriteria, ensure that the query filters down the results to the most relevant entries to avoidunnecessary load.
Data Change Limits (DML statements): DML operations: flows can perform up to 150 DML changes per transaction, which includesadding, updating, or deleting records. This limit helps maintain system responsiveness bypreventing bulk operations that could monopolize resources. Example: When updating status fields for a batch of opportunities, structure the flow tocollect opportunities into a collection variable first and perform a single update operationinstead of updating each record individually within a loop.
Total records managed: A flow can handle a total of 10,000 records during DML operations.This means that if a flow attempts to modify a large number of records, it must be designed tobatch the operations effectively. Example: For a flow that processes multiple records from a report, consider splitting therecords into smaller batches to ensure that the total does not exceed this limit.
Performance Limits: CPU time: The maximum allowed CPU time for processing operations on Salesforce servers is10,000 milliseconds (10 seconds). This limit ensures that long running processes do not hinderperformance for other users. Example: If a flow contains complex logic that requires substantial processing, considerbreaking it down into smaller, more manageable flows or using asynchronous processes toimprove performance.

---

## Page 217

Batch operations: In batch processing, duplicate updates are limited to a maximum of 12times in a single batch operation. This restriction helps maintain data integrity and preventsexcessive load on the system. Example: When implementing a flow to update records in bulk, ensure that each batchonly performs necessary updates to stay within this limit. Using collection variableseffectively can help manage updates without exceeding the threshold.
Data handling considerations
Salesforce flows are not optimized for handling large volumes of data simultaneously. For bulk dataoperations, consider using tools like Apex or Salesforce Data Loader for faster and more efficientprocessing.
Example: If you need to update thousands of records, using Data Loader is significantly more efficientthan attempting to handle these updates solely through a flow.
Flow best practices
When working with Salesforce flows, adhering to best practices can significantly streamline yourdevelopment process, save time, and enhance efficiency. Here are some essential best practices, alongwith their importance and relevant examples: Collaboration and testing: Importance: Engaging team members in the development and testing process leads to betterdesigns and minimizes errors, especially when changes to subflows are required.
Example: Before finalizing a flow that handles customer orders, collaborate with your team toreview the logic and conduct thorough testing. This collaborative approach can uncoverpotential issues and improve the overall design.
Document everything: Importance: Thorough documentation ensures clarity and ease of maintenance. It serves asa reference for you and your team, especially during future modifications.
Example: Before building a flow for onboarding new employees, document its purpose, thespecific data fields being updated, and the method of invocation (for example, triggered by abutton click). This helps prevent confusion later if multiple developers need to work on the flow.
Update fields before record save: Importance: For same record field updates, using before-save flow triggers optimizesperformance and ensures data integrity by updating fields before the record is saved.
Example: If a flow needs to update a field on an account record based on conditions (forexample, changing the account status), implement this logic using a before-save flow trigger.This approach avoids unnecessary delays and ensures that the data is accurate before therecord is saved.
Avoid data elements in loops: Importance: Placing data elements within a loop can lead to performance issues and riskhitting Salesforce governor limits, potentially causing flows to fail. Data elements are shown inFigure 13.1.
Example: When developing a flow that updates multiple account records, collect all theaccounts into a collection variable first. Then, perform a single DML operation outside the loop

---

## Page 218

to update all accounts at once, significantly improving performance and avoiding governorlimits.
Use sObject collection variables and assignment steps outside the loop for betterperformance.
Figure 13.1: Data elements Use after-save logic wisely: Importance: After-save triggers are designed for tasks that need to occur after the recordhas been saved, thus ensuring that all data is available for the flow’s logic.
Example: If you need to send a welcome email to new employees after their records havebeen created, implement this logic in an after-save trigger. This ensures that all fields, such asemail addresses, are populated and accurate.
Exercise caution with formula variables: Importance: Using complex formula variables in Salesforce flows requires careful attention toensure they function as intended, particularly when dependent on multiple fields.
Example: If a formula relies on several variables that might not always be populated, it couldlead to unexpected results. Before finalizing a flow that calculates discount rates based onvarious criteria, test the formula thoroughly to ensure all potential input scenarios are handledcorrectly.
Debugging ease: Importance: flows are typically easier to debug than other automation tools like ProcessBuilder. Quick debugging allows you to identify and resolve issues efficiently.
Example: If you encounter an error in your flow that handles customer feedback, you can usethe debugger to step through each element and identify where the logic breaks, facilitatingfaster fixes compared to reviewing complex Process Builder configurations.
Avoid hard-coding Salesforce IDs: Importance: Hard coded IDs can lead to maintainability issues, especially when migratingflows between different Salesforce environments (e.g., from sandbox to production).
Example: Instead of hard coding an ID for a record type in a flow, use the Get Recordelement to dynamically retrieve the record type ID based on the record's criteria. This ensuresthat your flow works seamlessly across various environments.
Always set a fault path: Importance: Designing a fault path allows you to gracefully handle errors that may ariseduring flow execution, improving user experience and data integrity.

---

## Page 219

Example: If a flow that processes customer orders encounter an error, having a fault pathconfigured to display a user-friendly error message or send an alert to the admin helps introubleshooting and maintains user trust.
As shown in Figure 13.2, design a fault path to handle flow errors effectively. You can use
{!$Flow.FaultMessage} to get a fault message.
Figure 13.2: Fault path in flow Use debugger instead of saving many versions: Importance: Utilizing the debugger allows you to quickly test and iterate on your flowwithout cluttering your org with multiple versions. You can easily fix and improve your workwithout creating multiple versions.
Example: If you are refining a flow that automates billing, use the debugger to test changesin real-time. This approach helps you in save time and spot issues instantly without creatingnew flow versions.
Find failed flows faster: Importance: Quickly locating failed flows aids in efficient troubleshooting and minimizesdowntime.
Example: Instead of sifting through emails for error notifications, navigate directly to thePaused and Failed flow Interviews section in Setup, as shown in Figure 13.3. This allowsyou to address any issues promptly.
Figure 13.3: Paused and failed flow interviews

---

## Page 220

Use subflows for reusability: Importance: Subflows promote modular design, making it easier to maintain and update yourlogic without duplicating effort.
Example: If multiple flows require the same logic for sending notifications, implement thislogic as a subflow. This way, any changes made to the notification logic will automatically applyto all calling flows, ensuring consistency and reducing errors.
Build in a test environment first: Importance: Developing and testing flows in a sandbox or developer environment reducesthe risk of impacting production data and allows for thorough testing.
Example: Before deploying a flow that automates lead qualification, build and test it in asandbox to ensure that all logic works as expected. This practice helps catch errors early,minimizing disruptions when the flow goes live.
Wait until the end to edit the database: Importance: Restricting data access during flow design ensures that data integrity ismaintained throughout the process.
Example: If your flow processes customer orders, make all necessary database edits at theend of the flow, ensuring that all relevant data is collected and validated before any changesare made. This practice prevents partial updates and maintains accurate records.
Incorporating these best practices into your flow development process can lead to more efficient,maintainable, and scalable solutions.
Bulkify your flow
In the world of Salesforce automation, optimizing your flow to handle records in bulk is not just goodpractice; it is crucial. Welcome to the concept of bulkification, where we ensure that any automation, webuild is optimized to handle multiple records, minimizing the consumption of governor limits.
Understanding transactions and governor limits
Transactions encompass everything between DML operations and commits, and they are bound bygovernor limits. When dealing with large datasets, Salesforce processes the data in batches, eachcontaining a maximum of 200 records, ensuring that each batch operates within the governor limits.
For example, when processing a large dataset of 10,000 records, Salesforce divides the data intobatches of 200 records each. Each batch is processed separately, ensuring that the transaction stayswithin governor limits. Failing to bulkify your flow can lead to hitting Salesforce governor limits, resultingin incomplete transactions and potentially causing data integrity issues.
Bulkified flow elements
Elements that create, update, or delete records, lookup records, and send emails fall under the categoryof bulkified elements. When these elements are reached in your flow, Salesforce waits until all flowinterviews reach that point, executing the bulkifiable element just once across all interviews, effectivelyconserving governor limits.
Example: Suppose you need to update the status of multiple opportunity records based on certaincriteria. Instead of updating each record individually, use a collection variable to gather all relevantrecords and perform a single bulk update operation.
Guidelines for achieving bulkification in a flow
To ensure that bulkification is achieved in your flow, implement the following guidelines:

---

## Page 221

1. Use bulk query and bulk DML actions: Step 1: Use bulk query actions to retrieve multiple records at once. For instance, use the GetRecords element to fetch all opportunity records that meet a certain condition.Step 2: Use bulk DML actions, such as Update Records, to apply changes to all records atonce. For example, after retrieving relevant opportunity records, store them in a collectionvariable and update their status in a single operation.Importance: This minimizes the number of DML operations, ensuring that your flow operatesefficiently.
2. Minimize SOQL queries and DML statements: Step 1: Consolidate SOQL queries to reduce their number. For example, if you need to retrieverecords from two related objects, perform a single query that includes both.Step 2: Use collection variables to store results, reducing the need for additional queries later.Importance: Minimizing SOQL queries and DML statements reduces the risk of hittinggovernor limits and improves the efficiency of your flow. For instance, excessive queries canslow down processing and lead to timeouts.
3. Aggregate data before processing: Step 1: Before performing calculations, collect all necessary data into a single variable.Step 2: Perform the aggregation (for example, summing values) in memory before updatingrecords.Example: If calculating total sales for multiple opportunities, aggregate the sales values firstand then update the opportunities with the calculated total.Importance: This reduces the number of operations, speeding up your flow and minimizingresource consumption.
4. Avoid nested queries and loops: Step 1: Instead of nesting queries within loops, retrieve all related records in a single querybefore entering a loop.Step 2: Use collection variables to process records collectively.Importance: Nested queries can cause performance degradation and lead to governor limitsbeing hit. For instance, querying within a loop can exponentially increase the number ofqueries executed.
5. Bulk-enabled flow elements: Step 1: Utilize flow elements specifically designed for bulk processing. The Get Recordselement, when bulkified, retrieves all relevant records in a single operation.Step 2: Ensure that DML actions are set to operate on collections.Importance: Using bulk-enabled elements helps to optimize performance and managegovernor limits effectively.
6. Filter and process in batches: Step 1: Implement filters to segment records into manageable batches based on criteria (forexample, status or region).Step 2: Process each batch separately to prevent exceeding limits.Importance: This reduces the risk of hitting governor limits when dealing with very largedatasets.

---

## Page 222

7. Test with bulk data: Step 1: Create a test environment to simulate processing large datasets.Step 2: Run your flow with sample data sets that represent the maximum number of recordsexpected.Importance: Thorough testing helps identify performance bottlenecks and ensures that yourflow operates efficiently without exceeding governor limits.
8. Error handling: Step 1: Implement fault paths in your flow to capture errors during processing.Step 2: Route these errors to a dedicated log or notification process for review.Importance: Proper error handling is crucial for maintaining data integrity and userexperience during bulk processing.
Mastering to fix common issues in flow
While working with flows in Salesforce, you may encounter situations where your flow seems to hit aroadblock. Common issues can range from using the wrong field or incorrect variables to flawed logic,permission conflicts, or even problematic code. However, addressing these challenges becomes moremanageable with the right strategies. This section discusses some effective methods for troubleshootingand fixing common flow issues.
Proactive testing with debug
Before integrating your flow into established processes, utilize Salesforce's debug feature in the flowBuilder (as shown in Figure 13.4). This proactive testing allows you to identify and resolve potentialissues before they impact your production environment.
Example: When developing a flow that calculates discounts on opportunities, running the flow indebug mode enables you to see the values of variables at each step, helping you verify that thecalculations are performed correctly.
Figure 13.4: Debugging in flow Builder

---

## Page 223

Check for required fields
Ensure that all necessary fields are provided when creating a flow for any object. For instance, whenworking with the opportunity object, essential fields like Name, Stage Name, and Closed Date must beincluded. Missing any required fields can trigger errors in your flow (as shown in Figure 13.5).
Justification: Properly identifying and including required fields minimizes the risk of errors when theflow attempts to save or update records.
Figure 13.5: Ensuring required fields
Handling flow errors caused by inactive users
If you encounter errors when resuming a paused flow due to an inactive user, consider freezing theuser. Complete all flow interviews assigned to them before deactivating the user. This precaution helpsprevent disruptions caused by inactive users.
Scenario: For example, if a flow is scheduled to run tasks for a sales rep who is no longer active, theflow might fail when it tries to execute actions tied to that user.
User permissions matter
The smooth operation of a flow might be exclusive to the admin. When other users face issues, it isoften due to lacking necessary permissions. Always verify and grant the required permissions to ensureconsistent results.
Example: If a flow updates records but users receive an insufficient privileges error, check the userprofiles and permission sets to ensure they have access to the relevant objects and fields.
Beware of null values
In DML operations within flows, especially when dealing with IDs, be diligent about checking for nullvalues. Overlooking this step can lead to unexpected errors.
Example: When updating records based on a collection variable, ensure that the variable is not nullbefore attempting to perform a DML operation. Adding a Decision element to check for null can preventunnecessary errors.
Reviewing and debugging
When your flow breaks, review the logic and flow elements. Salesforce's debug feature enables you tostep through each element, inspect variables, and identify the root cause of issues.
Justification: Systematic debugging allows you to isolate where the flow is failing, whether due toincorrect data, faulty logic, or misconfigured flow elements.

---

## Page 224

Documentation and collaboration
Document your flow comprehensively, including its purpose, triggers, and any special considerations.Collaborate with others to gain different perspectives and insights when troubleshooting.
Example: Maintaining a centralized document detailing the flow's functionality and configurations helpsonboard new team members and aids in troubleshooting efforts when issues arise.
Considerations for flow data
When engaging with data in Salesforce flow, understanding and addressing various aspects is crucial forensuring effective and reliable automation. The key considerations for flow data are as follows: Object and field permissions: Verify that the user executing the flow possesses the necessary permissions to access andmodify the objects and fields involved in the flow.
Incorrect permissions can lead to execution failures and hinder the intended automation.
Variables: When deleting a record variable or record collection variable, note that variable assignmentsusing the deleted variable are set to null.
When one flow launches another, input variables can receive values during launch. For non-collection text, picklist, or multi-select picklist variables, a null value is converted to an emptystring.
Automatic storing of field values in the Get Record element is available only for screen flowsand auto launched flows.
Bulkification: Design your flows with bulk processing in mind to efficiently handle multiple records. This notonly minimizes governor limits but also ensures scalability and optimal performance.
API limits: Be aware of Salesforce API limits, especially when integrating with external systems. Monitorand optimize your flow to avoid exceeding API callout limits.
Date and date/time: During the runtime of a flow, be mindful that the time zones associated with date and timevalues may differ from what is visually represented in flow Builder.
Date and time values at runtime align with the time zone settings of the user actively runningthe flow.
Governor limits: Stay aware of Salesforce governor limits, such as SOQL queries, DML statements, and CPUtime.
Design your flow to stay within these limits to ensure optimal performance and avoid executionfailures.
By keeping these considerations in mind, you ensure that your flow not only functions as intended, butalso operates seamlessly within the broader Salesforce ecosystem. Now, let us explore how to use thedebug log for running flows in the next section.
Debug log for running flow

---

## Page 225

When troubleshooting and fine-tuning your Salesforce flows, the debug log is an invaluable tool thatprovides detailed insights into the execution process. Understanding how to utilize the debug log forrunning flows can significantly enhance your ability to identify and resolve issues effectively.
Follow these steps to enable debug logging: 1. Navigate to Setup in Salesforce.2. In the Quick Find box, enter Debug Logs.3. Click on Debug Logs as shown in Figure 13.6, and then click New.
Figure 13.6: Debug logs
4. Select the User for whom you want to generate the log as shown in Figure 13.75. Set the start and end date for the log.6. Choose the appropriate log levels. For flow debugging, set Workflow and Apex Code to Finest.
Figure 13.7: New debug logs
For logging flow execution, do the following: 1. Once debug logging is enabled, perform the actions that trigger your flow.

---

## Page 226

2. Navigate back to the Debug Logs page and refresh until you see the generated log for the user, asshown in Figure 13.8.
Figure 13.8:  Debug log details
Interpreting flow debug logs involves the following steps: 1. Open the log and look for entries related to your flow.2. Filter by the flow's name to narrow down the log entries.3. Pay attention to elements like FLOW_START_INTERVIEW, FLOW_ELEMENT_BEGIN, andFLOW_ELEMENT_END.
The key debugging information to be kept in mind is as follows: Flow execution steps: Understand the sequence of steps taken during flow execution.

---

## Page 227

Variable values: Check the values of variables at different stages of the flow.
Element execution times: Identify which elements take the most time to execute.
Error details: Debug logs provide error messages and details when something goes wrong.
Tips for efficient debugging are as follows: Focused logging: Set log levels only for the areas you are troubleshooting to reduce log size.
Use system.debug(): Introduce debug statements within your flow using the Debug element tolog specific information.
Iterative debugging: Make small changes, run the flow, and analyze the debug log. Repeat untilissues are resolved.
External tools: Leverage external tools like Salesforce Inspector or Developer Console foradvanced debugging.
By mastering the debug log for running flows, you empower yourself to swiftly identify, diagnose, andresolve issues within your Salesforce automation, ensuring a smooth and efficient workflow. Now, let usexplore considerations for flow Lightning runtime in the next section.
Checking failed or paused flow interviews
To review failed or paused flow interviews, follow these steps: 1. Navigate to Setup and type Paused and Failed flow Interview in the Quick Find box as shown in Figure13.9.2. Access the corresponding screen and manage failed or paused flow interviews efficiently afterclicking on Name.
Figure 13.9: Paused and failed flow interviews
Debugging flow during development
During developing a flow, encountering challenges with a process that is not functioning as expected isnot uncommon. This is where the debug option in flow Builder proves to be an indispensable ally. Itgrants you real-time visibility into each step of your process, allowing you to precisely understand itsbehavior.
The benefits of flow Builder debugging are as follows: Real-time insight: The debug option enables you to observe each step of your process in real-time, shedding light on its inner workings.
Dynamic adjustments: You have the flexibility to adjust input variables, which are the dataelements your process works with, dynamically.
Restarting at any point: Restart your process at any juncture to delve into different parts of it,facilitating in-depth investigation.

---

## Page 228

The steps to debug your flow is as follows: 1. Open the flow in flow Builder.2. Click on the Debug button as shown in Figure 13.10:
Figure 13.10: Debug
3. Select input as shown in Figure 13.11:
Figure 13.11: Paused and failed flow interviews
4. Now click on Run.

---

## Page 229

5. As shown in Figure 13.12, you can check details log of your flow:
Figure 13.12: Debug details
These steps initiate the debugging process, allowing you to navigate through your flow's executionseamlessly.
By embracing the debugging features within flow Builder, you transform the development phase into amore interactive and insightful experience, ensuring the robustness of your processes before they golive.
Considerations for flow Lightning runtime
In the Lightning runtime environment, flow users consistently engage with the active version of a flow.Notably, users with the Manage flow permission, designated as flow admins, hold the capability toexecute the latest flow version for testing purposes without activating it for general users. This flexibilityextends to subflow elements, allowing flow admins to run the most recent version of a flow referencedthrough a subflow.
The key features for flow admins are as follows:

---

## Page 230

Testing unactivated versions: flow admins can execute the latest flow version for testingwithout activating it for all users.
Subflow testing: The ability to run the latest version of a flow called through subflow elements.
This strategic approach ensures that flow admins have the tools necessary to thoroughly test the latestflow versions independently and within the context of subflows.
Flow interview
A flow interview, akin to a record of an object, represents an instance of a flow. In an interview, variousdata can be passed into variables from sources such as Salesforce records, user inputs, or manualentries. Interviews do not execute actions, such as sending emails or modifying records, until theassociated transaction concludes. Transactions are complete when the interview either finishes orexecutes a screen.
Limitations of Lightning runtime for flows
When Lightning runtime is enabled, flows in Lightning Experience will not load in the followingscenarios: Web tabs: Execution of flows within web tabs in Lightning Experience is restricted.
List buttons with existing windows: flows will not load when invoked from list buttonsconfigured to open in an existing window, with or without a sidebar.
These limitations are in place to ensure a seamless user experience, encouraging the adoption ofLightning components for enhanced performance and functionality.
Flow runtime accessibility considerations
When utilizing screen readers or assistive technologies during the execution of screen flows, it is crucialto be aware of the following accessibility considerations: Screen title changes: The title of the screen might not change when navigating with Next orPrevious.
Labels for flow screen components: Components without defined labels may pose challengesfor screen readers.
Language settings: Mismatched language settings between screen readers and flow languagescan affect proper reading.
Incomplete required fields: Screen readers may struggle to read error messages when a userfails to complete a required field in certain components.
Addressing these considerations ensures a more inclusive and accessible user experience during theruntime of flows in Lightning Experience.
The following quick reference guide provides an overview of best practices and troubleshootingstrategies for optimizing Salesforce flows to ensure efficient and reliable automation:
 
 Best practices
 
 Description
  
  Proactive testing with debug
  
  Use the debug feature to test flows before deployment, allowing you to identify and resolve potential
issues early.
  
  Check for required fields

---

## Page 231

Ensure all necessary fields are included for the object being used in the flow to prevent errors during
record creation or updates.
  
  Handle flow errors from
inactive users
  
  Freeze inactive users before deactivating their accounts to avoid disruptions in paused flow
interviews.
  
  Verify user permissions
  
  Confirm that all users have the necessary permissions to operate the flow effectively, especially non-
admin users.
  
  Beware of null values
  
  Check for null values in DML operations to prevent unexpected errors, particularly when dealing with
IDs.
  
  Review and debug logic
  
  Use the debug feature to review flow logic, inspect variables, and pinpoint the root cause of issues
when a flow fails.
  
  Documentation and
collaboration
  
  Maintain comprehensive documentation of your flow's purpose, triggers, and special considerations
while collaborating with team members for insights.
  
  Utilize the log inspector
  
  Use the Log Inspector for advanced troubleshooting by analyzing system logs to identify
performance bottlenecks or errors in your flow.
  
  Analyze system logs
  
  Access system logs to diagnose issues, pinpointing errors and performance problems that may not
be visible in debug mode.
Table 13.1: Best practices and troubleshooting tips for Salesforce flows
The following table provides troubleshooting strategies:
 
 Troubleshooting strategy
 
 Description
  
  Using debug feature
  
  Access the debug feature in flow Builder to test the flow step-by-step, inspecting variables at each
stage.
  
  Validating user
permissions
  
  Review and adjust user permissions to ensure they have access to all necessary features and elements
of the flow.
  
  Inspecting null values
  
  Implement checks for null values in DML operations to avoid unexpected errors during execution.
  
  System log analysis
  
  Utilize the log inspector to analyze execution logs and identify areas causing delays or errors in flow
processing.
Table 13.2: Troubleshooting strategies
Conclusion
This chapter has equipped you with a robust set of skills and insights. From understanding theintricacies of flow limits and considerations to implementing industry-standard practices, this chapteraimed to connect theory and practical application.
Through the lens of bulkifying your flow, mastering issue resolution, and data considerations, weexamined the nuances of efficient flow design and offered solutions for common challenges. Thechapter also examined debugging with the log, teaching you to troubleshoot and optimize flowexecution effectively. Additionally, we navigated the considerations and limitations within the Lightningruntime for flows, ensuring a seamless user experience.

---

## Page 232

In the next chapter, you will explore user access for flows, distribution strategies for internal andexternal users, packaging considerations, and integrating flows with experience cloud and websites.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 233

CHAPTER 14Distributing and Sharing flows
Introduction
In this chapter, we will explore the crucial process of distributing and sharing flows within yourorganization and beyond. When investing time and effort into designing and testing your flows, it isparamount to ensure they reach the right users and stakeholders, empowering them to streamlineprocesses and drive efficiency. This chapter contains information that will help you in effectively sharingyour flows, from granting user access to deploying flows in various contexts.
Distributing and sharing flows is a crucial aspect of maximizing the utility and impact of your Salesforcesolutions. Once you have designed and tested your flows, it is essential to understand how to grantaccess to users, deploy flows within your organization, and distribute them to external stakeholders.This chapter will guide you through the process of sharing flows with internal and external users,exploring packaging considerations, and integrating flows into Experience Cloud portals and externalwebsites.
Structure
This chapter is organized into the following sections: User access for the flow
Distribute flows to internal users
Packaging considerations for flows
Distribute flows to external users
Experience Cloud and flows
Objectives
The chapter aims at providing you with the knowledge and skills needed to effectively distribute andshare flows. We aim to provide a deep understanding of the intricacies involved in granting user access,exploring packaging considerations, and leveraging different distribution methods. By the end of thischapter, you will have a comprehensive understanding of how to strategically deploy flows within yourorganization and extend their reach to external users and stakeholders. Furthermore, we will explorethe integration of flows into Experience Cloud portals and external websites, enabling you to enhanceuser experiences and streamline processes across various platforms.
User access for the flow
In Salesforce flow, managing user access is essential for controlling who can edit and run flows withinyour organization. This ensures that sensitive processes are only accessible to authorized users,maintaining data integrity and security. Let us explore how you can customize user access for your flowsin Salesforce.

---

## Page 234

Navigating flow access control
In Salesforce, you have the power to control who can edit and run your flows, all while adhering to thespecific needs of your organization. This is where flow access comes in, allowing you to customizepermissions based on user records, profiles, or permission sets.
Customizing access for your flows
The steps are as follows: 1. Finding your flow settings: 1. Begin by navigating to Setup and entering flows in the Quick Find box. Select flows to accessyour flow management settings.
2. Tweaking flow access: 1. Once in the flows section, identify the flow you wish to manage and click on its name to openits details.
3. Access settings: 1. Within the flow details, as shown in Figure 14.1, locate and click on Edit Access to adjust theaccess settings for the flow:
Figure 14.1: Edit access to flow
4. Adjusting access: 1. In the Edit Access section, you have the option to override the default access behaviour forthe flow. As shown in Figure 14.2, select Override default behavior and restrict access toenabled profiles or permission sets to customize access settings beyond the defaultconfigurations:

---

## Page 235

Figure 14.2: Override default behavior
5. Limiting access: 1. With the override in place, you can now restrict access to the flow based on specific userprofiles or permission sets. This ensures that only designated individuals can edit and run theflow.
6. Granting permissions: 1. From the list of available profiles, choose the ones you want to grant edit and run flowpermissions to. Simply move these selected profiles to the Enabled Profiles list by clickingAdd.
7. Saving your changes: 1. Once you have fine-tuned your access settings, do not forget to save your changes. Thisensures that your customized access permissions are applied effectively, safeguarding yourflow.
You can also control this flow permissions from the profile or permission set if override default behavioris checked in the above setting. The steps are as follows: 1. In Salesforce, navigate to Setup and search for Object Manager and search for Profile.2. Choose desired profile.3. Click on flow Access (permission to execute flows).4. Edit the flow Access as shown in Figure 14.3:

---

## Page 236

Figure 14.3: Edit flow access
5. Add Available flows to Enabled flow (the desired flow you want to give access to) and Save, asshown in Figure 14.4:
Figure 14.4: flow access to the profile
Distribute flows to internal users
Once you have designed and customized your Salesforce flow, and granted it access, then it is time toensure that your internal users can use it. Internal users within your Salesforce Organization are thebackbone of your operations. These users include sales representatives, managers, administrators, andother personnel who rely on Salesforce to perform their day-to-day tasks. Distributing flows to internalusers ensures that they have access to the tools they need to excel in their roles.
Here are some important points for planning distribution of flows to users:

---

## Page 237

Identifying target users: Before distributing a flow, it is essential to identify the specific internalusers who will benefit from it. Consider their roles, responsibilities, and the tasks they performwithin Salesforce.
User training and communication: Provide comprehensive training and communication tointernal users about the purpose and functionality of the flow. Ensure that they understand how theflow will streamline their workflows and improve efficiency.
Access configuration: Configure access settings to grant appropriate permissions to internalusers. Determine whether users need read-only access, edit access, or the ability to run the flow,and adjust permissions accordingly.
Sharing methods: Salesforce offers various methods for sharing flows with internal users,including sharing via profiles, permission sets, public groups, and roles. Choose the method thataligns best with your organization's structure and user roles.
Documentation and support: Provide comprehensive documentation and support resources tointernal users to help them navigate and use the flow effectively. This includes step-by-step guides,FAQs, and access to support channels for assistance.
Feedback and iteration: Encourage internal users to provide feedback on the flow's functionalityand usability. Use this feedback to iterate and improve the flow over time, ensuring that itcontinues to meet the evolving needs of your organization.
Here are some pro tips for internal user distribution: Regularly communicate updates and improvements to internal users to keep them informed andengaged.
Monitor usage metrics and user feedback to gauge the effectiveness of the distributed flows andidentify areas for improvement.
Create a culture of continuous learning and improvement within your team to drive adoption andmaximize the benefits of distributed flows.
We will explore various methods for allowing users to use flows in this section.
Create an object-specific quick action
When it comes to making processes more efficient, the best action would be launching a flow directlyfrom a record page. With just a few clicks, users can access the exact flow they need, right where theyneed it.
This method allows users to launch a flow directly from a record page by creating a quick action.
Let us look at the step-by-step instructions: 1. In your Salesforce Org, navigate to Setup and search for Object Manager.2. Select the desired object (example Contact), and click Buttons, Links and Actions.3. Click New Action as shown in Figure 14.5:

---

## Page 238

Figure 14.5: Create a new action
4. Choose flow as the Action Type as shown in Figure 14.6.5. Select the flow you want to launch as shown in Figure 14.6:
Figure 14.6: Action details
6. Add the newly created action to the desired page layout so users can access the action from recorddetails.
This approach provides easy access to flows from record pages, improving user productivity andworkflow efficiency.
Add a flow to the Actions & Recommendations component

---

## Page 239

The Actions & Recommendations component offers a curated list of suggested actions, including flows,conveniently displayed on Lightning pages. It is like having your own virtual guide, helping you navigatethrough tasks effortlessly.
With this approach, you can surface flows on Lightning pages using the Actions &Recommendations component. (You need to create a New Deployment as shown in Figure 14.7):
Figure 14.7: Create new deployment 1. Open the Lightning App Builder and select the desired Lightning page.2. Drag the Actions & Recommendations component onto the page layout.3. Configure the component to display the flow you want to include as shown in Figure 14.8.4. Save the changes to the Lightning page.
Figure 14.8: Actions & Recommendations
5. This approach offers a user-friendly interface for accessing flows and other recommended actionsdirectly from Lightning pages as shown in Figure 14.9:
Figure 14.9: View Actions & Recommendations
Add a flow to a utility bar

---

## Page 240

Adding flows to the utility bar helps save time. With just a glance at the bottom of the screen, users canaccess essential flows no matter where they are in Salesforce.
You can add flows for quick access across Lightning apps using the utility bar through the followingsteps: 1. Navigate to the App Manager in Setup and select the desired Lightning app.2. Click Edit and access the utility bar settings.3. Click Add Utility Item and select flow as the item type as shown in Figure 14.10.4. Choose the flow you want to add and configure its display settings.5. Save the changes to the Lightning app.
This approach enhances user productivity by providing easy access to flows from any page within aLightning app.
Figure 14.10: Add flow to utility bar
Sharing the flow URL
Whether it is through a custom button, link, or web tab, sharing the flow URL helps users to accessflows from anywhere in Salesforce.
To share flow URLs, follow the given steps: 1. Obtain the URL of the flow by navigating to the flow Setup.2. Click on View Details and Versions in front of your flow as shown in Figure 14.11:

---

## Page 241

Figure 14.11: View details and versions for flow
3. Copy the URL of the flow from URL as shown in Figure 14.12:
Figure 14.12: Get the URL of the flow
4. You can create a custom button, link, or web tab in Salesforce and configure it to redirect to theflow URL.
Embed a flow in a custom Aura component
Customization is essential when it comes to creating a seamless user experience. By embedding flowswithin custom Aura components, users can enjoy a tailored interface that aligns perfectly with theirworkflow.
To embed a flow in your Aura component, add the lightning:flow component to it, for example:
<aura:component>
  <aura:handler name="init" value="{!this}" action="{!c.init}" />
  <lightning:flow aura:id="flowData" />
</aura:component>
In the JavaScript controller, identify which flow to start, for example:
({
  init : function (component) {
    // Find the component whose aura:id is "flowData"
    const flow = component.find("flowData");
    // In that component, start your flow. Reference the flow's API Name as below

---

## Page 242

flow.startFlow("Employee_Onboarding");
  },
})
Embed a flow in a Visualforce page
Embedding flows in Visualforce pages offers a timeless approach to incorporating flows into Salesforce.With the flexibility and customization options of Visualforce, users can enjoy a familiar interface thatmeets their specific needs. 1. To embed flows in Salesforce using Visualforce pages, use the <flow:interview> component to embedthe flow within the Visualforce page.2. Set the name attribute to the API name of the flow:
<apex:page>
<flow:interview name="Employee_Onboarding"/>
</apex:page>
Call flow in Lightning Web Components
Integrating flows into LWC offers a modern approach to enhancing the user experience.
To embed a screen flow from any LWC with the new lightning-flow component, use the <lightning-flow> tagto call the flow within the LWC.
Figure 14.13: flow in LWC
Developers can improve their flows by customizing finish behavior, setting custom styling, or launchingflows from their LWCs. They can also offload complex input collection and branching logic to flow,saving time and money.
Prepare your org for paused flow interviews
Enabling the pause and resume feature ensures that the users can pick up right where they left off,even during unexpected interruptions. It gives users the flexibility and control they need to stayproductive.
To enable and configure the pause and resume feature to enhance user experiences with flows, ensurethat the pause and resume feature is enabled in your Salesforce.
From the Setup | Process Automation Setting, enable Let users pauses flows option as shown inFigure 14.4:

---

## Page 243

Figure 14.14: Process automation setting
Packaging considerations for flows
Packaging flows involves bundling their associated components to ensure portability and easydeployment across Salesforce environments. It is crucial to identify and include all dependent elementslike custom objects, fields, Apex classes, and other necessary flows for seamless functionality.Maintaining version control is essential for compatibility and efficient update management.
If you are distributing flows on the AppExchange or within managed packages, using a namespace isnecessary to avoid conflicts with other components.
Salesforce offers various package types tailored to different distribution and deployment requirements: Unlocked packages: Suited for open source and collaborative projects, prioritizing flexibility andcustomization.
Managed packages: Ideal for commercial offerings or proprietary solutions, offering greaterversioning and upgrade control.
Now, let us look at some best practices for packaging flows: Modularization: Break down complex flows into smaller, reusable modules to enhancemaintenance and reusability.
Documentation: Document flow dependencies, configuration instructions, and user/administratorconsiderations comprehensively.
Testing: Conduct thorough testing across different environments to ensure functionality andcompatibility.
Security: Consider security implications, especially regarding sensitive data or external systemintegration.
Performance optimization: Optimize flows for performance by minimizing resource consumptionand unnecessary processing steps.
When planning deployment, ensure a smooth transition across Salesforce environments: Deployment strategy: Carefully plan deployment to ensure a seamless transition.
Sandbox testing: Test flows in sandbox environments before production deployment.
Rollback plan: Have a rollback plan in place to address deployment failures or unexpected issues.

---

## Page 244

Training and support: Provide adequate training and support for effective usage andmanagement of packaged flows.
Additional packaging considerations for flows are as follows: Component inclusion: When packaging flows, ensure all referenced components and fields areincluded in the package or dependent packages.
Updating packaged flows: Follow specific steps to update managed package versions withoutdisrupting users.
Additional notes: Considerations like Apex actions, email alerts, namespace usage, andlimitations regarding flow triggers and deletion in packaging orgs should also be noted.
Distribute flows to external users
By expanding the scope of your Salesforce flows beyond internal users, you can extend the reach ofyour flows to external users. You can engage with customers, partners, and other external stakeholdersmore effectively, enhancing collaboration and driving business growth.
Using sites and Salesforce experience cloud involves the following steps: 1. Salesforce Sites and Salesforce Experience Cloud (Communities) provide platforms for hosting andsharing custom-branded websites and portals with external users.2. Drag the flow component in your Experience Cloud builder as shown in Figure 14.15:
Figure 14.15: flow in the Experience Cloud
3. Configure the flow as shown in Figure 14.16:

---

## Page 245

Figure 14.16: Configure your flow
Experience Cloud and flows
Experience Cloud, formerly known as Community Cloud, is Salesforce's platform for building brandedonline portals, communities, and websites. It enables organizations to connect and collaborate withcustomers, partners, and employees in a secure and personalized environment.
Leveraging Salesforce flows in Experience Cloud
Integrating Salesforce flows with Experience Cloud enhances the functionality and usability ofcommunity portals by providing interactive, guided experiences for users. With Salesforce flows,organizations can automate processes, streamline workflows, and deliver personalized interactionswithin their Experience Cloud environments.
Key use cases
The key use cases are as follows: Customer onboarding and account management: Guide new customers through theonboarding process with automated account setup and profile creation. Enable self-service accountmanagement for users to update information and access resources conveniently.
Case management and support: Empower customers to submit support requests and track casestatus directly within the community portal. Automate case routing and resolution processes toimprove responsiveness and customer satisfaction.
Knowledge base and self-service resources: Build interactive knowledge bases and self-service resources within the community portal using Salesforce flows. Provide guidedtroubleshooting steps and FAQs to enable users to resolve issues independently.
Appointment scheduling and event registration: Enable users to schedule appointments,book services, or register for events seamlessly through the community portal. Automateappointment scheduling workflows and send reminders to users for improved engagement.
Adding a flow to Experience Cloud
To add a Salesforce flow to your Experience Cloud portal, follow these steps: 1. Create or edit a Lightning community: 1. Navigate to Setup and select All Sites as shown in Figure 14.17:

---

## Page 246

Figure 14.17: Digital experiences
2. Choose the community you want to add the flow to or create a new one.
3. Enter the community builder and select the page where you want to add the flow.
2. Add a flow component: 1. In the community builder, drag and drop the flow component onto the desired page.
2. Configure the flow component by selecting the flow you want to add as shown in Figure14.18:
Figure 14.18: flow components
3. Configure the flow as shown in Figure 14.19:

---

## Page 247

Figure 14.19: Configure your flow
3. Customize and preview: 1. Customize the appearance and layout of the flow component to match the design of yourcommunity.
2. Preview the page to ensure the flow is displayed correctly and functions as expected.
4. Publish changes: 1. Once satisfied with the configuration, save and publish your changes to make the flowavailable to community users as shown in Figure 14.20:
Figure 14.20: Publish your site
Conclusion
In this chapter, we examine the important process of distributing and sharing flows within yourorganization and beyond. After you have invested time and effort into designing and testing your flows,it is paramount to ensure they reach the right users and stakeholders, empowering them to streamlineprocesses and drive efficiency. This chapter covers everything you need to know about effectivelysharing your flows, from granting user access to deploying flows in various contexts.
Distributing and sharing flows is crucial to maximizing the utility and impact of your Salesforce solutions.Once you have designed and tested your flows, it is essential to understand how to grant users access,deploy them within your organization, and distribute them to external stakeholders. This chapter tookyou through the process of sharing flows with internal and external users, exploring packagingconsiderations, and integrating flows into Experience Cloud portals and external websites.

---

## Page 248

In the next chapter, we will integrate flows outside of Salesforce and learn how to connect flows withdata that resides outside of Salesforce, stored in external databases. Topics to be covered includeexternal objects, outbound message actions, External Services, and HTTP Callouts. The next chapter willexpand your understanding of flow integration and empower you to leverage flow capabilities beyondthe confines of the Salesforce platform.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 249

CHAPTER 15Integrating flow Outside Salesforce
Introduction
In today's interconnected world, businesses often rely on a multitude of systems and services tostreamline their operations and serve their customers effectively. The need to integrate with externaldata sources, services, and APIs is increasingly common to create a seamless end-to-end process.
In this chapter, we will explore various methods for integrating flow processes outside of Salesforce,enabling you to connect and interact with data and services that reside beyond the confines of yourSalesforce Organization. From accessing data in external databases to triggering actions in third-partysystems, we will cover a range of techniques and best practices to extend the capabilities of your flowprocesses and create integrated solutions that span across Salesforce and external environments.
Structure
This chapter is organized into the following sections: External objects
Outbound message actions
Using External Services in flow
HTTP callout
Objectives
In this chapter, our aim is to equip you with the knowledge and skills necessary to seamlessly integrateSalesforce flow processes with external data sources, services, and APIs. We will delve into variousintegration techniques, including accessing data from external databases, triggering actions in third-party systems, and interacting with external services via HTTP requests.
By exploring the concepts of external objects, outbound message actions, External Services, and HTTPcallouts, you will learn how to bridge the gap between Salesforce and external environments, enablingyou to create end-to-end workflows that span across disparate systems. Whether you are synchronizingdata between Salesforce and external databases, automating processes in third-party services, orconsuming data from external APIs, this chapter will provide you with the tools and insights necessaryto extend the capabilities of your flow processes and create integrated solutions that meet the evolvingneeds of your business.
By the end of this chapter, you will be equipped with the knowledge and confidence to leverage theseintegration techniques effectively, empowering you to build robust, scalable, and interconnectedsolutions that drive value and efficiency for your organization.
External objects

---

## Page 250

External objects in Salesforce provide a powerful way to access and interact with data stored in externaldatabases, making it appear as if it were native Salesforce data. These external data sources couldinclude legacy databases, third-party systems, or even data stored in other Salesforce Organizations.Let us discuss its key features and benefits: Virtual representation: External objects create a virtual representation of the data in theexternal database within Salesforce, allowing you to interact with it using standard Salesforce toolsand processes.
Real-time access: External objects provide real-time access to data in external systems, ensuringthat your flow processes can stay up to date with the latest information.
Customizable integration: You can customize the integration of external objects to suit yourspecific requirements, defining the relationships between external data and Salesforce objects.
Using external objects in flow
Here are various ways you can use external objects in flow: Define external data source: Begin by defining an external data source in Salesforce, specifyingthe connection details for the external database.
Create external object: Once the external data source is defined, create an external object inSalesforce to represent the data from the external database.
Access external data in flow: With the external object set up, you can now access andmanipulate external data within your flow processes using standard flow elements such as recordlookup and record create.
Here are some use cases for external objects: Customer data integration: Integrate customer data from an external CRM system into yourSalesforce flow processes to streamline sales and service workflows.
Inventory management: Access inventory data from an external database to automateinventory updates and order processing within Salesforce.
Financial data integration: Incorporate financial data from an external accounting system intoyour flow processes for real-time reporting and analysis.
Prior to creating external objects, set up an External Data Source by following these steps: 1. From Setup, enter External Data Sources in Quick Find box and then select External Data Sources.2. Create a New Data Source with entries as shown in Figure 15.1. (In this example, we have useda public URL https://orderdb.herokuapp.com/orders.svc/ for demonstration):

---

## Page 251

Figure 15.1: Create external data source
3. Click on the Save button.4. Click on the Validate & Sync button.5. Check the external objects(tables) you want to use and click on the Sync button. Refer to thefollowing figure:
Figure 15.2: Select tables
6. Order and OrderDatail objects are synced. Now you can validate the external objects. Refer tothe following figure:

---

## Page 252

Figure 15.3: Synced tables
7. Click on the Order object, and from object details, it can be identified by (__x) underscoreunderscore x at the end of the object API Name. Refer to Figure 15.4:
Figure 15.4: External object details
Access external data in flow
Create a Screen flow and add the Get Records element, as shown in Figure 15.5. In the Object list,you can see that the Order external object is available. You can use it the same way you would a customobject in the flow:
Figure 15.5: Get records element
You can display the records in the screen element after dragging the Data Table, as shown in Figure15.6:

---

## Page 253

Figure 15.6: Fill data table details along with data source
Outbound message actions
Outbound message actions are a powerful Salesforce feature that allows you to trigger HTTP POSTrequests to external systems or services when certain criteria are met within your flow processes. Theseoutbound messages are sent asynchronously, enabling you to integrate with external systems withoutdisrupting the flow of your Salesforce processes. Here are its key features and benefits: Event-driven integration: Outbound message actions allow you to trigger external actions basedon specific events or conditions within your flow processes, such as record updates or workflow ruleevaluations.
Asynchronous communication: Outbound messages are sent asynchronously, meaning thatthey do not block the execution of your flow processes, providing a seamless integrationexperience.
Reliable delivery: Salesforce ensures reliable delivery of outbound messages by automaticallyretrying failed deliveries and providing delivery status notifications.
Using outbound message actions in flow
Here is how to use outbound message actions in flows: 1. Define outbound message action: Begin by defining an outbound message action in Salesforce,specifying the external endpoint URL to which the HTTP POST request will be sent.2. Configure trigger conditions: Configure the trigger conditions for the outbound message action,specifying the criteria that will cause the action to be triggered, such as record field changes orworkflow rule evaluations.3. Define message content: Define the content of the outbound message, including the data to besent to the external system and any additional headers or parameters required by the endpoint.4. Activate and test: Once the outbound message action is configured, activate it and test theintegration to ensure that the HTTP POST requests are being sent to the external system asexpected.
Here are the use cases for outbound message action: Integration with external systems: Trigger actions in external systems, such as sendingnotifications or updating records, based on events within your Salesforce processes.
Third-party integrations: Integrate with third-party services or applications, such as emailmarketing platforms or customer support systems, to automate communication and workflows.

---

## Page 254

Data synchronization: Synchronize data between Salesforce and external databases or systemsby triggering updates or data transfers via outbound messages.
Let us think of a use case for a business using Salesforce as well as an external system.
Imagine a business leveraging Salesforce as its primary platform for customer relationship managementand an external system to streamline additional processes.
In the heart of this dynamic business environment, Salesforce stands as the central hub for managingleads, contacts, accounts, and opportunities. However, the company has integrated Salesforce with anexternal system, recognizing the need to synchronize crucial information for comprehensive businessinsights.
As leads progress through the sales funnel and are eventually converted into accounts, contacts, andopportunities within Salesforce, it becomes imperative to relay this critical data to the external system inreal-time. This ensures that all stakeholders have access to the latest information, empowering them tomake informed decisions and drive business growth.
To address this challenge, the company employs the power of Salesforce flows and outbound messagesto seamlessly transmit essential data to the external system upon lead conversion.
So, here is what we are going to implement: when a lead is converted in Salesforce, we will initiate aflow to send essential data, including Converted Account ID, Converted Contact ID, ConvertedOpportunity ID, and Annual Revenue, to an external system via outbound messages.
Creating outbound message
Follow the given steps to create an outbound message: 1. Go to Home | Setup | search for Outbound Message | Click on Create Outbound Message button |select Lead Object. Refer to the following figure:
Figure 15.7: Select object
2. Click on the Next button.3. Fill the following details: 1. Name: Lead conversion outbound Message
2. Unique Name: Lead_conversion_outbound_Message
3. Endpoint URL: Enter the URL that accepts lead information into the Endpoint URL field.
4. Protected component: Checked
5. Send Session ID: Checked

---

## Page 255

4. Add fields that you want to send.5. Click on the Save button.
Creating triggered flow
Here is how to create a triggered flow: 1. Go to Setup | search for flow | click on New button | select Record-Triggered Flow | click onCreate button. Refer to the following figure:
Figure 15.8: Record-triggered flow
2. Add action Element and then follow the steps: 1. Category | Outbound Messages | select your outbound message that you just created.
2. Save the flow: Activate the flow by Clicking on Activate button.
3. Convert any of the lead record and verify the data received in external system.
4. Salesforce will continue sending requests until it receives a response from the external system.Refer to Figure 15.9.
(Setup | Monitor | Outbound Messages):

---

## Page 256

Figure 15.9: Salesforce Waiting for XML Response
Salesforce accepts the response in XML format. An example is provided below:
<?xml version="1.0" encoding="UTF-8"?>
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:out="http://soap.sforce.com/2005/09/outbound">
<soapenv:Header/>
<soapenv:Body>
<out:notificationsResponse>
<out:Ack>true</out:Ack>
</out:notificationsResponse>
</soapenv:Body>
</soapenv:Envelope> 
External Services
External Services in Salesforce provide a powerful way to integrate your flow processes with externalservices and APIs, allowing you to perform actions such as making HTTP requests, invoking SOAPservices, or consuming REST APIs directly from your flow. Here are the key features and benefits: Seamless integration: External Services enable seamless integration with external systems andservices, providing a unified interface within Salesforce flow to interact with a wide range ofexternal endpoints.
Standardized invocation: External Services allow you to define standardized invocable methodsthat encapsulate the functionality of external services or APIs, simplifying the integration processand promoting reusability.

---

## Page 257

Enhanced productivity: By leveraging External Services, you can streamline the development offlow processes that require interaction with external systems, reducing the need for custom codeand accelerating time to value.
Using External Services in flow
Follow the given steps for using External Services in flow: 1. Define External Service: Begin by defining an External Service in Salesforce, specifying thedetails of the external endpoint, including the service name, endpoint URL, authenticationrequirements, and method definitions.2. Generate Apex class: Salesforce automatically generates an Apex class based on the definition ofthe External Service, which encapsulates the logic for invoking the external service methods withinyour flow processes.3. Invoke External Service method: Once the External Service is defined and the Apex class isgenerated, you can invoke the methods of the external service directly within your flow using thegenerated Apex class, passing input parameters and handling response data as needed.4. Handle responses: Handle the responses from the external service within your flow processes,performing actions such as parsing response data, error handling, and decision making based onthe outcome of the external service invocation.
Here are the use cases for External Services: Integration with third-party APIs: Integrate with third-party APIs such as payment gateways,mapping services, or social media platforms to perform actions such as processing payments,retrieving location data, or posting to social media.
Custom integration scenarios: Implement custom integration scenarios with external systemsor services that are not directly supported by Salesforce, leveraging External Services to createtailored integration solutions.
Legacy system integration: Integrate with legacy systems or on-premises applications usingExternal Services to modernize and streamline business processes that span across Salesforce andexternal environments.
HTTP callout
HTTP callouts in Salesforce provide a mechanism for invoking external HTTP services or APIs fromwithin your flow processes. This allows you to send HTTP requests to external endpoints, such asRESTful APIs or web services, and handle the responses within your flow. Here are its key features andbenefits: External integration: HTTP callouts enable seamless integration with a wide range of externalsystems and APIs, allowing you to exchange data and trigger actions in external environments fromwithin your flow processes.
Versatility: HTTP callouts support various HTTP methods such as GET, POST, PUT, DELETE,allowing you to perform a wide range of operations, including retrieving data, creating records,updating information, and more.
Asynchronous execution: HTTP callouts are executed asynchronously, ensuring that they do notblock the execution of your flow processes, thereby providing a seamless integration experiencewithout impacting performance.
Using HTTP callout in flow
Follow the given steps for using HTTP callout in flow:

---

## Page 258

1. Create an HTTP request: Begin by creating an HTTP request within your flow using the HTTPRequest element. Specify the HTTP method, endpoint URL, request headers, and any requestbody or parameters required by the external endpoint.2. Send HTTP request: Once the HTTP request is configured, use the Send HTTP Requestelement to send the request to the external endpoint. The flow will asynchronously execute theHTTP callout and continue processing other elements while waiting for the response.3. Handle response: After sending the HTTP request, use the HTTP Response element to handlethe response returned by the external endpoint. You can parse the response data, perform errorhandling, and make decisions based on the outcome of the HTTP callout.
Here are the use cases for HTTP callout: Integration with third-party APIs: Use HTTP callouts to integrate with third-party APIs such asweather services, payment gateways, or social media platforms to retrieve data or trigger actionsbased on external events.
Data synchronization: Synchronize data between Salesforce and external systems by sendingand receiving data via HTTP callouts, ensuring that information is kept up to date across differentenvironments.
Automated processes: Trigger automated processes in external systems by making HTTPcallouts from your flow processes, enabling end-to-end automation of business workflows that spanacross Salesforce and external environments.
Let us follow the given steps for HTTP callout from flow: 1. Create a permission set: 1. For users who want to use HTTP callout. Setup| Permission Set | New | provide details,then Save. Refer to the following figure:
Figure 15.10: Create permission set
2. Assign the permission set to yourself to test the flow.3. Create an external credential: Create external credential from Setup | Named Credentials |External Credentials.4. Create an external credential principle: Click on the New button to create an externalcredential principle. This is required for mapping with permission set later.5. Create a named credential:

---

## Page 259

1. Setup | Named Credentials | New
2. In the URL, paste your end point URL of the API.
6. Map external credential principle and permission set: 1. Map external credential principle with your created permission set.
2. Setup | Permission Sets | select permission set you created | External CredentialPrincipal Access.
7. Salesforce flow using the Create HTTP callout element: 1. Create one Autolaunched flow(No Trigger) in Salesforce to call the API.
2. Add element New Action. It will open a model as shown in Figure 15.11, then select CreateHTTP Callout as shown in Figure 15.12:
Figure 15.11: Action

---

## Page 260

Figure 15.12: Create a new HTTP callout
Conclusion
In the journey of integrating Salesforce flow outside the confines of your Salesforce environment, youhave explored diverse techniques and tools to connect seamlessly with external data sources andservices. From the versatility of external objects and the event-driven nature of outbound messageactions to the standardized integration capabilities of External Services and the direct interactionprovided by HTTP callouts, you now possess a robust set of tools for crafting end-to-end workflows thattranscend Salesforce boundaries.
As businesses continue to evolve, the ability to integrate disparate systems becomes increasinglycrucial. The knowledge gained in this chapter empowers you to not only navigate these integrationchallenges but also to leverage them strategically. By blending the power of Salesforce flow withexternal data and services, you have the capacity to orchestrate sophisticated processes, automateworkflows, and synchronize information seamlessly.
Remember to apply the best practices discussed, from optimizing performance to implementing robusterror handling. This will ensure that your integrations remain reliable, secure, and adaptable to yourbusiness landscape's dynamic demands.
As you move forward, consider the possibilities that these integration techniques unlock. Whetherenhancing customer experiences, streamlining internal processes, or staying ahead in a rapidly changingmarket, Salesforce flow's integration capabilities provide a foundation for innovation and efficiency.
With the knowledge gained from this chapter, you are well positioned to explore, experiment, andarchitect solutions that not only meet today's challenges but also anticipate tomorrow’s integrationneeds. As you embark on your integration journey, may your flow processes seamlessly connect thedots and empower your organization to thrive in the interconnected digital era.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 262

CHAPTER 16Migrating to flow from Workflow and ProcessBuilder
Introduction
In this chapter, we will focus on ensuring the success of your migration by implementing a thoroughtesting strategy for flows after the transition. As you embark on this journey to harness the power ofSalesforce's most advanced automation tool, it is crucial to validate the functionality, reliability, andperformance of your flows to ensure a seamless transition for your organization.
Throughout this chapter, we will provide you with a comprehensive testing strategy designed to coverall aspects of flow functionality, integration, performance, and usability. By following this strategy, youcan identify and address any issues early in the process, resulting in a smoother transition and improveduser experience.
Now, as we approach the final stages of the migration process, it is crucial to focus on testing yourflows to ensure they meet your organization's requirements and expectations. Whether it is unit testingto validate individual flow elements, integration testing to verify interactions
with other Salesforce components or user acceptance testing to gather feedback from end users, eachaspect of the testing strategy plays a vital role in ensuring the success of your migration.
Migrating to a new automation tool can be a complex and challenging process, but with the right testingstrategy in place, you can confidently navigate the transition and unlock Salesforce flow's full potentialfor your organization. So, let us dive in and explore the testing strategy that will guide you towards asuccessful migration and empower you to harness the full power of Salesforce flow.
Structure
This chapter is organized into the following sections: Strategy and plan for automation tool migration
Converting workflow rules to flows
Converting processes to flows
Reviewing the considerations for migration
Testing strategy for flow after migration
Objectives
The objective of this chapter is to equip readers with the knowledge and tools necessary to effectivelytest Salesforce flows after migrating from workflow rules and Process Builder. By emphasizing theimportance of testing in the migration process, this chapter aims to provide a comprehensiveunderstanding of the testing considerations and strategies required to ensure the functionality,

---

## Page 263

reliability, and performance of flows. Through practical insights and best practices, readers will learnhow to conduct thorough unit testing, integration testing, user acceptance testing, and performancetesting to identify and address any issues early in the migration process. Ultimately, the goal is tofacilitate a seamless transition to Salesforce flow, empowering organizations to leverage their advancedautomation capabilities with confidence and efficiency.
Strategy and plan for automation tool migration
As organizations prepare to migrate their automation processes from workflow rules and Process Builderto Salesforce flow, careful planning and strategy are essential to ensure a smooth transition. Thissection will outline key considerations and steps to prepare for the migration, setting the foundation fora successful transition to flow. Let us take a look at them: Understanding the need for migration: The evolution of Salesforce's automation tools, withflow emerging as the most powerful declarative automation tool, has prompted the unification ofdeclarative tools. Salesforce's announcement of retiring workflow rules and Process Builder by 2023signals the need for organizations to migrate their automation processes to flow.
Assessing current automation processes: Before initiating the migration process, reviewingand understanding existing automation processes in Salesforce is crucial. Utilize tools likeLucidchart to visually represent these processes, identifying bottlenecks, dead ends, andopportunities for improvement. Document the entire lifecycle of each process, including the actionsperformed at each stage.
Mapping declarative automation: Map the existing workflow rules and Process Builderprocesses to each stage of the documented business processes. Identify inactive, outdated, orobsolete automation processes that can be updated or removed to reduce technical debt.Determine the context in which new flows will run and plan accordingly.
Planning and designing automation processes: Take time to plan and design the automationprocesses, ensuring alignment with business rules and objectives. Avoid creating new technicaldebt by resisting the urge to immediately start building flows. Utilize tools like Lucidchart to designthe new flows, outlining all necessary information before translating them into flow actions andvariables.
Designing the solution: Consider the end solution and whether multiple flows will be necessary.Avoid a 1-to-1 migration approach, as it can hinder scalability and maintenance. Analyze existingflows to identify elements that can be updated or incorporated into new flows. Explore thepossibility of reusing complex automation processes as subflows and evaluate whether non-automation solutions may be more optimized.
Migration decision logic
When deciding on how and where to migrate workflow rules and processes, consider the followinglogic: Analyze existing automation to determine if it can be incorporated into existing flows or if newflows are needed.
Test the new Salesforce migration tool or build flows from scratch for processes that cannot beincorporated.
Consider scalability, maintenance, and optimization when designing the migration solution.
By following these steps and considerations, organizations can effectively plan and strategize theirautomation tool migration, setting the stage for a successful transition to Salesforce flow. This proactiveapproach will mitigate risks and ensure a smooth migration process, ultimately maximizing the benefitsof Salesforce's advanced automation capabilities.

---

## Page 264

Logic for migration decision
Consider the following guidelines for determining which solution to use when migrating from workflowrules and Process Builder to Salesforce flow: Same record field updates: Workflow rules are commonly used for same record field updates.These updates should be migrated and implemented in before save flows to optimize performanceand avoid recursion risks.
Related record updates and email alerts: If updates to related records or email alerts are sent,the business logic should be implemented in after save flows.
Highly complex automation: For automation with highly complex implementation logic orinvolving multiple loops, high performance batch processing is required. In these cases, acombination of flow and invocable Apex should be used to efficiently handle complex calculations.
Scheduled actions and multiple record updates: Processes requiring scheduled actions ormultiple record updates should utilize a scheduled path in flow. Additionally, adjusting the batchsize can help avoid hitting per transaction Apex limits.
Branching logic and subflows: If the process involves branching logic, introducing subflows foreach process and using a master flow to invoke them can be an effective approach. By followingthis logic and considering the specific requirements of each automation process, organizations canmake informed decisions on how to migrate their workflow rules and Process Builder processes toSalesforce flow. This approach ensures that the migration is optimized for performance, scalability,and efficiency, ultimately maximizing the benefits of Salesforce's advanced automation capabilities.
Converting workflow rules to flows
External objects in Salesforce provide a powerful way to access and interact with data stored. Asorganizations transition from workflow rules to Salesforce flow, the Migrate to flow tool provides aseamless and intuitive solution for migrating existing processes. This tool, available in both sandbox andproduction environments, simplifies the migration process and allows for thorough testing in a sandboxenvironment before deploying changes to production.
Using the Migrate to flow tool
To access the Migrate to flow tool, navigate to the Setup menu and search for it. Once accessed, thetool presents a list of all workflow rules, allowing administrators to select the desired rule for migration.Upon selection, the tool facilitates the creation of a corresponding flow, which is initially inactive.Administrators can preview the flow before activation, ensuring accuracy and completeness. Uponactivation, the new flow becomes active, seamlessly replacing the workflow rule.
Example
Consider a workflow rule that updates the account owner based on specific criteria, such as the accounttype or industry. The Migrate to flow tool can translate this process into a clear and easilyunderstandable flow.
Comparison
The original workflow rule may have consisted of multiple actions triggered by similar conditions.However, Decision elements can combine these actions into a single flow. For example, supposemultiple workflow rules are responsible for updating different fields on the account record based onspecific criteria. By consolidating these actions into a single flow, triggered after the account is updated,administrators can streamline the automation process and eliminate the need for multiple workflowrules. The flow can incorporate Decision elements to determine the appropriate field updates based onspecific criteria, simplifying the automation process and enhancing efficiency.

---

## Page 265

Benefits of migration
The migration from workflow rules to flows offers several benefits, including improved clarity, enhancedfunctionality, and simplified maintenance. Flows provide a clearer and more intuitive representation ofautomation processes compared to workflow rules, making it easier for administrators to understandand manage. Additionally, flows offer enhanced functionality, allowing for more complex automationlogic and integration with other Salesforce features. By consolidating multiple workflow rules into asingle flow, organizations can reduce clutter and streamline their automation processes, improvingefficiency and productivity.
In summary, the Migrate to flow tool simplifies the transition from workflow rules to Salesforce flow,offering organizations a seamless and efficient solution for migrating existing processes. By leveragingthis tool, organizations can harness Salesforce flow's full potential to streamline their automationprocesses and drive business success.
Converting processes to flows
Transitioning processes to flow in Salesforce involves careful planning and execution to ensure a smoothmigration. Although Salesforce has yet to provide a dedicated migration tool, we can still efficientlymigrate processes using flow's capabilities.
Understanding the migration process
When migrating processes to flow, we need to consider each process's unique requirements anddetermine the best migration approach. While some processes may be straightforward to migrate,others with complex actions or decision points may require more careful planning.
Let us consider a scenario in which we have a process for managing employee performance reviews.This process involves multiple steps, including setting performance goals, conducting reviews, andproviding employee feedback.
Migration strategy
To migrate this process to flow, we will break down each step and identify the corresponding actionswithin the flow. We will then create a new flow in Salesforce and replicate each step of the processusing flow elements like record updates, email alerts, and Decision elements.
For example, we will use record update elements to set performance goals and provide feedback, andemail alert elements to notify employees and managers about upcoming reviews.
Benefits of migration
Migrating processes to flow offers several benefits. Flows provide a more visual and intuitive way torepresent automation processes, making it easier for administrators to understand and manage them.Additionally, flows offer enhanced functionality and flexibility, allowing for more complex automationlogic and integration with other Salesforce features.
Reviewing the considerations for migration
Before diving into the migration process, reviewing and considering various factors is crucial to ensure asuccessful transition from your current automation tools to Salesforce flow. Let us explore some keyconsiderations to keep in mind during the migration process: Current automation setup: Take stock of your existing automation setup, including workflowrules and Process Builder configurations. Understand each automation process's complexity,dependencies, and performance to determine the best migration approach.
Business processes and rules: Review your organization's business processes and rulescorresponding to the automation processes in Salesforce. Ensure alignment between your

---

## Page 266

automation solutions and business objectives to avoid disruption during the migration.
Technical debt and optimization: Assess the technical debt accumulated in your currentautomation setup. Identify opportunities to optimize and streamline your processes during themigration to flow, improving efficiency and performance in the long run.
Impact on users and operations: Consider the impact of migration on end users and day-to-dayoperations. Communicate changes effectively to stakeholders and provide training and support asneeded to ensure a smooth transition.
Testing and validation: Develop a comprehensive testing strategy to validate the functionalityand performance of migrated processes in a sandbox environment. Conduct thorough testing toidentify and address any issues before deploying changes to production.
Data integrity and security: Ensure data integrity and security throughout the migrationprocess. Review data access permissions and configurations to prevent unauthorized access or dataloss during the migration.
Subflows consideration: Consider incorporating subflows into your migration strategy. Subflowsare a convenient way to handle separate business processes, making them easier to maintain andupdate. They also help build reusable automation processes, improving efficiency and reducingredundancy. However, be mindful of their limitations, such as not being available in record-triggeredbefore save flows and potential debugging challenges.
Documentation and knowledge transfer: Document the migration process, including anychanges made to automation configurations and workflows. Provide training and knowledgetransfer sessions to empower users and administrators to effectively manage the new automationsetup.
Feedback and continuous improvement: Solicit feedback from users and stakeholders duringand after the migration process. Use feedback to identify areas for improvement and iterate onyour automation solutions to better meet the needs of your organization.
By carefully reviewing and addressing these considerations proactively, you can ensure a smooth andsuccessful migration from your current automation tools to Salesforce flow. This strategic approach willhelp minimize disruption, maximize efficiency, and unlock the full potential of Salesforce's powerfulautomation capabilities.
Testing strategy for flow after migration
After migrating your automation processes to Salesforce flow, thorough testing is essential to ensure thefunctionality and performance of the migrated flows. A robust testing strategy will help identify anyissues or discrepancies and ensure a smooth transition to the new automation solution. Let us outline acomprehensive testing strategy for flow after migration: Current automation setup: Take stock of your existing automation setup, including workflowrules and Process Builder configurations. Understand each automation process's complexity,dependencies, and performance to determine the best migration approach.
Business processes and rules: Review your organization's business processes and rulescorresponding to the automation processes in Salesforce. Ensure alignment between yourautomation solutions and business objectives to avoid disruption during the migration.
Technical debt and optimization: Assess the technical debt accumulated in your currentautomation setup. Identify opportunities to optimize and streamline your processes during themigration to flow, improving efficiency and performance in the long run.
Impact on users and operations: Consider the impact of migration on end users and day-to-dayoperations. Communicate changes effectively to stakeholders and provide training and support asneeded to ensure a smooth transition.

---

## Page 267

Testing and validation: Develop a comprehensive testing strategy to validate the functionalityand performance of migrated processes in a sandbox environment. Conduct thorough testing toidentify and address any issues before deploying changes to production.
Data integrity and security: Ensure data integrity and security throughout the migrationprocess. Review data access permissions and configurations to prevent unauthorized access or dataloss during the migration.
Additional considerations for flow migration: Embrace flow as the future: Recognize that flow is the future of Salesforce automation. Getfamiliar and comfortable with building flows to prepare for upcoming changes.
Enhancements for flow migration: Add fault paths, unit tests, debug logs, and dynamicsolutions to enhance flow functionality and reliability.
Continuous improvement and feedback: Seek feedback and continuously improve yourprocesses. Share your experiences and plans for migration to engage with other Salesforceprofessionals.
Conclusion
This chapter has provided valuable insights into the importance of testing from workflow rules andProcess Builder to Salesforce flow in the migration process. We have emphasized the critical role thattesting plays in ensuring the functionality, reliability, and performance of flows after migration andoutlined a comprehensive testing strategy to guide readers through this process.
By following the testing strategy outlined in this chapter, organizations can identify and address anyissues early in the migration process, resulting in a smoother transition and improved user experience.Through thorough unit testing, integration testing, user acceptance testing, and performance testing,organizations can validate the functionality and reliability of their flows, ultimately empowering them toleverage the full potential of Salesforce's advanced automation tool.
As organizations navigate the transition to Salesforce flow, it is essential to prioritize testing to mitigaterisks and ensure a successful migration. By incorporating testing into the migration process,organizations can minimize disruption to business operations and optimize the utilization of Salesforce'smost powerful automation tool.
In conclusion, thorough testing is key to a successful migration to Salesforce flow. By following thestrategies outlined in this chapter, organizations can confidently embrace the transition and unlock thefull potential of their automation processes.
Additionally, as organizations continue to explore advanced automation options in Salesforce, it isimportant to consider the use cases where Apex triggers may be necessary. In the next chapter, readerswill delve into the comparison between flow and Apex triggers, learn the basics of Apex triggers,understand their context variables, and explore how to automate complex processes using Apextriggers. The chapter will also cover best practices for Apex triggers, strategies for handling bulkoperations, and ways to combine the power of flow and Apex triggers for enhanced automationcapabilities.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 268

CHAPTER 17Hands-on Apex Triggers for Automation
Introduction
Welcome to the final chapter of the book. Throughout this book, we have explored various tools andtechniques for automating processes within the Salesforce platform, from the user-friendly declarativecapabilities of Salesforce flow to the powerful programmatic capabilities of Apex.
In this concluding chapter, we will shift our focus to Apex triggers, a cornerstone of Salesforceautomation that offers unparalleled flexibility and control in executing complex business logic. We willdelve into the fundamentals of Apex triggers, explore best practices for their implementation, and learnhow to leverage them alongside Salesforce flow to create comprehensive automation solutions.
Structure
This chapter is organized into the following sections: Flow versus Apex trigger
Apex trigger basics
Apex trigger context variables
Automate using Apex trigger
Bulkify the Apex trigger
Best practices for the Apex trigger
Combine the power of flow and Apex trigger
Objectives
In this concluding chapter, our objective is to provide you with a holistic understanding of Apex triggersand their indispensable role in Salesforce automation. We aspire to guide you through the foundationalprinciples of Apex triggers, elucidating their usage, nuances, and best practices. Moreover, we endeavorto demonstrate how Apex triggers can seamlessly integrate with Salesforce flow, facilitating the creationof robust and comprehensive automation solutions. By the culmination of this chapter, our goal is foryou to emerge equipped with the knowledge and proficiency to adeptly implement Apex triggers in yourSalesforce Org. Armed with this expertise, you will be empowered to automate processes with precision,efficiency, and agility, thereby driving transformative outcomes within your organization. As we embarkon this enlightening journey into the realm of Apex triggers, let us unlock the boundless potential ofSalesforce automation together.
Flow versus Apex trigger
In the previous chapters, we have explored the power of Salesforce flows and how they enable us toautomate processes visually without writing code. Now, let us delve into how flows compare to another

---

## Page 269

powerful automation tool in Salesforce: Apex triggers.
You are already familiar with flows and how they allow you to create automation processes using avisual interface. Flows are fantastic for automating straightforward tasks like updating fields, sendingemails, or guiding users through a series of steps.
With flows, you can easily create complex workflows by connecting different elements like screens,decisions, and actions. They are ideal for scenarios where you want to automate a process withoutdiving into code, making them accessible to a wide range of users, from admins to business analysts.
Now, let us talk about Apex triggers. Unlike flows, which are built using a visual interface, Apex triggersare blocks of code that execute in response to specific events in Salesforce, such as record creation,update, or deletion.
Apex triggers offer more flexibility and control over your automation logic than flows. With Apextriggers, you can perform complex calculations, query related records, and interact with externalsystems using code. They are perfect for handling advanced scenarios that require custom businesslogic or integration with external systems.
Choosing between flows and Apex triggers
So, when should you use flows, and when should you use Apex triggers? It all comes down to thecomplexity of the task and your comfort level with code. Flows: Stick with flows for automating straightforward processes that can be easily visualized andimplemented using a drag and drop interface. Flows are great for scenarios where you want toautomate a process quickly without writing code.
Apex triggers: Consider using Apex triggers for more complex scenarios that require custombusiness logic, data manipulation, or integration with external systems. If you are comfortablewriting code and need more control over your automation logic, Apex triggers might be the betteroption.
Following are some cases when you can consider using flow or Apex trigger: Same-record field updates:
Flow: Before-save flow trigger: Available and recommended for same-record field updatesdue to better performance compared to after-save triggers.
After-save flow trigger: Not ideal for same-record field updates due to performanceconsiderations. Apex: Apex triggers: Available and recommended for same-record field updates ifperformance is a concern.
High performance batch processing: Flow: Not ideal for high-performance batch processing.
Apex: Apex triggers: Available and recommended for high performance batch processing dueto Apex's configurability and rich debug capabilities.
Cross-object CRUD: Flow: Before-save and after-save flow triggers: Not available for cross-object CRUDoperations.
Apex: Apex triggers: Available and recommended for cross-object CRUD operations.
Asynchronous processing: Flow: After-save flow trigger: Available and recommended for asynchronous processing.

---

## Page 270

Apex: Apex triggers: Available and recommended for asynchronous processing with morecontrol over callouts and error handling.
Complex list processing: Flow: Not ideal for complex list processing.
Apex: Apex triggers: Available and recommended for complex list processing due to flow'slimitations in handling lists.
Custom validation errors: Flow: Available for custom validation errors.
Apex: Apex triggers: Available and recommended for handling custom validation errors untilflow supports addError() method directly.
When deciding between flow and Apex triggers for triggered automation on the Salesforce platform, it iscrucial to consider factors such as performance, maintainability, and complexity. Flow is ideal for simpleruse cases, offering ease of maintenance and debugging, making it suitable for teams with mixed oradmin-heavy skill sets. On the other hand, Apex triggers excel in handling complex scenarios requiringhigh performance, sophisticated logic, or specific functionalities like cross-object CRUD operations orcomplex list processing. Your decision should be guided by the specific use case, team skill sets, andperformance requirements to ensure the best approach for your automation needs.
Apex trigger basics
Apex triggers serve as the backbone of Salesforce automation, enabling developers to implementcustom business logic and automate processes in response to various events. These events, known astrigger events, can occur before or after a database operation (such as insert, update, or delete) on arecord. Apex triggers allow developers to perform custom actions and business logic before or afterthese database operations, providing high flexibility and control over the platform's behaviour.
To summarise, Apex code can be invoked automatically by using Apex triggers. Apex triggers enableyou to perform custom actions before or after changes to Salesforce records, such as insertions,updates, or deletions.
A trigger is Apex code that executes before or after the following types of operations: Insert
Update
Delete
Merge
Upsert
Undelete
Types of Apex triggers
There are two main types of Apex triggers based on when they execute in relation to the databaseoperation: Before triggers: Before triggers execute before the database operation is performed. They arecommonly used to update or validate record values before they are saved to the database. Beforetriggers are ideal for enforcing data integrity and applying business rules before data is committedto the database.
After triggers: After triggers execute after the database operation has been completed and thechanges are committed to the database. They are used to access field values that are set by the

---

## Page 271

system (such as a record's Id or LastModifiedDate field) and to perform additional actions basedon the changes made to records. After triggers are often used for tasks such as sendingnotifications, logging changes, or updating related records.
Key considerations for Apex triggers
Let us take a look at the key considerations for Apex triggers: Governor limits: Apex triggers are subject to Salesforce's governor limits, which imposeconstraints on resource usage, such as CPU time, heap size, and DML statements. It is important todesign triggers with these limits in mind to ensure efficient and reliable execution.
Bulk processing: Apex triggers should be designed to handle bulk processing of recordsefficiently. This involves writing trigger logic that can process multiple records at once to minimizethe impact on performance and avoid hitting governor limits.
Error handling: Proper error handling is crucial in Apex triggers to ensure robustness andmaintain data integrity. Developers should implement error handling mechanisms, such as try-catchblocks, to gracefully handle exceptions and provide users with meaningful error messages.
Let us consider a simple use case where we want to automatically update the Description field on theAccount object whenever a new Contact is created. The Description field should be updated with astatic value (for simple demo) indicating that it is updated based on Contact:
trigger AccountTrigger on Contact (after insert) {
    AccountTriggerHandler.handleContactUpdate(Trigger.new);
}
Let us understand the above simple code: 
trigger AccountTrigger on Contact (after insert) {:
This line declares an Apex trigger named AccountTrigger that fires after new Contact recordsare inserted.
AccountTriggerHandler.handleContactsUpdate(Trigger.new);:
This line calls the handleContactsUpdate method from the AccountTrigger Handler class, passing in
Trigger.new, which represents the list of new Contact records that caused the trigger to fire.
To better organize our code, we are using a trigger handler class called AccountTriggerHandler. Thishandler class contains the logic to perform updates to the Account records based on changes in Contactrecords. Using a separate handler class like this is considered a best practice in Salesforce developmentbecause it keeps the trigger code simple, promotes reusability, and makes the logic easier to test andmaintain.
In the AccountTriggerHandler, we define a method named handleContactUpdate. This method performsthe actual work of gathering the Account records related to the newly inserted Contact records andupdating their Description fields:
public class AccountTriggerHandler {
    public static void handleContactUpdate(List<Contact> lstContacts) {
        //Initialize a set to store unique Account IDs related to the Contacts being processed
        Set<Id> setAccountIds = new Set<Id>();
 
        //Collect Account IDs from the new Contacts

---

## Page 272

for (Contact con : lstContacts) {
            setAccountIds.add(con.Account.Id); // Add each Contact's Account ID to the set
        }
 
        // Query for related Accounts based on the collected Account IDs and update the Description field
        List<Account> lstAccountsToUpdate = [SELECT Id, Description FROM Account WHERE Id IN :setAccountIds];
 
        // Loop through the queried Accounts
        for(Account acc : lstAccountsToUpdate) {
            acc.Description = 'Updated Description based on Contacts'; // Set a static value just for a demo for the Description field
        }
        // Update the Account records with modified Description field values
        update lstAccountsToUpdate;
    }
}
Let us understand this in detail: 
public class AccountTriggerHandler {:
This line declares a public class named AccountTriggerHandler.
public static void handleContactsUpdate(List<Contact> lstContacts) {:
This line declares a public, static method named handleContactsUpdate that takes a list of
Contacts (lstContacts) as input.
Set<Id> setAccountIds = new Set<Id>();:
This line initializes a set (setAccountIds) to store unique Account IDs related to the Contactsbeing processed.
for (Contact con : lstContacts) { setAccountIds.add(con.AccountId); }:
This loop iterates over each Contact in the input list (lstContacts) and adds its Account ID tothe setAccountIds set.
List<Account> lstAccountsToUpdate = [SELECT Id, Description FROM Account WHERE Id IN :setAccountIds];:
This SOQL query retrieves the related Accounts based on the collected Account IDs in the
setAccountIds set. It selects the Account ID and Description fields.
for (Account acc : lstAccountsToUpdate) { acc.Description = 'Updated Description based on Contacts'; }:
This loop iterates over the queried Accounts (lstAccountsToUpdate) and sets a static value forthe Description field of each Account.
update lstAccountsToUpdate;:
This statement updates the Account records with the modified Description field values.
This class provides a reusable method (handleContactsUpdate) to update the Description field ofrelated Accounts based on newly inserted Contacts.

---

## Page 273

Apex trigger context variables
Apex triggers execute in various contexts, depending on the trigger event type and the point in thetransaction lifecycle. The context in which a trigger executes determines developers' available behaviorand capabilities within the trigger logic. Trigger context variables serve as conduits for accessinginformation about the trigger event and manipulating records accordingly.
Types of Apex trigger context variables
Salesforce provides a comprehensive list of context variables available for triggers, each serving aspecific purpose in trigger execution. Let us delve into these context variables, as outlined in the officialSalesforce documentation: 
isExecuting: Returns true if the current context for the Apex code is a trigger, not a Visualforce page, aweb service, or an executeanonymous() API call.
isInsert, isUpdate, isDelete: Return true if the trigger was fired due to an insert, update, or deleteoperation, respectively, from various sources such as the Salesforce user interface, Apex, or theAPI.
isBefore, isAfter: Return true if the trigger was fired before or after any record was saved, respectively.
isUndelete: Returns true if the trigger was fired after a record is recovered from the Recycle Bin,following an undelete operation from the Salesforce user interface, Apex, or the API.
new, newMap: Provide access to the new versions of the sObject records. The new context variablereturns a list of new versions, while the newMap context variable returns a map of IDs to new versionsavailable in specific trigger contexts.
old, oldMap: Provide access to the old versions of the sObject records. The old context variable returnsa list of old versions, while the oldMap context variable returns a map of IDs to old versions availablein specific trigger contexts.
operationType: Returns an enum of type System.TriggerOperation corresponding to the current operation,facilitating programming logic variation based on different trigger types.
size: Represents the total number of records in a trigger invocation, encompassing both old andnew records.
Here are some context variable considerations: 
trigger.new and trigger.old cannot be used in Apex DML operations.
You can use an object to change its own field values using trigger.new, but only in before triggers.
In all after triggers, trigger.new is not saved, so a runtime exception is thrown.
trigger.old is always read-only.
You cannot delete trigger.new.
Automate using Apex trigger
In Salesforce development, automation is key to driving efficiency and maximizing productivity. WhileSalesforce offers a range of declarative automation tools, complex business requirements sometimesdemand a more tailored approach. This is where Apex triggers come into play, enabling developers toautomate processes and execute custom logic based on specific events within the Salesforce platform.
Apex triggers serve as the backbone of automation in Salesforce, allowing developers to respond todatabase events such as record insertions, updates, deletions, and more. By writing Apex triggers,developers can enforce business rules, perform calculations, update related records, and integrate withexternal systems seamlessly. This level of customization ensures that organizations can automate eventhe most intricate business processes to meet their unique requirements.

---

## Page 274

Choosing Apex triggers for automation
While Salesforce provides powerful declarative automation tools like Process Builder and workflow rules,their capabilities are limited, especially when dealing with complex scenarios or external integrations.Apex triggers offer a higher degree of control and flexibility, allowing developers to execute customlogic, interact with multiple records, and integrate with external systems using Apex code. This makesthem the preferred choice for automating intricate business processes beyond declarative tools’capabilities.
For example, imagine a telecommunications company that integrates with an external service to verifyaddresses for new customers. The process involves making an API callout to a third-party service,passing customer address details in JSON format, and receiving a response containing the verifiedaddress details in JSON format.
However, the response from the third-party service is complex and includes various fields such as streetaddress, city, state, ZIP code, latitude, longitude, and additional metadata. The telecommunicationscompany needs to parse this JSON response, extract relevant address details, and update the customerrecords in Salesforce with the verified address information.
The challenge here is that the JSON response structure may change over time due to updates orchanges in the third-party service, making it difficult to handle dynamically within Salesforce flow.Additionally, the company requires real-time processing of address verification to ensure accuratecustomer data.
In this scenario, using an Apex trigger would be beneficial due to its flexibility in handling complex JSONparsing and dynamic processing requirements. With Apex, developers can write custom code to parsethe JSON response, extract relevant address details, and update the customer records accordingly. Apextriggers provide the necessary control and customization to handle complex business logic and ensurereal-time processing of address verification for new customers.
Bulkify the Apex trigger
In Salesforce development, optimizing code for bulk data operations is essential for maintainingperformance and scalability. When dealing with large volumes of records, inefficient code can lead toperformance issues and governor limit errors. Bulkifying Apex triggers is a crucial technique thatensures trigger logic efficiently handles multiple records in a single transaction, thereby improvingperformance and preventing governor limit exceptions. Let us delve into the importance of bulkificationand explore strategies for implementing it in Apex triggers.
Understanding bulk data operations
Bulk data operations in Salesforce involve the manipulation of multiple records in a single transaction.These operations, such as inserting, updating, or deleting large numbers of records, are common indata-intensive applications and integrations. When writing Apex triggers, it is crucial to optimize thetrigger logic to handle bulk data operations efficiently, ensuring that the code performs well undervarious load conditions.
Non-bulkified Apex triggers are prone to performance issues and governor limit errors when dealingwith large datasets. For example, if trigger logic queries records inside a loop or performs DMLoperations within a loop, it can result in hitting governor limits such as SOQL query limits, CPU timelimits, or DML statement limits. These limitations can impact the application's performance andscalability, leading to degraded user experience and potential system failures.
Strategies for bulkification
Bulkifying Apex triggers involve refactoring trigger logic to efficiently handle collections of recordsinstead of processing them one by one. Here are some strategies for bulkifying Apex triggers:

---

## Page 275

Bulk querying records: Instead of querying records inside a loop, bulkify trigger logic byquerying records outside the loop and using collections to store query results. This reduces thenumber of SOQL queries executed and improves performance.
Bulk processing records: Process collections of records in bulk to minimize DML operations. Usecollections such as lists or maps to store records and perform DML operations outside the loop toprocess multiple records in a single transaction.
Use of maps for record lookups: Use maps to store related records and perform lookups basedon record IDs. This eliminates the need for nested loops and improves performance by reducing thenumber of iterations.
Avoid nested loops: Refactor trigger logic to eliminate nested loops, which can result in quadratictime complexity and impact performance, especially with large datasets.
Test with bulk data: Test trigger logic with bulk datasets to ensure that it performs efficientlyunder various load conditions and does not exceed governor limits.
Let us consider a scenario where we want to update a custom field on the Account object based on thetotal number of associated Contacts. We can bulkify the trigger logic to handle large volumes of Account-Contact relationships efficiently, as shown:
trigger ContactTrigger on Contact (after insert, after update, after delete) {
    if(Trigger.isAfter) {
        if(Trigger.isInsert || Trigger.isUpdate) {
            ContactTriggerHandler.handleContacts(Trigger.new);
        }
    }
}
public class ContactTriggerHandler {
    public static void handleContacts(List<Contact> lstNewContacts) {
        Set<Id> setAccountIds = new Set<Id>();
        // Collect Account IDs from the affected Contacts
        for(Contact con : lstNewContacts) {
            setAccountIds.add(con.AccountId);
        }
        // Query for related Accounts and update custom field
        List<Account> lstAccountsToUpdate = [SELECT Id, Contact_Count__c,  (SELECT Id FROM Contacts) FROM Account WHERE Id IN :setAccountIds];
        for(Account acc : lstAccountsToUpdate) {
            acc.Contact_Count__c = acc.Contacts.size();
        }
        //update the Account records
        update lstAccountsToUpdate;
    }
}

---

## Page 276

Let us take a closer look at how the trigger and handler code efficiently handle a large amount of data,a concept known as bulkification: Bulk data processing: The ContactTrigger trigger efficiently processes bulk data by accepting a listof Contact records (List<Contact>) as input in the ContactTriggerHandler handler class. This trigger runsafter records are inserted, updated, or deleted (after insert, after update, after delete), enabling itto handle multiple Contact records simultaneously.
Query optimization: The trigger collects Account IDs from the inserted or updated Contacts andthen queries for related Accounts. By using a set to store the Account IDs (Set<Id>), duplicateAccount IDs are automatically handled, ensuring that each Account is only queried once, even if itis associated with multiple Contacts.
Querying related records: The trigger queries related Accounts (List<Account>) using the IN clausewith the set of Account IDs. This approach optimizes the SOQL query by fetching all relevantAccounts in a single query, rather than querying within a loop for each Contact, which would resultin inefficient, repetitive queries.
Efficient data processing: The handler ContactTriggerHandler processes the list of new Contacts(List<Contact>) passed from the trigger. It iterates over this list once to collect unique Account IDswithout duplication, ensuring efficient processing.
Handling multiple records: The trigger and handler are designed to handle multiple Contactrecords simultaneously. They efficiently process each record within the provided collection,updating the Contact_Count__c field for each associated Account based on the total number of Contactsrelated to that Account.
Single DML operation: After updating the Contact_Count__c field for each relevant Account, thehandler performs a single DML operation (update lstAccountsToUpdate;) to update all modified Accountrecords. This bulk DML operation minimizes the number of database transactions, contributing tooverall performance optimization.
In summary, above trigger and handler logic is bulkified to efficiently handle large volumes of Account-Contact relationships by optimizing queries, processing data in bulk, and minimizing databasetransactions. This approach ensures scalability and performance when processing multiple Contactrecords simultaneously.
Best practices for the Apex trigger
In the world of Salesforce development, Apex triggers are indispensable tools for automating businessprocesses and executing custom logic. However, to maximize their effectiveness and maintainability,developers must adhere to a set of best practices tailored to optimize trigger performance andscalability. Let us take a look at some of them: Bulkification: Bulkify trigger logic to efficiently handle large volumes of records in a singletransaction. Add records to collections and perform DML operations against them to minimize thenumber of DML operations.
Governor limits awareness: Stay mindful of Salesforce governor limits and utilize the LimitsApex Methods to monitor resource consumption. Minimize the number of SOQL queries and DMLstatements to prevent hitting governor limits and ensure efficient trigger execution.
Query optimization: Optimize SOQL queries by preprocessing records and generating sets, whichcan be used in single SOQL statements with the IN clause. This reduces the number of queriesexecuted and improves query performance.
One trigger per object: Stick to the principle of using only one trigger per object to maintainclarity and organization in trigger logic, as shown in the sample code. Multiple triggers on the sameobject can lead to complexity and difficulty in managing trigger behaviour.

---

## Page 277

The following example demonstrates a single trigger on the Lead object that managesmultiple events in one place:
trigger LeadTrigger on Lead (before insert, after insert, before update, after update, before delete, after delete, after undelete) {
    if(Trigger.isBefore) {
        if(Trigger.isInsert) {
            // Before insert
        }
        else if(Trigger.IsUpdate) {
            //Before Update
        }
        else {
            // Before Delete
        }
    }
    else {
        // Is After
        if(Trigger.isInsert) {
            // After Insert
        }
        else if(Trigger.IsUpdate) {
            // After Update
        }
        else if(Trigger.isDelete) {
            // After Delete
        }
        else {
            // After Undelete
        }
    }
}
Bulkify helper methods: Ensure that helper methods used within triggers are bulkified to handlecollections of records efficiently. Reuse code and methods to avoid redundancy and improvemaintainability.
Logic separation: Keep trigger logic minimal by separating business logic into helper classes ortrigger frameworks. This promotes code reusability, simplifies maintenance, and adheres to theSeparation of Concerns principle.
Avoid nesting loops: Refrain from nesting loops within loops as it can lead to quadratic timecomplexity and impact performance, especially with large datasets. Use bulk processing techniques

---

## Page 278

to handle records collections efficiently.
Asynchronous callouts: If making callouts from triggers, use future methods annotated with
@future(callout=true) to execute the callout asynchronously. This prevents blocking the triggerexecution and ensures smooth performance.
Batch Apex for large data volumes: Consider using batch Apex for processing large volumes ofdata in chunks. Batch Apex allows for efficient processing of large datasets while avoiding governorlimit issues.
Handle trigger recursion: Prevent trigger recursion by ensuring that triggers are executed onlyonce per transaction. As shown in class CheckRecursive below, static Boolean variables in Apexclasses are used to control trigger execution and avoid recursive calls.
public class CheckRecursive {
    public static Boolean firstCall = false;
}
trigger ContactTrigger on contact (after update) { 
    if(!CheckRecursive.firstCall) {
        CheckRecursive.firstCall = true;
        // Call your Handler method here
    }
}
Temporarily disabling triggers: For data loading scenarios, temporarily disable triggers to speedup the process. Create a custom setting and a corresponding checkbox field to control when atrigger should fire, and include logic in the trigger code to respect this setting, as shown in thefollowing code:
trigger LeadTrigger on Lead (before insert) {
    DataLoad_Setting__c objSetting = DataLoad_Setting__c.getInstance(UserInfo.getUserId());
    if(objSetting.LargeData_Load__c) return; //Skip Trigger
    LeadTriggerHandler.beforeInsert(Trigger.New);
}
For developers immersed in Salesforce, the Apex Recipes library is a goldmine of practical examples.These concise and clear code snippets cater to various tasks while adhering to best practices. Whetheryou are a seasoned developer or just starting out, these examples are accessible athttps://github.com/trailheadapps/apex-recipes, and they offer valuable insights into real-worldsolutions. Delve into this resource to enhance your understanding of industry-standard approaches,keeping your code clear and concise. Refer to the table of contents for easy navigation and considerusing the Salesforce CLI and a scratch org for the initial deployment. The use of Apex Recipes willundoubtedly elevate your skills, contribute to the success of your Salesforce projects, and ensureefficient, scalable, and maintainable solutions that adhere to Salesforce best practices and governancestandards.
Combine the power of flow and Apex trigger
Salesforce flow and Apex triggers are two powerful tools used for automating processes in Salesforce.They create a potent combination that can handle a wide range of automation scenarios when usedtogether. Let us explore how flow and Apex trigger work together to enhance automation:

---

## Page 279

Declarative power of flow: Salesforce flow is a user friendly tool that allows users to automate processes without writingcode.
With flow, users can design workflows, automate business processes, and guide users throughcomplex processes using a visual interface.
Programmatic flexibility of Apex trigger: Apex triggers provide developers with the flexibility to execute custom logic before or afterdatabase operations.
Developers can use Apex trigger to enforce business rules, perform calculations, and integratewith external systems using code.
Synergy between flow and Apex trigger: Flow and Apex trigger can complement each other to handle complex automation scenarios.
Record-triggered flow can be cause of executing an Apex trigger, which can then executecustom logic, interact with external systems, and update records accordingly.
Let us imagine a scenario where a company wants to automate the process of assigning leads to salesrepresentatives based on predefined criteria.
Flow can gather lead information and initiate the assignment process, while an Apex trigger can handlethe assignment logic and update the lead records accordingly.
The benefits of combining flow and Apex trigger are as follows: Seamless integration: flow and Apex trigger can work together seamlessly to achieveautomation goals.
Increased flexibility: Combining flow and Apex trigger provides both declarative andprogrammatic options to handle complex automation requirements.
By understanding how to combine the power of flow and Apex trigger, you can create efficient andflexible automation solutions tailored to their specific business needs.
Conclusion
In this chapter, we explored Salesforce automation through Apex triggers. We began by understandingthe fundamental differences between Salesforce flow and Apex triggers, recognizing the scenarioswhere each excels and how they can complement each other to create robust automation solutions.
We then explored the basics of Apex triggers, exploring their structure, context variables, and role inautomating various operations such as data manipulation and integration. Through practical examplesand explanations, we gained insights into how Apex triggers can enhance business processes withinSalesforce.
As we delved deeper, we uncovered best practices for designing, implementing, and optimizing Apextriggers. From bulkifying triggers to handling recursion and governor limits, we learned how to ensureefficient and scalable automation solutions that adhere to Salesforce best practices.
Furthermore, we explored the synergy between flow and Apex triggers, witnessing how their combinedpower can streamline complex processes and improve operational efficiency.
Through a real-world example of lead assignment automation, we witnessed firsthand thetransformative impact of integrating flow and Apex triggers in automating critical business workflows.
Armed with this knowledge, you are now equipped to embark on your own journey of Salesforceautomation using Salesforce flow and Apex triggers. Whether it is optimizing existing processes or

---

## Page 280

building new automation solutions, the possibilities are endless with the combined power of Salesforceflow and Apex triggers.
As you continue to explore and implement automation solutions in Salesforce, remember to stay curiousand always be learning, experiment with new techniques, always strive for efficiency and scalability inyour designs, and be a trailblazer to inspire many more.
Join our book’s Discord spaceJoin the book's Discord Workspace for Latest updates, Offers, Tech happenings around the world, NewRelease and Sessions with the Authors:
https://discord.bpbonline.com

---

## Page 281

Index
A
Apex 217
Apex Action 214
Apex Action, challenges 216
Apex Action, executing 223, 224
Apex Action, limits 216
Apex Action, situations 215, 216
Apex, classes
collections 219
if-else 218
loops 218
variables 218
Apex Collections, types
list 219
map 219
set 219
Apex, key features
execution 217
integration 217
object oriented 217
syntax 217
Apex, methods
class, declaration 220
class, instantiation 220
debug log 220
method, declaration 220
method, invocation 220
Apex Trigger 298
Apex Trigger, architectures 300
Apex Trigger, automating 304, 305
Apex trigger, best practices 308-310
Apex Trigger, cases 299
Apex Trigger, complexity 299
Apex Trigger Context Variables 303
Apex Trigger Context Variables, types 303
Apex Trigger, key
bulk, processing 301
error, handling 301
governor, limits 301
Apex Trigger, operations 300
Apex Trigger, types
after 301
before 300
Assignment Element 29
Autolaunched Flow 171
Autolaunched Flow, advantages 176
Autolaunched Flow, challenges
compliance, ensuring 171

---

## Page 282

dynamic, environments 171
efficient user, managing 171
repetitive tasks 171
Autolaunched Flow, characteristics
external system, integrating 188
manual, initiation 188
record, independence 188
Autolaunched Flow, considering
error, handling 186
flow, designing 186
query criteria 186
Autolaunched Flow, guidelines
paper-based, planning 172
pre-construction, analyzing 172
user decision points, considering 172
Autolaunched Flow, key points
account, query 186
flow, invocation 186
parameter map, creating 185
Autolaunched Flow, scenarios 172
Autolaunched Flow, steps 172-175
Autolaunched Flow, use cases
dynamic responses 171
efficient user, cleanup 171
multi-flow operations, streamlining 171
seamless actions 171
Automation 3
Automation, benefits
accuracy, improving 3
competitive, advantage 3
cost, saving 3
efficiency, increasing 3
scalability 3
Automation, importance 2
Automation, scenarios
customer, onboarding 5
customer, service 5
data, integrating 6
lead, managing 5
lead, routing 5
opportunity, managing 5
Quote, generating 5
reporting 5
Automation, steps
collaborating 10
continuosly, learn 11
focus, outcomes 10
identify, managing 10
measure, succussing 10
open/change 10
Automation, tips
embrace, changing 9
identify, processing 9
monitor, optimizing 9

---

## Page 283

plan, integrating 9
prioritize tasks 9
tools, evaluating 9
train, communicating 9
Automation, workflow 7
B
Batch Processing 140
Batch Processing, benefits
consistency 141
efficiency 141
performance, managing 141
resource, optimizing 141
scalability 141
Batch Processing, key factors
batch size 141
data segmentation 141
error, handling 141
frequency 141
Batch Processing, use cases
customer, communications 140
inventory, managing 140
sales order, processing 140
bulk data operations 306
bulkification 238
bulkification, consumption
bulkified flow, elements 239
governor limits, transactions 238
guidelines, achieving 239-241
Bulkify Apex trigger 305
Bulkify Apex trigger, concepts 307, 308
Bulkify Apex trigger, strategies 306
Business Process 6
Business Process, challenges
complexity 8
inconsistency 8
performance, issues 9
security, vulnerabilities 9
Business Process, exceptations
consistency 8
efficiency 8
flexibility 8
security 8
Business Process, use cases
customer, feedback 7
customer, inquiries 7
inventory, managing 7
order, processing 7
payment, processing 7
D
Debug Flow, steps 248-250
Debugging 51
Debugging, techniques

---

## Page 284

collaborative, troubleshooting 52
Debug Logs 52
error message, notifying 52
fault, connectors 52
Flow Builder 51
Rollback, debug 52
test, validating 52
Debug Log 245
Debug Log, execution 246
Debug Log, steps 245, 247
Debug Log, tips
external, tools 247
focused, logging 247
interative, debugging 247
system.debug() 247
Decision Element 33, 34
delete record-triggered flows 115
delete record-triggered flows, steps 115, 116
delete record-triggered flows, use cases 116-121
Distribute Flows 259
Distribute Flows, configuring 267, 268
Distribute Flows, methods
action & recommendations 261
aura components, embedding 264
flow interview, preparing 266
lightning web, components 265
object-specific quick action 260
URL, sharing 263
utility bar, adding 262
visualforce page, embedding 265
Distribute Flows, points
access, configuring 259
documentation, supporting 260
feedback, iteration 260
methods, sharing 260
target user, identifying 259
user, communicating 259
Distribute Flows, pros 260
E
Error Handling 66
Error Handling, techniques
conditional, branching 66
error scenarios, identifying 66
flow, continuity 67
log/tracking 66
message, notifying 66
rollback, recovery 66
test, feedback 67
user, guidance 66
Experience Cloud 269
Experience Cloud, steps 269-271
Experience Cloud, use cases 269
External Objects 274

---

## Page 285

External Objects, deploying
comparison 291
flow tool, migrating 290
migration, benefits 291
External Objects, key features
customizable, integrating 274
real-time, accessing 274
virtual, representation 274
External Objects, steps 275, 276
External Objects, use cases 275
External Objects, ways 274, 275
External Services 282
External Services, key features
productivity, enhancing 282
seamless, integrating 282
standardize, invocation 282
External Services, steps 282
External Services, use cases 283
F
Failed Flow Interviews 55
Fast Field Updates 98
Fast Field Updates, steps 99-106
Flow Builder 38
Flow Builder, benefits 248
Flow Builder, button
Activate 42
Debug 42
Run 42
Save 43
Save As 42
Flow Builder, characteristics
purpose 196
record-centric 196
visual, interface 196
Flow Builder, components
Elements 38
Flow Logic 41
Resources 39
Screens 40
test, previewing 42
Flow Builder, step
accessing 43
elements, adding 44, 45
flow, creating 44
screen, configuring 46-48
Flow Interview 251
Flow Interview, best practices 252
Flow Interview, considering 251
Flow Interview, limitations 251
flow interviews, steps 247
Flow Orchestration 193
Flow Orchestration, anatomy 194-196
Flow Orchestration, components

---

## Page 286

stages 193
steps 193
Flow Orchestration, key features
control, monitoring 197
coordination, flows 197
user-centric 196
Flow Orchestration, types
Autolaunched Orchestration 193
Record-triggered Orchestrations 194
for loop 218
H
HTTP Callout 283
HTTP Callout, features
asynchronous, executing 283
external, integrating 283
versatility 283
HTTP Callout, steps 284, 285
HTTP Callout, use cases 284
I
insert record-triggered flows 96
insert record-triggered flows, steps
actions/tasks, configuring 97
exception/error, handling 97
flow, creating 96
flow logic, designing 96
flow trigger, setup 96
monitor, optimizing 97
objective, defining 96
test flow, activating 97
Invocable Method 220
Invocable Method, properties 221
Invocable Method, steps 221, 222
L
Lightning Runtime 250
Lightning Runtime, key features 251
Lightning Web Component (LWC) 225
LWC, components
embed flow, significance 228
success, considering 229
LWC, reasons
dynamic data, handling 225
seamless, integrating 225
tailored, functionality 225
user interaction, enhancing 225
LWC, steps 225-227
M
migration 292
migration, benefits 292
migration decision, logic 289
migration, foundation 288, 289

---

## Page 287

migration, reviewing 292, 293
migration, strategy 292
migration, testing 293, 294
O
Orchestration Run 197
Orchestration Run, lifecycle
error handle, resilience 197
flow, coordination 197
initiation, triggering 197
real-time, monitoring 197
Orchestrations 192
Outbound Message Actions 278
Outbound Message Actions, benefits
asynchronous, communicating 278
event-driven, integrating 278
reliable, delivery 278
Outbound Message Actions, steps 280
Outbound Message Actions, usase 278, 279
Outbound Message Actions, use cases 279
P
Packaging Flows 266
Packaging Flows, best practices
documentation 267
modularization 267
performance, optimization 267
security 267
testing 267
Packaging Flows, considering
additional, notes 267
component, inclusion 267
updating 267
Packaging Flows, types
managed 267
unlocked 267
Paused Flow Interviews 54
platform event messages 152
platform event messages, components 152
platform event messages, practices 153
platform event messages, use cases 153
Platform Events 148
Platform Events, key concepts
API, streaming 149
event delivery 149
event schema 148
event triggers 149
loose coupling 148
performance, scalability 149
permissions, security 149
publish-subscribe, model 148
Platform Events, steps 155-166
Platform Events, use cases
alert, monitoring 149

---

## Page 288

custom, application 149
integration 149
Internet of Things (IoT) 149
process, automation 149
real-time, reporting 149
platform event-triggered flow 149
platform event-triggered flow, components
activation 150
event, publishers 150
flow builder 150
flow, elements 150
platform event 149
test, monitoring 150
platform event-triggered flow, use cases
automate record, updating 150
dynamic approval, process 150
integration 150
IoT Data, processing 150
real-time, notifications 150
Pre-built Automation 21
Pre-built Automation, key differentiators
AppExchange 22
flow, templates 22
Salesforce, integrating 22
Process Builder 15
Process Builder, challenges
debugging 8
maintenance 8
order, execution 8
testing 8
Process Builder, scenario 15
publish event messages 151
publish event messages, components 151
publish event messages, use cases 151
R
record-triggered flows 94
record-triggered flows, automations 107, 108
record-triggered flows, benefits
automation 95
flexibility 95
maintainablity 95
scalability 95
user, experience 95
record-triggered flows, characteristics
event-driven 189
implicit, execution 189
tied objects 189
record-triggered flows, differences 94
record-triggered flows, purpose 94
record-triggered flows, scenario
approval, processes 95
automate, notifications 95
data, integrity 96

---

## Page 289

workflow, automation 96
record-triggered flows, steps 97, 98
record-triggered flows, use case 108-115
record-triggered orchestration 198
record-triggered orchestration, use cases 198-209
REST API, steps 186, 187
REST API, tips
authentication 188
error, handling 188
input, parameters 188
S
Salesforce 2
Salesforce Automation 3
Salesforce Automation, key features
approval, processes 4
light app, building 4
process, building 4
salesforce, flow 4
workflow 4
Salesforce Automation, services
builder, process 4
market, cloud 4
sales cloud 4
Salesforce, workflow 3
service, cloud 4
Salesforce Flow 16
Salesforce Flow, benefits
accuracy, improving 17
customization 17
flexibility 17
productivity, increasing 17
Salesforce Flow, best practices 234-238
Salesforce Flow, capabilities
Apex Code, integrating 18
business processes, automating 18
data, manipulating 18
debugging 19
decision, making 18
external system, integrating 18
loops, iterations 18
mobile, supporting 19
reusability 19
user, interacting 18
version, deploying 18
Salesforce Flow, considerations 244
Salesforce Flow Data, elements
collections 29
formulas 29
records 29
sObjects 29
variables 29
Salesforce Flow Decision, elements 32, 33
Salesforce Flow Essential, features

---

## Page 290

data, maintenance 19
guide, processes 19
record changes, automating 19
schedule, executing 19
user, interaction 19
visual, designing 19
Salesforce Flow, features
goals, defining 20
keep, simplifying 20
performance, optimizing 20
practices, leverage 21
process, identifying 20
test, thoroughly 20
Salesforce Flow, limits
data change 233
performance 233
Query 232
Salesforce Flow Potential, functions
custom business, processes 20
data entry, automation 19
data, validating 20
guide data, entry 20
survey/feedback, collecting 20
Salesforce Flow, steps 31, 32
Salesforce Flow, types
autolaunched 27
platform event-triggered 27
record-triggered 26
record-triggered orchestration 27
schedule-triggered 27
screen 26
Salesforce Flow, usase 18
Salesforce Flow, use cases
approval, processes 18
contract, managing 18
customer, onboarding 17
lead, qualification 17
Salesforce, issues
debug, reviewing 243
documentation, collaborating 243
fields, checking 242
flow errors, handling 243
null values 243
proactive debug, testing 241
user permission 243
Salesforce, key components
connectors 28
Elements 28
resources 28
Salesforce, methods 49
Salesforce ORG, creating 74-79
Salesforce, versions 49-51
schedule-triggered flows 124
schedule-triggered flows, benefits

---

## Page 291

consistency, efficiency 126
customer relationship, improving 126
scalability 126
time resource, saving 126
schedule-triggered flows, capabiilities
error, handling 139
event log, monitoring 140
event queue, managing 140
governance, compliance 140
precision, timing 139
reliability 139
resource, efficiency 139
scalability 139
schedule-triggered flows, configuring 126-138
schedule-triggered flows, key points
alerts/error, handling 144
audit, reviewing 144, 145
capacity, planning 144
performance, optimizing 144
salesforce tools, monitoring 142, 143
schedule-triggered flows, role
data, collection 125
Email, delivery 126
error, handling 126
flow, configuring 126
message, personalization 126
schedule-triggered flows, tasks
customer engagement 125
data process, recurring 125
governance, compliance 125
resource allocation, optimizing 125
time-sensitive, actions 125
screen flows 58
screen flows, benefits
data collection, efficiency 72
scalable, customizing 73
user friendly, experience 72
screen flows, break down
completion, onboarding 73
document, uploading 73
information, collecting 73
role, assignment 73
screen flows business, logic
apex logic 63
desicion, elements 62
error handling 63
external system, integrating 62
formula, fields 62
loop, iteration 62
validation, rules 63
varibable, assignment 62
screen flows display, records
condition display, logic 63
field, mapping 63

---

## Page 292

real-time calculations 64
record actions 64
records, lookup 63
related, records 64
visual representation 64
screen flows, distributing 89-91
screen flows distribution, techniques
continuous, improvement 65
documentation user, training 65
flow visibility, controlling 65
Light App Builder, including 65
light pages, embedding 64
links button, creating 65
mobile, accessibility 65
URL Access, utilizing 65
screen flows, fundamentals
components 60
flow builder 60
flow, connectors 60
flow, elements 60
purpose, structure 60
variable resource, managing 60
screen flows key, learning 68, 69
screen flows, scenarios
business rules, decision making 59
complex data, collection 59
guided user, experiences 59
real time data, validation 59
user engagement, enhancing 59
screen flows, techniques
conditional, visibility 61
error, handling 61
indicators, navigating 61
information, gathering 61
mobile, responsiveness 62
prepopulating data 61
user friendly, designing 61
Subflow 27
Subflow, benefits
easy, maintenance 28
encapsulation 28
modularity 28
reusability 27
Subflow, concepts
business logic, encapsulation 68
components, reusable 68
creating 67
design, benefits 67
name, conventions 68
parameter, passing 67
scalability, promoting 68
understanding 67
Subflow, usage 80-89

---

## Page 293

T
Troubleshooting 53
Troubleshooting, strategies 252
Troubleshooting, techniques
collaborate 54
data problem, troubleshooting 53
documentation, sharing 54
error message, logs 53
flow, configuring 53
flow variables, checking 53
formula expressions, validating 53
validation errors, handling 53
W
Workflow 14
Workflow/Process Builder, key differences 16
Workflow, scenario 14
