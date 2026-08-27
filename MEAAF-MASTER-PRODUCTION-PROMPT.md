# MEAAF WINDOWS — MASTER PRODUCTION EXECUTION PROMPT v2.0
## Secure Enterprise Hospital + Pharmacy + Accounting + ERP Platform
### Product: مِعاف | MEAAF
### By: Victoria Line Soft | فكتوريا لاين سوفت
### Contact: 771119726

============================================================
0. ROLE AND MISSION
============================================================

أنت فريق هندسي متكامل يعمل كجهة تنفيذ Production Engineering وليس كمولد واجهات.

الأدوار المطلوبة:
- Principal Software Architect
- Senior Windows Desktop Engineer
- Backend/API Engineer
- Database Engineer
- Accounting Systems Engineer
- Healthcare Systems Engineer
- Security Engineer
- DevSecOps Engineer
- QA Automation Engineer
- Performance Engineer
- UI/UX Engineer
- Windows Installer/Release Engineer

مهمتك تنفيذ مشروع MEAAF الموجود في الملفات المرفقة وتحويله إلى منتج Windows مؤسسي حقيقي قابل للبناء والتثبيت والتشغيل والصيانة.

لا تنشئ Demo.
لا تنشئ Prototype.
لا تضع واجهات وهمية.
لا تعتبر TODO أو Placeholder تنفيذًا.
لا تقل "تم" إلا بعد وجود دليل قابل للتحقق.

============================================================
1. PRODUCT IDENTITY — لا تغيّرها
============================================================

اسم المنتج:
مِعاف

English:
MEAAF

الوصف:
منظومة الإدارة الصحية والمحاسبية الذكية

Parent Company:
Victoria Line Soft
فكتوريا لاين سوفت

الوصف:
فكتوريا لاين سوفت للأنظمة المحاسبية والإدارية والتطبيقات والخدمات البرمجية المتكاملة

Contact:
771119726

استخدم الشعار المرفق باعتباره الأصل الرسمي للهوية.
لا تعيد رسم الشعار ولا تغيره من شاشة إلى أخرى.

============================================================
2. FIRST ACTION — INSPECT BEFORE CODING
============================================================

قبل تعديل أي ملف:

1. افحص كامل المشروع.
2. افحص solution/project files.
3. افحص dependencies.
4. افحص database/schema/migrations.
5. افحص كل View/Page/Window.
6. افحص Services/Repositories/Domain.
7. افحص Authentication/Authorization.
8. افحص Backup/Restore.
9. افحص Printing/Reports.
10. افحص Tests.
11. افحص Build configuration.
12. افحص Installer.
13. افحص أي secrets أو credentials مكشوفة.
14. افحص TODO/NotImplemented/placeholder/mock/demo code.

أنشئ:
PROJECT-BASELINE.md

ويحتوي:
- Existing
- Working
- Partial
- Missing
- Broken
- Security Risk
- Build Risk
- Test Gap

ممنوع حذف وظيفة موجودة فقط لتقليل العمل.

============================================================
3. TRUTHFUL ENGINEERING POLICY
============================================================

لا تستخدم:
"جاهز"
"مكتمل"
"100%"
"Production Ready"

إلا إذا كان هناك دليل.

كل وظيفة لها:
IMPLEMENTATION STATUS
TEST STATUS
EVIDENCE

الحالات:
PASS
FAIL
NEEDS REVIEW
BLOCKED
NOT IMPLEMENTED

إذا لم تستطع تنفيذ اختبار بسبب عدم توفر Windows/Printer/Environment:
لا تخمن.
ضع:
BLOCKED — Environment Required

============================================================
4. TARGET ARCHITECTURE
============================================================

استخدم Architecture قابلة للصيانة.

يفضل عند ملاءمة المشروع:
- .NET LTS المناسب
- WPF/Windows Desktop
- MVVM
- Dependency Injection
- EF Core أو Persistence strategy مناسبة
- SQLite/local DB للـOffline عند ملاءمتها
- ASP.NET Core Secure API للـCentral/Sync
- Structured Logging
- Automated Testing

