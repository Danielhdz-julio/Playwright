#  Playwright
Incluye ejecución automatizada, cobertura funcional positiva y negativa, así como generación de evidencia mediante reportes y pipeline de integración continua.
Qué se implementó
Diseño de estrategia de pruebas (Smoke + Regression)
Automatización de pruebas UI (flujo de login)
Automatización de pruebas API (validación de endpoints REST)
Implementación de Page Object Model (POM) para mantenibilidad
Uso de fixtures personalizadas para reutilización de datos
Configuración mediante variables de entorno (.env)
Uso de hooks (beforeEach) para preparación de escenarios
Etiquetado de pruebas (@smoke, @regression)
Generación de reportes HTML como evidencia
Integración con CI/CD (GitHub Actions)
## Stack
- Playwright
- JavaScript
- UI Testing
- API Testing
- Page Object Model
- Fixtures
- Hooks
- Environment variables
- GitHub Actions

## Installation
```bash
npm install
npx playwright install
```

## Setup
1. Copia el archivo `.env.example`
2. Renómbralo a `.env`

## Run tests
### All
```bash
npm test
```

### Smoke
```bash
npm run test:smoke
```

### Regression
```bash
npm run test:regression
```

### UI only
```bash
npm run test:ui
```

### API only
```bash
npm run test:api
```

### Headed mode
```bash
npm run test:headed
```

### Open report
```bash
npm run report
```

## Project structure
```bash
qa-portfolio-evidence/
├── .github/workflows/playwright.yml
├── docs/
│   ├── bug-report-example.md
│   ├── evidence-summary.md
│   ├── test-cases.md
│   └── test-plan.md
├── fixtures/
│   └── test-fixtures.js
├── pages/
│   └── LoginPage.js
├── tests/
│   ├── api/
│   │   └── users.spec.js
│   └── ui/
│       └── login.spec.js
├── utils/
│   └── test-data.js
├── .env.example
├── package.json
└── playwright.config.js
```

## What is covered
### UI
- Successful login
- Invalid username
- Invalid password

### API
- Get all users
- Get user by ID
- Validate 404 for non-existing user

## Why this looks better in a portfolio
- Tiene estructura real
- Separa datos y lógica
- Usa etiquetas smoke y regression
- Incluye evidencia documental
- Tiene pipeline CI
- Se puede enseñar sin andar explicando “luego lo arreglo”

## Recommendation for your evidence
Sube este proyecto a GitHub y agrega:
- Screenshot del reporte HTML
- Screenshot de ejecución en terminal
- Link del repositorio en tu CV
- 2 o 3 bullets en LinkedIn describiendo lo que validaste
