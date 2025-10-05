# Umukamisha Celine
**ID:** 27400
**Date:** 05th October 2025  

# PL/SQL Assignment

## TASK 1: CREATE A NEW PLUGGABLE DATABASE (PDB)

**Objective:** Create a pluggable database with the format FirstTwoLettersOfFirstName_pdb_StudentID

**Result:** Pluggable database ce_pdb_27400 was successfully created with admin user celine_plsqlauca_27400.

![Task 1 Screenshot](images/task1.png)

## TASK 2: CREATE AND DELETE A PDB

**Objective:** Create another PDB with format FirstTwoLettersOfName_to_delete_pdb_StudentID, then delete it.

**Creation:**

![Task 2 Creation](images/task2-creation.png)

**Deletion:**

![Task 2 Deletion](images/task2-deletion.png)

**Result:** Pluggable database was successfully created and then completely removed including all associated datafiles.

## TASK 3: ORACLE ENTERPRISE MANAGER

**Objective:** Configure and access Oracle Enterprise Manager Database Express

**Access Method:**
- URL: https://localhost:5500/em/login
- Username: SYS
- Authentication: SYSDBA privileges

**Notes:** Oracle Enterprise Manager was accessed using the SYS administrative account. Initial attempts were made to access OEM using the custom PDB user account (celine_plsqlauca_27400) created in Task 1. However, authentication with this user account was unsuccessful. After investigation, this is a known limitation of Oracle Database Express Edition, which restricts Enterprise Manager access to CDB-level administrative accounts (SYS and SYSTEM) rather than individual PDB users. Using the SYS account is the standard method for OEM administrative access in Express Edition installations.

**Dashboard Overview:** The Oracle Enterprise Manager dashboard displays:
- Database status and uptime information
- Database type (Single Instance) and version (21.3.0.0.0 Enterprise Edition)
- Performance metrics including Activity, Services, and Containers
- Resource utilization (CPU, Active Sessions, Memory, Data Storage)

**Login with SYS and Password**

![OEM Login](images/oem-login.png)

**Dashboard**

![OEM Dashboard](images/oem-dashboard.png)

## ISSUES ENCOUNTERED AND SOLUTIONS

1. **PDB User Authentication in OEM:** Attempted to login to Enterprise Manager using the PDB-specific user account but encountered "Invalid Database Credentials" errors. This was resolved by using the SYS account, which is the appropriate administrative account for OEM access in Oracle Express Edition.

2. No other significant issues encountered. All SQL commands executed successfully on first attempt.

## CONCLUSION

All three tasks were completed successfully:
- Task 1: Created permanent PDB ce_pdb_27400 for classwork storage
- Task 2: Demonstrated PDB lifecycle management by creating and deleting a temporary PDB
- Task 3: Successfully accessed and navigated Oracle Enterprise Manager Database Express

The assignment demonstrated understanding of pluggable database architecture, SQL*Plus commands, and Oracle database administration tools.

---


