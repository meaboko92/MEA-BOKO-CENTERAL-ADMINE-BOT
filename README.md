🚀 MEA BOKO CENTRAL ADMIN — MASTER BUILD PROMPT

1. PROJECT IDENTITY

Build a complete, modular, scalable central administration platform named:

MEA BOKO CENTRAL ADMIN

Repository:

MEA-BOKO-CENTRAL-ADMIN

Codespace:

mea-boko-central-admin

Brand/platform concept:

MEA BOKO — GENERAL DIGITAL MARKET B2B + AI BUSINESS CENTRAL

Main purpose:

Create ONE central system that manages MEA BOKO's business, marketplace, bots, APIs, AI, database, CRM, payments, marketing, communications, analytics, automation, and integrations.

Do NOT create disconnected mini-projects.

Use one central backend and one central database architecture.

---

2. IMPORTANT FIRST INSTRUCTION

Before creating or changing code:

1. Inspect the entire repository.
2. Inspect all existing files.
3. Identify existing MEA BOKO code.
4. Identify existing Telegram bot code.
5. Identify existing FastAPI code.
6. Identify existing database models.
7. Identify existing configuration.
8. Identify duplicate functionality.
9. Preserve useful existing code.
10. Do NOT blindly overwrite working files.
11. Create a clear implementation plan.
12. Then implement the system.
13. Run tests.
14. Fix errors.
15. Verify that the application starts successfully.

If the repository is empty, create the complete project from scratch.

---

3. CENTRAL ARCHITECTURE

Build this architecture:

                     MEA BOKO CENTRAL ADMIN
                              │
                              ▼
                     CENTRAL ADMIN DASHBOARD
                              │
                              ▼
                     FASTAPI CENTRAL CORE
                              │
    ┌─────────────────────────┼─────────────────────────┐
    │                         │                         │
    ▼                         ▼                         ▼

DATABASE HUB                AI HUB                  BOT HUB
PostgreSQL             OpenAI / Gemini             Telegram
│                         │                         │
└─────────────────────────┼─────────────────────────┘
│
┌───────────────┬──────────┼──────────┬───────────────┐
▼               ▼          ▼          ▼               ▼
Marketplace         CRM       Payments   Marketing    Communication
│               │          │          │               │
└───────────────┴──────────┴──────────┴───────────────┘
│
AUTOMATION
│
ANALYTICS

FastAPI is the central integration layer.

PostgreSQL is the central operational database.

The Admin system controls the platform.

---

4. CORE TECHNOLOGY

Use:

- Python 3.12+
- FastAPI
- Uvicorn
- PostgreSQL
- SQLAlchemy 2.x
- Alembic
- Pydantic v2
- pydantic-settings
- httpx
- JWT authentication
- secure password hashing
- pytest
- Docker
- Docker Compose

Use asynchronous programming where appropriate.

Keep the architecture simple.

Start as a modular monolith.

Do NOT create unnecessary microservices.

---

5. PROJECT STRUCTURE

Create a clean structure:

MEA-BOKO-CENTRAL-ADMIN/

├── app/
│   ├── main.py
│   ├── config.py
│   ├── database.py
│   │
│   ├── api/
│   │   └── v1/
│   │       ├── router.py
│   │       ├── auth.py
│   │       ├── users.py
│   │       ├── companies.py
│   │       ├── marketplace.py
│   │       ├── products.py
│   │       ├── buyers.py
│   │       ├── sellers.py
│   │       ├── exporters.py
│   │       ├── importers.py
│   │       ├── coffee.py
│   │       ├── machinery.py
│   │       ├── vehicles.py
│   │       ├── gemstones.py
│   │       ├── real_estate.py
│   │       ├── leads.py
│   │       ├── customers.py
│   │       ├── orders.py
│   │       ├── payments.py
│   │       ├── ai.py
│   │       ├── telegram.py
│   │       ├── marketing.py
│   │       ├── notifications.py
│   │       ├── analytics.py
│   │       ├── automation.py
│   │       ├── integrations.py
│   │       ├── admin.py
│   │       ├── system.py
│   │       ├── webhooks.py
│   │       └── health.py
│   │
│   ├── models/
│   ├── schemas/
│   ├── services/
│   ├── integrations/
│   ├── security/
│   ├── admin/
│   ├── workers/
│   └── utils/
│
├── frontend/
│   └── admin-dashboard/
│
├── alembic/
├── tests/
├── scripts/
├── docs/
├── .env.example
├── .gitignore
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md

