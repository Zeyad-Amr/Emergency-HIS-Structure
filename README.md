# Emergency-HIS-Structure
Hospital Information System for Emergency Departments — registration, triage assessment, examinations, inpatient management.

## Structure
```bash
    src/
    ├── app/                                # Pages named by app routes
    │   ├── home/
    │   ├── about/
    │   ├── contact/
    │   └── .../
    │
    ├── assets/                             # Shared assets (e.g., fonts, images)
    │   ├── fonts/                          # Fonts
    │   ├── data/                           # Data files (e.g., JSON, CSV)
    │   ├── images/                         # Images
    │   ├── illustrations/                  # Illustrations
    │   └── icons/                          # Icons
    │
    │
    ├── config/
    │   ├── env/
    │   │   ├── development.env             # Environment variables for development
    │   │   ├── production.env              # Environment variables for production
    │   │   └── testing.env                 # Environment variables for testing
    │   └── settings/
    │       ├── api-keys.ts                 # API keys
    │       └── app-config.ts               # Application configuration
    │
    ├── core/
    │   ├── _mock/                          # Mock data
    │   ├── api/
    │   │   ├── api-client.ts               # API client
    │   │   ├── config.ts                   # API configuration
    │   │   ├── endpoints.ts                # API endpoints
    │   │   ├── error-code.ts               # API error codes
    │   │   ├── error-message.ts            # API error messages
    │   │   ├── error-response.ts           # API error response
    │   │   └── index.ts                    # API client
    │   ├── auth/                           # Authentication-related code
    │   ├── base/                           # Base classes
    │   ├── components/                     # General Shared UI components
    │   ├── layout/                         # Layout components (e.g., header, footer)
    │   ├── redux/                          # Redux store, reducers, and thunk
    │   │   ├── slices/                     # Redux slices
    │   │   ├── thunks/                     # Redux thunks
    │   │   ├── index.ts                    # Redux provider
    │   │   ├── types.ts                    # Redux types
    │   │   └── store.ts                    # Redux store
    │   ├── routes/                         # Application routes or navigation paths
    │   ├── service-locator/                # Service locator
    │   │   ├── app-service.ts              # Application service
    │   │   ├── index.ts                    # Service locator
    │   │   ├── service-keys.ts             # Service keys
    │   │   └── service-locator.ts          # Service locator
    │   ├── shared/                         # Shared code
    │   │   ├── components/                 # Shared UI components
    │   │   ├── constants/                  # Shared constants
    │   │   ├── hooks/                      # Shared React hooks
    │   │   ├── types/                      # Shared TypeScript types and interfaces
    │   │   └── utils/                      # Shared utility functions and helpers
    │   └── theme/                          # Styling and theming-related files
    │
    ├── modules/
    │   └── auth/
    │      ├── data/
    │      │   ├── datasources/             # Data sources (e.g., API, LocalStorage)
    │      │   ├── models/                  # Data models or structures for data transfer without behavior (e.g., User, Post)
    │      │   └── repositories/            # Data access and storage (e.g., UserRepository)
    │      ├── domain/
    │      │   ├── entities/                # Domain-specific entities with behavior and business rules (e.g., User, Post)
    │      │   ├── interfaces/              # Domain-specific interfaces (e.g., IUserRepository)
    │      │   ├── repositories/            # Abstraction for data access (e.g., UserRepository)
    │      │   ├── contants/               # Domain-specific constants
    │      │   └── usecases/                # Business logic (e.g., Login, Logout)
    │      └── presentation/
    │          ├── pages/                   # Feature-specific pages
    │          ├── components/              # Feature-specific UI components
    │          └── controllers/             # Feature-specific controllers
    │              ├── slices/              # Redux slices
    │              ├── thunks/              # Redux thunk
    │              ├── index.tsx            # Controller for the feature
    │              └── types.ts              # Redux thunk
    │
    └── services/                           # External services or integrations
```

