BI &amp; Data Analytics Portfolio

# [Project 1: DataBase & BI reporting: Project Overview](https://github.com/gastonlucca/Gaston-Portfolio) 
* BI REPORTING STRUCTURE: Create a system of BI reporting which allows a display of data and reporting system, to track the performance of the program.

1. Definition of reporting tool 
2. Definitions of KPIs
3. Definition of the dashboard, regular reporting, and ad-hoc reporting

* DATABASE STRUCTURE: Design and create a solid database which contain structural data, easy to retrieve which allows answer simples queries.

1. Data gathering porcess and normalization
2. ETL procces 
3. Database estructure: variables – dimensions, define transactional tables, schemas (star)- data types
4. Data base Wharehouse – site – back up - testing

![](https://github.com/gastonlucca/Gaston-Portfolio/blob/master/BI%20MECON%20porject%202.PNG)

# [Project 2:  Analysis of trends and metrics for La.Radio.live](https://github.com/gastonlucca/Gaston-Portfolio)
For this project I have select and define a series of metrics, relevant to analyze the performance of the Facebook site for the company, [LaRadio.live](https://laradio.live/)

Gathering all this information I was able to summary the performance of the Facebook site, estimate by linear regression the future like level. Through this analysis I have generated actionable conclusions and extraction of actionable insights, in order to calibrate the marketing strategy of the company. 

Broadcasting Performance:

![Broadcasting Performance](https://github.com/gastonlucca/Gaston-Portfolio/blob/master/La%20Radio.%20Correlation.PNG)

# [Project 3: Support Function Cost Automation: Objetives, Estructure & Dashboards](https://github.com/gastonlucca/Gaston-Portfolio)
* OBJECTIVES: 

1. To improve collection, preparation and display of data to promote a change in financial analysis department.
2. Automatization of process that it is been build from different sources (SAP ERP, ORACLE, manual settings, local files) 

* ESTRUCTURE: 


![](https://github.com/gastonlucca/Gaston-Portfolio/blob/master/SFC%20Data%20Architecture.PNG)

* DASHBOARDS:

![](https://github.com/gastonlucca/Gaston-Portfolio/blob/master/SFC.%20Data%20Model%202-%20DASHBOARDS%201.png)

![](https://github.com/gastonlucca/Gaston-Portfolio/blob/master/SFC.%20Data%20Model%202-%20DASHBOARDS%202.png)
![](https://github.com/gastonlucca/Gaston-Portfolio/blob/master/SFC.%20Data%20Model%202-%20DASHBOARDS%203.png)


# [Project 4: Finances BI Report: Project Overview](https://github.com/gastonlucca/Gaston-Portfolio)
* OBJECTIVES: 

1. Provide to the finances department a BI solution in order to improve the collection and display of data
2. Improve data visualization and analytics through Tableau softwares



> Note: WIP

# [Project 5: Deploying BI solution & Advanced analytics with IDS - AWS + Tableau](https://github.com/gastonlucca/Gaston-Portfolio) 
* BI REPORTING ESTRUCTURE: Create a system of BI & Advance analitic reporting which allow to cover Business use case (bussines analitics demands) 

1. Definition of Use case (Agile methodology/ Canva model) 
2. Business/Data Analysis + prioritization: How to solve the use case and how we prioritize the backlog 
3. Data Architecture: What is the data architecture I need to resolve this problem
4. Definitions of KPIs, business rules, data quality rules, Critical data elements 
5. Deploy data governance: to guarantee that the technical solution is in compliance with the company data strategy (Dat quality, tools, data security) 
6. Development part: Coding (Scrum master methodology) + UAT + delivering the model 
7. Definition of the dashboard, regular reporting, and ad-hoc reporting

* DATABASE STRUCTURE: Design and create a solid database that contains structural data, easy to retrieve which allows answer simple queries + live data connection

1. Data gathering process and normalization
2. ETL process + data ingestion 
3. Database structure: variables – dimensions, define transactional tables, schemas (star)- data types
4. Database Wharehouse – site – back up - testing  

* Process automation  by DDBB deployment: Data flow

![](https://github.com/gastonlucca/Gaston-Portfolio/blob/master/IDS%20Data%20Flow.PNG)

* Data Architecture + data ingestion for data model customization 

![](https://github.com/gastonlucca/Gaston-Portfolio/blob/master/BI%20Architecture.PNG)

> Note: WIP

# [Project 6: Deploying Data Governance base on DCAM approach](https://github.com/gastonlucca/Gaston-Portfolio) 

* What is the right strategy to develop a solid data analytic environment in an organization
* Customizing DCAM based on the particularities of your organization
* Active data security: Virtuous data quality circle
* Active data security: Data attack surface - Data breach map - Deploy of the control point of access 

![](https://github.com/gastonlucca/Gaston-Portfolio/blob/master/dcam_components_graphic_feb_.png)

> Note: WIP

# [Project 7: Data Architecture for quotation model](https://github.com/gastonlucca/Gaston-Portfolio)

1. Data research to create a quotation model based on SAP 
2. Data ingestion and analysis 
3. JOIN STATEMENT identification on SQL code
4. Data architecture to be programming on ETL Power Center  
5. Designing the schema

![](https://github.com/gastonlucca/Gaston-Portfolio/blob/master/Quotation%20model%20on%20SAP%20ERP.PNG)

Schema target 	tabla target 	Schema	Object	Depedent Schema	Dependent Object (Table /View)	Fields (join)	JOIN CLAUSE
edw_europebi	edw_europebi.fact_ offert_detail _ iberia 	app_0108_europebi	sd_ibs_zqu_hgen	app_0108_europebi	sd_ibs_zqu_det	nquot + nvrsio	left join app_0108_europebi.sd_ibs_zqu_det det on hgen.nquot = det.nquot and hgen.nvrsio = det.nvrsio
edw_europebi	edw_europebi.fact_ offert_detail _ iberia 	app_0108_europebi	sd_ibs_zqu_hgen	app_0108_europebi	sd_ibs_zqu_hstd	nquot + nvrsio	left join app_0108_europebi.sd_ibs_zqu_hstd hstd on hgen.nquot = hstd.nquot and hgen.nvrsio = hstd.nvrsio
edw_europebi	edw_europebi.fact_ offert_detail _ iberia 	app_0108_europebi	sd_ibs_zqu_hgen	app_0108_europebi	sd_ibs_zqu_cust	nquot + nvrsio	left join app_0108_europebi.sd_ibs_zqu_cust cust on cust.nquot = hgen.nquot and cust.nvrsio = hgen.nvrsio
edw_europebi	edw_europebi.fact_ offert_detail _ iberia 	app_0108_europebi	sd_ibs_zqu_hgen	app_0108_europebi	sd_ibs_zqu_1stascht	stsch , status, spras	left join app_0108_europebi.sd_ibs_zqu_1stascht stascht   on hgen.stsch =stascht.stsch and hgen.status=stascht.status and hgen.spras=stascht.spras
edw_europebi	edw_europebi.fact_ offert_detail _ iberia 	app_0108_europebi	sd_ibs_zqu_hgen	edw	dim_schneider_worker (usertable)	usercrea_id	left join edw.dim_schneider_worker usertable ON usertable.id_ = hgen.usercrea
edw_europebi	edw_europebi.fact_ offert_detail _ iberia 	app_0108_europebi	sd_ibs_zqu_hgen	edw	dim_customer_all (acc) 	leg_sacc_id_ 	left join edw_di_customer_all acc ON acc.leg_sacc_id_= mcust.sapcust  ???
edw_europebi	edw_europebi.fact_ offert_detail _ iberia 	app_0108_europebi	sd_ibs_zqu_hgen	edw_europebi	fact_net_orders_service_contracts_iberia (fact) 	zzoferta	left join edw_europebi.fact_net_orders_service_contracts_iberia fact  ON fac.zzoferta = hgen.nquot
![image](https://user-images.githubusercontent.com/69059703/187313949-4b167243-ee7a-4ed1-ab25-ee2da7340d7c.png)