طبقات واضحة:
Presentation
Application
Domain
Infrastructure
Persistence
Security
Reporting
Printing
Synchronization
Licensing
AI
Diagnostics

لا تضع Business Logic داخل Views.

============================================================
5. OFFLINE-FIRST
============================================================

MEAAF يجب أن يعمل Offline في الوظائف الأساسية.

Offline:
- Patients
- Visits
- Billing
- Payments
- Inventory
- Purchasing
- Pharmacy
- Accounting
- Reports
- Printing
- Backup

استخدم:
Transactions
Atomic Operations
Recovery
Retry
Outbox/Queue

إذا انطفأ الجهاز أثناء عملية:
- لا تترك Transaction نصف مكتملة.
- لا تنشئ قيودًا غير متوازنة.
- لا تكرر الدفع.
- لا تضاعف حركة المخزون.
- لا تفقد البيانات committed.

============================================================
6. ENTERPRISE MODULES
============================================================

نفذ فعليًا:

CORE
- Configuration
- Organization
- Branches
- Warehouses
- Cashboxes
- Departments
- Cost Centers

AUTH
- Users
- Roles
- Permissions
- Sessions
- Devices
- Password Management

HOSPITAL
- Patients
- Patient Files
- Clinics
- Doctors
- Appointments
- Emergency
- Admissions
- Rooms
- Beds
- Operations
- Laboratory
- Radiology
- Medical Services
- Insurance
- Billing

PHARMACY
- Medicines
- Items
- Batches
- Expiry
- Sales
- Returns
- Purchases
- Inventory

ACCOUNTING
- Chart of Accounts
- Journal Entries
- Posting
- Reversal
- Adjustments
- General Ledger
- Trial Balance
- Income Statement
- Balance Sheet
- Cash Flow
- Customers
- Suppliers
- Cashboxes
- Banks
- Currencies
- Taxes
- Cost Centers
- Fiscal Periods

INVENTORY
- Receipt
- Issue
- Transfer
- Adjustment
- Stock Count
- Return
- Damaged
- Expired

PURCHASING
Purchase Request
→ Approval
→ Quotations
→ Purchase Order
→ Receipt
→ Supplier Invoice
→ Accounting
→ Payment

HR
- Employees
- Departments
- Positions
- Contracts
- Attendance
- Leaves
- Advances
- Loans

PAYROLL
Attendance
→ Calculation
→ Allowances
→ Deductions
→ Advances
→ Loans
→ Approval
→ Payment
→ Journal Entry

FIXED ASSETS
- Assets
- Cost
- Depreciation
- Maintenance
- Transfer
- Disposal
- Sale

INSURANCE
- Companies
- Contracts
- Coverage
- Copayment
- Claims
- Accepted
- Rejected
- Pending
- Settlements

REPORTING
- Financial
- Hospital
- Pharmacy
- Inventory
- Purchasing
- HR
- Audit
- Sync
- System Health

============================================================
7. DATABASE INTEGRITY
============================================================

Database must have:
- Foreign Keys
- Unique Constraints
- Indexes
- Check Constraints where applicable
- Transactions
- Referential Integrity

Prevent:
- orphan records
- duplicate business documents
- duplicate payments
- negative stock where business rules prohibit it
- unbalanced journal entries
- invalid state transitions

Critical financial operations must be atomic.

============================================================
8. ACCOUNTING SAFETY
============================================================

Rules:

Debit = Credit for every posted journal entry.

Posted entries:
- cannot be silently edited.
- corrections use reversal/adjustment.
- every reversal references original entry.
- fiscal period controls must be enforced.

Test:
- posting
- reversal
- adjustment
- closing
- reopening
- concurrent posting
- crash during posting
- duplicate submission

============================================================
9. AUTHENTICATION
============================================================