Organize files logically.

Do not put the entire application into one Python file.

---

6. CENTRAL ADMIN DASHBOARD

Create a central dashboard containing:

Dashboard

Show:

- total users
- active users
- companies
- buyers
- sellers
- exporters
- importers
- products
- leads
- orders
- payments
- revenue/commission statistics
- AI usage
- bot status
- API status
- database status
- integration status
- recent activity
- notifications
- errors

Use cards, tables, charts, filters, and status indicators.

---

7. MAIN ADMIN MENU

Create the central menu:

🏠 Dashboard

👥 Users & Customers

🏢 Companies

🌍 Marketplace

☕ Coffee Market

💎 Gemstone Market

🏗 Machinery

🚗 Vehicles

🏠 Real Estate

📦 Products

🛒 Buyers

🏭 Sellers

🌎 Exporters

📥 Importers

🎯 Leads / CRM

📋 Orders

💳 Payments

🤖 AI HUB

📱 Telegram / Bots

📣 Marketing & Social

📧 Communication

📊 Analytics

⚙️ Automation

🔌 API & Integrations

🔐 Security

📝 Audit Logs

⚙️ System Settings

---

8. API CENTER

Create:

API & INTEGRATION CENTER

Endpoint prefix:

"/api/v1"

Main groups:

/auth
/users
/companies
/products
/marketplace
/buyers
/sellers
/exporters
/importers
/coffee
/machinery
/vehicles
/gemstones
/real-estate
/leads
/customers
/orders
/payments
/ai
/telegram
/marketing
/notifications
/analytics
/automation
/integrations
/admin
/system
/webhooks
/health

Every module must have clean schemas, validation, authentication and authorization.

---

9. USER MANAGEMENT

Create users with:

- UUID
- name
- username
- email
- phone
- country
- city
- account type
- status
- verification
- role
- created_at
- updated_at

Roles:

SUPER_ADMIN
ADMIN
MANAGER
MARKETING_MANAGER
SALES_MANAGER
BROKER
AGENT
EXPORTER
IMPORTER
BUYER
SELLER
CUSTOMER
VIEWER

Implement RBAC.

---

10. COMPANY MANAGEMENT

Companies must support:

- company name
- registration information
- country
- city
- address
- business type
- industry
- contact person
- email
- phone
- website
- verification status
- products
- buyers/sellers
- documents
- notes

---

11. B2B MARKETPLACE

Build a general marketplace.

Categories must support:

☕ Coffee

💎 Gemstones

🏗 Machinery

🚜 Construction Equipment

🛵 Motorcycles

🛺 Electric Tricycles

🚗 Vehicles

🏠 Real Estate

🏭 Industrial Products

🌾 Agricultural Products

🛢 Oil / Industrial Materials

🧴 Cosmetics

🔩 Metals / Materials

📦 General Products

Allow future categories without changing the core architecture.

---

12. PRODUCT MANAGEMENT

Product fields:

- title
- description
- category
- subcategory
- seller
- country
- region
- city
- quantity
- unit
- price
- currency
- minimum order quantity
- availability
- verification
- images
- documents
- specifications
- created_at
- updated_at

Implement:

Create
Read
Update
Delete
Search
Filter
Pagination
Verification
Publish/unpublish

---

13. COFFEE MARKET MODULE

Create a dedicated Ethiopian coffee marketplace module.

Support:

- origin
- region
- zone
- woreda
- coffee type
- variety
- processing method
- washed
- natural
- honey
- grade
- altitude
- harvest year
- quantity
- price
- currency
- certification
- supplier
- exporter
- buyer
- sample information

Allow Ethiopian origins to expand without changing the core system.

---

14. GEMSTONE MODULE

Support gemstone listings including:

- gemstone type
- origin
- location
- rough/cut
- weight
- carat
- color
- clarity
- treatment
- certification
- price
- currency
- seller
- verification

---

15. MACHINERY MODULE

Support:

- excavators
- loaders
- tractors
- coffee machinery
- mining machinery
- construction machinery
- industrial machinery
- spare parts

Fields:

brand
model
year
condition
capacity
location
price
currency
sale/rent
seller
availability

---

16. VEHICLE MODULE

Support:

- motorcycles
- electric tricycles
- Bajaj-type vehicles
- cars
- commercial vehicles
- trucks

Include:

brand
model
year
condition
engine/electric specifications
price
currency
location
seller
availability

---

17. REAL ESTATE MODULE

Support:

- houses
- shops
- warehouses
- land
- offices
- commercial buildings

Location hierarchy:

country
region/state
city
zone
woreda
neighborhood

---

18. CRM / LEADS

Build a CRM.

Lead statuses:

NEW
CONTACTED
QUALIFIED
NEGOTIATION
WON
LOST
ARCHIVED

Fields:

- lead source
- customer
- product
- assigned agent
- priority
- notes
- next action
- follow-up date
- status

---

19. ORDERS

Order workflow:

DRAFT
PENDING
CONFIRMED
PROCESSING
COMPLETED
CANCELLED

Order must reference:

buyer
seller
product
quantity
price
currency
commission
status

---

20. PAYMENT HUB

Create payment abstraction.

Support:

Chapa
PayPal
Future providers

Functions:

initialize payment
verify payment
transaction record
payment status
webhook
refund architecture
commission calculation

Never store card numbers.

Never expose payment secrets.

---

21. AI HUB

Create one AI gateway.

Providers:

OpenAI/ChatGPT
Google Gemini
Future AI providers

Create:

POST /api/v1/ai/chat
POST /api/v1/ai/translate
POST /api/v1/ai/analyze
POST /api/v1/ai/content
POST /api/v1/ai/market-research

AI tasks:

- customer support
- translation
- market research
- product descriptions
- marketing content
- lead analysis
- business analysis
- document assistance
- marketplace search
- business matching

Use an AI provider abstraction.

Do not hard-code one AI provider into the whole application.

---

22. TELEGRAM / BOT HUB

Create:

MEA BOKO BOT HUB

Manage:

- Main MEA BOKO Bot
- Admin Bot
- future bots
- Telegram channels
- webhook status
- bot health
- notifications
- commands

Architecture:

Telegram
↓
FastAPI
↓
Services
↓
Database

Do NOT make Telegram handlers contain the main business logic.

---

23. ADMIN BOT COMMANDS

Create commands:

/start
/admin
/dashboard
/users
/companies
/market
/products
/buyers
/sellers
/exporters
/importers
/leads
/orders
/payments
/ai
/marketing
/analytics
/automation
/api
/security
/logs
/health
/settings

The most important new command:

/api

It opens:

🔌 API & INTEGRATIONS CENTER

- FastAPI
- Bot Integrations
- AI
- Database
- Marketplace
- Payments
- Marketing
- Notifications
- Webhooks
- Security
- System
- Logs
- Health

---

24. MARKETING HUB

Centralize marketing management.

Support architecture for:

Facebook
Instagram
YouTube
TikTok
Telegram
Email

Functions:

- campaign management
- content management
- publishing queue
- hashtags
- target audience
- campaign analytics
- lead source tracking

Do not fake publishing if an external API is not configured.

Return:

NOT_CONFIGURED

when necessary.

---

25. COMMUNICATION HUB

Support:

Telegram
Email
Future SMS

Create notifications with:

recipient
channel
subject
message
status
provider
created_at

