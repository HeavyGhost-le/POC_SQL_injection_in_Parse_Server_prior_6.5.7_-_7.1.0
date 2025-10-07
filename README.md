Database Ghost - Advanced PostgreSQL Enumeration Tool
<p align="center"> <img src="https://img.shields.io/badge/Python-3.6%2B-blue?style=for-the-badge&logo=python" alt="Python"> <img src="https://img.shields.io/badge/PostgreSQL-SQL%20Injection-red?style=for-the-badge&logo=postgresql" alt="PostgreSQL"> <img src="https://img.shields.io/badge/CVE-2024--39309-orange?style=for-the-badge" alt="CVE-2024-39309"> <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License"> </p>
🚨 Critical Security Notice
⚠️ LEGAL DISCLAIMER: This tool is provided for educational and authorized security testing purposes ONLY. Unauthorized use against systems you don't own or lack explicit permission to test is illegal and unethical. Developers assume no liability for misuse.

📖 Overview
Database Ghost is an advanced PostgreSQL database enumeration tool designed to demonstrate the exploitation of SQL injection vulnerabilities in Parse Server (CVE-2024-39309). It provides comprehensive database reconnaissance capabilities through a single vulnerability point, enabling security researchers to assess the impact of this critical vulnerability.

CVE Reference: CVE-2024-39309 - SQL Injection in Parse Server prior to versions 6.5.7 and 7.1.0

✨ Features
🔍 Database Intelligence
Version Detection - PostgreSQL version and system information

Database Discovery - Current database and schema enumeration

User Analysis - Current user context and session information

🛡️ Privilege Assessment
Privilege Mapping - Comprehensive user privilege enumeration

Superuser Detection - Identify administrative database access

Capability Analysis - File operation and function privileges

📁 File System Operations
File Reading - Arbitrary file access via pg_read_file()

Directory Listing - Explore filesystem with pg_ls_dir()

System File Access - Read /etc/passwd, /etc/hosts, and critical system files

🗃️ Schema Enumeration
Schema Discovery - Complete database schema inventory

Table Analysis - Table structures, types, and relationships

Column Mapping - Detailed column information and data types

📊 Data Extraction
Sample Data Retrieval - Extract representative data from tables

Sensitive Data Detection - Pattern-based sensitive table identification

Row Count Analysis - Database size and table population metrics

🛠️ Installation
Prerequisites
Python 3.6 or higher

requests library

Quick Setup
```
# Clone the repository
git clone https://github.com/yourusername/database-ghost.git
cd database-ghost

# Install dependencies
pip install requests

# Make executable
chmod +x star_ghost_english.py
```

🎯 Usage Examples
Basic Comprehensive Enumeration
```
python3 star_ghost_english.py -u http://target:1337 -a parse-application-id
```