Every user:
- Username
- Password
- Employee
- Role
- Branch
- Department
- Status
- Last Login
- Sessions
- Devices

Implement:
- strong password hashing
- unique salt
- login throttling
- failed attempt protection
- session expiry
- logout
- session revocation
- password change
- secure credential storage

Never store plaintext passwords.

============================================================
10. RBAC + SCOPE
============================================================

Authorization model:

Tenant
→ Branch
→ Department
→ Warehouse/Cashbox
→ Module
→ Screen
→ Operation

Operations:
View
Add
Edit
Delete
Approve
Post
Reverse
Cancel
Print
Export
Import
Discount
ChangePrice
Return
ClosePeriod
ReopenPeriod
Backup
Restore
Sync

Authorization must be enforced server/domain side.

UI hiding is NOT security.

Test direct service/API access as well as UI.

============================================================
11. MULTI-TENANT ISOLATION
============================================================

Tenant A must NEVER read/write Tenant B.

Test:
- changed tenant ID
- changed record ID
- direct API call
- malformed request
- unauthorized export
- cross-branch request

Expected:
DENIED.

Do not rely only on frontend filtering.

============================================================
12. SECURITY — DEFENSE IN DEPTH
============================================================

Implement and test:

Application:
- Input validation
- Output encoding
- Secure error handling
- CSRF protection where relevant
- Rate limiting where relevant
- Secure file upload
- Path traversal prevention
- SQL injection prevention
- IDOR prevention
- Safe deserialization
- Dependency vulnerability management

Authentication:
- Password hashing
- Session security
- MFA for privileged administration
- Account lock/throttling
- Session revocation

Network:
- TLS
- Certificate validation
- Secure API authentication
- Request validation
- Replay protection for sensitive synchronization where applicable

Secrets:
- NEVER embed private keys/API secrets/passwords in source code.
- NEVER commit secrets.
- Use environment/secret store appropriate to deployment.
- Use Windows DPAPI/Credential Manager or equivalent for local protected secrets where appropriate.

============================================================
13. CODE/IP PROTECTION
============================================================

Client receives:
- signed release binaries
- required runtime/dependencies
- installer

Client does NOT receive:
- source code
- private signing keys
- server master secrets
- Victoria Line Soft control-plane credentials

Use where technically appropriate:
- Release build
- symbol separation
- code obfuscation for managed assemblies
- integrity verification
- signed executable
- signed installer
- signed updates

IMPORTANT:
Do not claim obfuscation prevents reverse engineering completely.
It only increases difficulty.

============================================================
14. DATA PROTECTION
============================================================

Protect sensitive data:
- encryption at rest where appropriate
- TLS in transit
- encrypted backups
- access control
- least privilege
- secure attachment storage
- checksum/integrity validation

Do not expose:
- passwords
- tokens
- encryption keys
- private keys
- sensitive customer data in logs.

============================================================
15. VICTORIA LINE SOFT CONTROL PLANE
============================================================

Separate administrative plane for:
- Clients
- Tenants
- Licenses
- Subscriptions
- Products
- Versions
- Updates
- Support
- Services
- Module activation

Privileged administration:
- MFA
- strong RBAC
- session management
- audit
- suspicious-login detection
- session revocation

No unnecessary access to customer data.

Use least privilege.

============================================================
16. LICENSING
============================================================

Editions:
Hospital Edition
Pharmacy Edition
Hospital + Pharmacy
Enterprise

Controls:
- users
- devices
- branches
- modules
- features
- subscription duration
- updates
- services

License must be cryptographically verifiable.

Never trust:
- UI flags
- local editable config
- plain license text.

License enforcement must occur in application/domain/service boundaries.

Graceful behavior on:
- expired
- invalid
- revoked
- offline grace period if intentionally supported

Do not destroy customer data when license expires.

============================================================
17. AUDIT
============================================================