Statuses:

PENDING
SENT
FAILED

---

26. ANALYTICS HUB

Dashboard analytics:

- users
- registrations
- products
- marketplace activity
- buyers
- sellers
- exporters
- importers
- leads
- conversions
- orders
- payments
- commissions
- AI usage
- marketing performance
- bot activity

Create reusable analytics services.

---

27. AUTOMATION HUB

Create an automation framework for:

- scheduled tasks
- lead follow-ups
- notifications
- product updates
- marketing workflows
- AI workflows
- payment notifications
- reminders
- reporting

Do not create unsafe autonomous financial actions.

Require appropriate permissions for sensitive operations.

---

28. DATABASE

Use PostgreSQL.

Create models for:

users
roles
permissions
companies
products
categories
coffee_origins
gemstones
machinery
vehicles
real_estate
buyers
sellers
exporters
importers
customers
leads
orders
payments
messages
notifications
ai_requests
marketing_campaigns
automation_jobs
api_integrations
webhook_events
audit_logs

Use:

UUIDs
timestamps
indexes
foreign keys
constraints
soft deletion where appropriate

Use Alembic migrations.

---

29. API INTEGRATIONS

Create an integration registry.

Each integration should have:

name
provider
status
configuration status
last checked
error status
created_at
updated_at

Possible integrations:

Telegram
OpenAI
Gemini
Chapa
PayPal
Email
Facebook
Instagram
YouTube
TikTok
Google services
Future APIs

Never expose secrets.

Show:

🟢 CONFIGURED

or

🔴 NOT CONFIGURED

instead of displaying credentials.

---

30. SECURITY

Implement:

JWT authentication
RBAC
password hashing
CORS
request validation
rate-limit architecture
webhook verification
audit logging
secure headers
secret management

Sensitive actions require proper permissions.

Never expose:

API keys
bot tokens
database passwords
payment secrets

---

31. AUDIT LOG

Record administrative actions:

LOGIN
LOGOUT
USER_CREATED
USER_UPDATED
ROLE_CHANGED
PRODUCT_CREATED
PRODUCT_UPDATED
PRODUCT_DELETED
PAYMENT_CREATED
PAYMENT_VERIFIED
INTEGRATION_CHANGED
SETTINGS_CHANGED

Never log secret values.

---

32. HEALTH CENTER

Create:

"GET /api/v1/health"

Check:

API
Database
Telegram
OpenAI
Gemini
Chapa
PayPal
Email

Return safe status only.

---

33. SYSTEM SETTINGS

Central settings:

platform name
platform description
default currency
supported currencies
languages
timezone
contact information
notification settings
marketplace settings
commission settings
AI settings
security settings

Never store secrets as ordinary public settings.

---

34. MULTILINGUAL ARCHITECTURE

Prepare the system for:

English
Amharic
Oromo
Sidama
Gedeo
Arabic
Chinese
and additional languages.

Do not hard-code all user-facing text into business logic.

Use a translation/i18n structure.

---

35. SEARCH

Create global search architecture.

Search:

users
companies
products
buyers
sellers
exporters
importers
leads
orders

Support filters and pagination.

---

36. DOCUMENTS / FILES

Create safe file/document architecture for:

business documents
certificates
product documents
export documents
company documents

Do not expose private documents publicly.

Use metadata and controlled access.

---

37. ENVIRONMENT VARIABLES

Create ".env.example".

Include placeholders:

DATABASE_URL=
SECRET_KEY=
JWT_SECRET_KEY=

TELEGRAM_BOT_TOKEN=
TELEGRAM_ADMIN_BOT_TOKEN=

OPENAI_API_KEY=
GEMINI_API_KEY=

CHAPA_SECRET_KEY=
CHAPA_PUBLIC_KEY=

PAYPAL_CLIENT_ID=
PAYPAL_CLIENT_SECRET=

SMTP_HOST=
SMTP_PORT=
SMTP_USERNAME=
SMTP_PASSWORD=

