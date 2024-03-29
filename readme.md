# redcap-testing-spec
Cypress project for redcap testing:

- system config
- em config
- (projects)


## Setup

Clone repository:
```bash
git clone https://github.com/tertek/redcap-testing-spec.git
cd redcap-dev-spec
```

Install npm dependencies and Cypress client:
```bash
npm install
.\node_modules\.bin\cypress install
```

## Configure

Create Cypress Config `cypress.env.json`,
for example:
```json
{
    "environment": "local",
    "version": "13.1.32",
    "username": "username",
    "password": "password",
    "api_token": "api-token"
}
```

Ensure required permissions are set within project directory:
- Directory /cypress/downloads needs to be writable
- Directory /cypress/fixtures needs to be readable

## Usage

Open in Cypress Client:
```bash
.\node_modules\.bin\cypress open
```

Headless with calling reports::
```bash
.\node_modules\.bin\cypress run
```

## Troublshooting
In case of errors, clear cache:
```bash
.\node_modules\.bin\cypress cache clear
```