Record:
- User
- Timestamp
- Device
- Tenant
- Branch
- Action
- Entity
- EntityId
- OldValue
- NewValue
- Reason
- Result
- CorrelationId

Sensitive operations:
- invoice modification
- cancellation
- returns
- discounts
- price changes
- inventory adjustment
- journal reversal
- permission changes
- settings
- period close/reopen
- cash withdrawal
- reconciliation
- backup
- restore
- sync
- exports
- failed authorization

Audit must be append-oriented and protected from ordinary users.

============================================================
18. BACKUP / RESTORE
============================================================

Support:
Manual
Automatic
Daily
Weekly
Monthly
End of Period

Full and incremental where technically appropriate.

Backup success requires:
1. file creation
2. integrity validation
3. readable metadata
4. successful test restore during QA
5. data comparison

Restore:
- authorization
- pre-restore backup
- compatibility check
- integrity check
- isolated test
- clear recovery path

Never claim restore works without actually restoring a test backup.

============================================================
19. SYNCHRONIZATION
============================================================

Architecture:

Local DB
→ Outbox
→ Validation
→ Secure API
→ Server
→ Confirmation

States:
Pending
Uploading
Synced
Failed
Retrying
Conflict

Requirements:
- idempotency
- deduplication
- retry with backoff
- conflict detection
- deterministic conflict policy
- audit
- no silent overwrite

Every sync item must have an identifier/correlation mechanism.

============================================================
20. SEARCH
============================================================

Global/Advanced Search:
- Name
- Code
- Number
- Phone
- Barcode
- Invoice
- Patient File
- Employee
- Supplier
- Document
- Date
- Amount
- Branch
- Department
- Warehouse
- User

Must respect authorization and tenant boundaries.

============================================================
21. REPORTS
============================================================

Implement real report generation.

Financial:
General Ledger
Trial Balance
Income Statement
Balance Sheet
Cash Flow
Account Statement
Customer/Supplier Statements

Hospital:
Patients
Visits
Clinics
Doctors
Emergency
Admissions
Operations
Lab
Radiology
Insurance
Revenue

Pharmacy:
Sales
Purchases
Inventory
Movement
Expiry
Damaged
Suppliers
Customers

Management:
Branch Performance
Employee Activity
Audit
Sync
System Health

============================================================
22. CUSTOM REPORT BUILDER
============================================================

Authorized user can choose:
- fields
- columns
- filters
- sorting
- grouping
- totals

Save templates.

No report can bypass authorization.

============================================================
23. PRINTING
============================================================

Support:
58mm
80mm
A5
A4
Custom

Proper template per paper size.

Must support:
RTL
LTR
mixed content
long tables
multi-page
header
footer
page numbers
totals
logo
user
date

Prevent:
clipping
overlap
missing totals
bad pagination
text outside page

Provide Preview.

============================================================
24. UI/UX
============================================================

Design:
Premium
Enterprise
Medical Technology
Modern
Minimal
Professional

Support:
Arabic RTL
English LTR
Light
Dark

Required states:
Loading
Empty
Error
Success
Validation
Permission Denied
Offline
Syncing
Conflict
Warning
Critical

Keyboard shortcuts where useful.

No fake counters or fake dashboard statistics.

============================================================
25. DASHBOARD
============================================================

Permission-aware dashboard:
- revenue
- expenses
- net result
- patients
- invoices
- cashboxes
- banks
- inventory
- alerts
- approvals
- sync state
- system health

Every number must come from actual data.

============================================================
26. SMART NOTIFICATIONS
============================================================

Implement real rules for:
- low stock
- near expiry
- cash difference
- inventory difference
- backup failure
- sync failure
- license expiry
- abnormal discounts
- repeated cancellations
- suspicious activity
- pending approvals

============================================================
27. MEAAF AI
============================================================

AI features:
- revenue analysis
- expense analysis
- inventory analysis
- near-expiry analysis
- sales analysis
- natural language reports
- branch performance
- anomaly indicators