FACEBOOK_ACCESS_TOKEN=
INSTAGRAM_ACCESS_TOKEN=
YOUTUBE_API_KEY=
TIKTOK_API_KEY=

APP_ENV=development
DEBUG=true

Never commit ".env".

---

38. DOCKER

Create:

Dockerfile

docker-compose.yml

Services:

api
postgres

Make:

docker compose up --build

start the development environment.

---

39. TESTING

Create tests for:

authentication
RBAC
users
companies
products
marketplace
coffee
buyers
sellers
exporters
importers
leads
orders
payments
AI gateway
Telegram
webhooks
analytics
audit logs
health

Use mocks for external APIs.

Tests must not require real API credentials.

---

40. DOCUMENTATION

Create a complete README explaining:

- MEA BOKO Central Admin
- architecture
- installation
- environment variables
- database
- migrations
- API
- Admin Bot
- AI
- marketplace
- payments
- marketing
- testing
- Docker
- deployment
- security

Create additional documentation under:

"docs/"

including:

architecture
API
database
integrations
security
deployment
Admin Bot

---

41. DEVELOPMENT PHASES

Implement in this order:

PHASE 1

Repository inspection
Architecture
FastAPI
Configuration
Database
Health

PHASE 2

Models
Schemas
Alembic
CRUD

PHASE 3

Authentication
RBAC
Admin

PHASE 4

Marketplace
Products
Coffee
Gemstones
Machinery
Vehicles
Real Estate

PHASE 5

Buyers
Sellers
Exporters
Importers
Customers

PHASE 6

CRM
Leads
Orders

PHASE 7

AI HUB

PHASE 8

Telegram / Bot HUB

PHASE 9

Payments

PHASE 10

Marketing / Social

PHASE 11

Notifications

PHASE 12

Analytics

PHASE 13

Automation

PHASE 14

Security
Webhooks
Audit logs

PHASE 15

Tests
Docker
Documentation
Deployment preparation

---

42. CODING AGENT RULES

When working on the project:

1. Inspect before modifying.
2. Explain the implementation plan briefly.
3. Work incrementally.
4. Preserve working code.
5. Avoid unnecessary rewrites.
6. Reuse existing models where possible.
7. Use migrations for database changes.
8. Run tests after major changes.
9. Fix errors rather than hiding them.
10. Never fake an integration.
11. Never hard-code secrets.
12. Never expose credentials.
13. Keep APIs versioned.
14. Keep business logic in services.
15. Keep Telegram handlers thin.
16. Keep database logic centralized.
17. Keep integrations modular.
18. Write documentation for major features.

---

43. FINAL ACCEPTANCE TEST

The system is considered successfully built only when:

- FastAPI starts
- PostgreSQL connects
- migrations work
- "/docs" works
- "/api/v1/health" works
- authentication works
- RBAC works
- Admin dashboard works
- Admin Bot architecture works
- "/api" command exists
- marketplace works
- products work
- coffee module works
- buyers/sellers/exporters/importers work
- CRM works
- leads work
- orders work
- AI gateway works with configured/mock providers
- Telegram integration works or clearly reports NOT_CONFIGURED
- payment architecture works or clearly reports NOT_CONFIGURED
- marketing integrations are modular
- notifications work
- analytics works
- automation framework works
- audit logs work
- tests pass
- Docker works
- README is complete
- no secrets are committed

---

44. FINAL GOAL

The final platform must function as:

MEA BOKO GENERAL DIGITAL MARKET B2B + AI BUSINESS CENTRAL

with one central administration system controlling:

BUSINESS + MARKETPLACE + BOTS + API + AI + DATABASE + CRM + PAYMENTS + MARKETING + COMMUNICATION + ANALYTICS + AUTOMATION + SECURITY

Use a modular monolithic architecture now.

Keep it simple enough to develop and maintain.

Make it scalable enough to become the main backend of the MEA BOKO ecosystem.

Do not build unnecessary separate applications.

Build one strong central system first.
