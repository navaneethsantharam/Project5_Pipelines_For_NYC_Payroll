# Project5_Pipelines_For_NYC_Payroll

Below are the data pipelines implemented-

1.**Pipeline Employee Master to Synapse->** Load EmpMaster.csv from storage account to synapse table->**NYC_Payroll_EMP_MD**

2.**Pipeline Agency Master to Synapse->** Load AgencyMaster.csv from storage account to synapse table->**NYC_Payroll_AGENCY_MD**

3.**Pipeline Load Title Master to Synapse->** Load TitleMaster.csv from storage account to synapse table->**NYC_Payroll_TITLE_MD**

4.**Pipeline Load 2021 Payroll into SQLDB->** Load NYC file for 2021(nycpayroll_2021.csv) to sql db table->**NYC_Payroll_Data**

5.**Pipeline Load Current Year Data from SQLDB to Synapse->** Copy NYC data for 2021 from sql db to synapse table->**NYC_Payroll_Data**

6.**Pipeline Load All Data into Synapse->** Master pipline to perform which performs all synapse loading in one-go (step1,step3 and step3 and step5 mentioned above)

7.**Pipeline Aggregate Total Paid->** Computes Totalpaid = (RegularGrossPaid + TotalOTPaid+TotalOtherPay) and aggregate by Agency Name and Fiscal Year on 2021 and 2020 data and load to synapse table->**NYC_Payroll_Summary**