AI MUST inherit user authorization.

Architecture:
User
→ Authorization
→ Safe Query/Analytics Layer
→ Allowed Data
→ AI
→ Response

NEVER:
User
→ AI
→ unrestricted database

Do not give the model raw unrestricted SQL/database credentials.

Log AI actions without leaking sensitive content unnecessarily.

============================================================
28. SELF-DIAGNOSTICS
============================================================

Monitor:
- database
- disk
- backup
- sync
- services
- license
- failed operations
- archive

States:
Healthy
Warning
Critical

Diagnostics must include actionable reason and timestamp.

============================================================
29. ARCHIVE
============================================================

Lifecycle:
Active
→ Inactive
→ Archived

Sensitive historical data must not be silently hard-deleted.

============================================================
30. PERFORMANCE ENGINEERING
============================================================

Test realistic scale:
- thousands of patients
- thousands of invoices
- millions of records
- large audit history
- large inventory
- multiple branches
- concurrent users
- large reports

Measure:
- startup
- login
- search
- save
- report generation
- printing
- backup
- restore
- synchronization

Record actual results.

============================================================
31. CRASH / RECOVERY
============================================================

Test forced termination during:
- invoice save
- payment
- inventory movement
- journal posting
- purchase receipt
- sync upload
- backup
- migration

After restart verify:
- no corruption
- no duplicate transaction
- no orphan data
- balances remain correct
- queues recover correctly

============================================================
32. TESTING MATRIX
============================================================

Mandatory:
Unit
Integration
API
Database
Security
Authorization
UI
E2E
Performance
Backup
Restore
Sync
Recovery
Installer

Test CRUD and critical workflows.

============================================================
33. SECURITY TEST MATRIX
============================================================

Attempt:
- wrong password
- brute-force style repeated failures within safe test limits
- expired session
- revoked session
- unauthorized operation
- changed TenantId
- changed BranchId
- changed record ID
- unauthorized export
- malicious input
- invalid file
- oversized attachment
- path traversal payload
- SQL injection payloads
- malformed API requests
- replay of sensitive sync request where applicable

All must be handled safely.

Do not perform destructive tests against real customer data.

============================================================
34. INSTALLER
============================================================

Produce a real Windows installer.

Test:
- clean installation
- first launch
- initial database
- login
- printing
- backup
- restore
- upgrade
- migration
- uninstall
- reinstall
- application data preservation policy

Installer and binaries should be signed if a valid signing certificate is supplied.

Never put a private signing key in source control.

============================================================
35. WINDOWS COMPATIBILITY
============================================================

Do not claim support based on theory.

For every supported Windows version record:
- OS version
- architecture
- runtime
- install result
- launch result
- database result
- printing result
- backup result
- update result
- uninstall result

If an OS cannot be supported by the selected runtime:
state it explicitly and document the minimum supported OS.

============================================================
36. DEVELOPMENT GATES
============================================================

Do not implement everything in one uncontrolled pass.

Use gates:

GATE 1:
Architecture + Database

GATE 2:
Core + Authentication + RBAC

GATE 3:
Audit + Accounting

GATE 4:
Hospital

GATE 5:
Pharmacy + Inventory + Purchasing

GATE 6:
HR + Payroll + Assets + Insurance

GATE 7:
Reports + Printing + Export

GATE 8:
Backup + Restore + Archive

GATE 9:
Offline + Sync

GATE 10:
Licensing + Control Plane

GATE 11:
Security Hardening

GATE 12:
AI

GATE 13:
Performance

GATE 14:
Windows Installer + Compatibility

GATE 15:
Full E2E + Release Audit

At every gate:
BUILD
→ TEST
→ FIX
→ RETEST

Do not continue while a blocking defect remains.

============================================================
37. DEFINITION OF DONE
============================================================

A feature is DONE only when:

- implemented
- connected to UI
- connected to domain/application
- persisted correctly
- authorized
- validated
- error handled
- audited where required
- tested
- documented
- retested after fixes

============================================================
38. NO-FICTION RULE
============================================================

Search the entire codebase for:
TODO
FIXME
NotImplementedException
throw new NotImplementedException
placeholder
mock
fake
demo
sample
dummy
coming soon

Classify every occurrence.

No production-critical placeholder may remain.

If a test uses mock data, it must be clearly isolated from production.

============================================================
39. RELEASE AUDIT
============================================================

Generate:

FINAL-AUDIT-REPORT.md
TEST-RESULTS.md
SECURITY-AUDIT.md
PERFORMANCE-REPORT.md
WINDOWS-COMPATIBILITY.md
BACKUP-RESTORE-REPORT.md
SYNC-TEST-REPORT.md
RELEASE-NOTES.md

Use only:
PASS
FAIL
NEEDS REVIEW
BLOCKED

Severity:
CRITICAL
HIGH
MEDIUM
LOW

============================================================
40. RELEASE BLOCKERS
============================================================

Release is BLOCKED if any of these fail:

- build
- startup
- login
- authorization
- tenant isolation
- accounting integrity
- database integrity
- backup validation
- restore
- offline recovery
- sync integrity
- security-critical test
- installer
- critical printing
- migration safety

============================================================
41. FINAL ARTIFACTS
============================================================

Produce:

/src
/tests
/database
/docs
/installer
/config
/release

Required:
- complete source
- solution
- projects
- migrations
- tests
- installer
- README
- BUILD-GUIDE.md
- SECURITY.md
- FINAL-AUDIT-REPORT.md
- TEST-RESULTS.md
- PERFORMANCE-REPORT.md
- WINDOWS-COMPATIBILITY.md
- BACKUP-RESTORE-REPORT.md
- SYNC-TEST-REPORT.md
- RELEASE-NOTES.md

Also produce release binaries only after successful build.

============================================================
42. REQUIRED FINAL OUTPUT
============================================================

في النهاية أعطني:

1. ماذا تم تنفيذه.
2. ماذا تم اختباره.
3. عدد الاختبارات.
4. عدد PASS.
5. عدد FAIL.
6. عدد NEEDS REVIEW.
7. عدد BLOCKED.
8. أهم المخاطر.
9. إصدارات Windows التي تم اختبارها فعليًا.
10. نتيجة Build.
11. نتيجة Installer.
12. نتيجة Backup/Restore.
13. نتيجة Offline/Sync.
14. نتيجة Security.
15. نتيجة Performance.
16. مكان ملفات المشروع.
17. مكان ملف Installer.
18. مكان FINAL-AUDIT-REPORT.

لا تقل 100% إلا إذا كان هناك دليل فعلي على كل Release Gate.

============================================================
43. EXECUTION COMMAND
============================================================

ابدأ الآن.

PHASE 0:
Inspect Project
→ Baseline
→ Dependency Audit
→ Security Scan
→ Build Attempt

ثم نفّذ GATE 1.

بعد كل Gate:
BUILD
TEST
FIX
RETEST

لا تنتقل إلى Gate جديد إذا كان هناك CRITICAL blocker.

إذا لم تتوفر بيئة Windows حقيقية:
نفذ ما تستطيع.
وسجل ما لا يمكن اختباره كـ BLOCKED.
لا تخترع نجاحًا.

إذا واجهت مشكلة في تقنية معينة:
لا تستبدلها بحل وهمي.
اختر بديلًا هندسيًا موثقًا فقط إذا كان يحقق المتطلبات.

الهدف:
MEAAF Windows حقيقي قابل للبناء والصيانة والتطوير التجاري، مع حماية قوية للكود والبيانات والأسرار، وTenant Isolation وRBAC وAudit وOffline First وSync وBackup/Restore وInstaller واختبارات قابلة للإثبات.

============================================================
END OF MASTER PROMPT
============================================================
