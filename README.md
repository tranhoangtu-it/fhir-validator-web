# fhir-validator-web

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000?style=flat-square&logo=flask&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

Web-based HL7 FHIR data validator with support for Japanese Implementation Guides.

## Features

- Validate FHIR resources against standard and custom profiles
- Support for Japanese FHIR IGs: JP-Core, JP-FHIR Terminology, JP-eCSCLINS
- Web UI for easy resource validation
- REST API for programmatic access
- Docker deployment

## Supported Implementation Guides

| IG | Description |
|----|-------------|
| JP-Core | Japan Core FHIR profiles |
| JP-FHIR Terminology | Japanese medical terminology |
| JP-eCSCLINS | Clinical information sharing |

## Tech Stack

- **Backend**: Python Flask
- **Validator**: HL7 FHIR Validator CLI (Java)
- **Frontend**: HTML/CSS/JavaScript
- **Deployment**: Docker

## Prerequisites

- Python 3.8+
- Java 11+ (for FHIR Validator CLI)

## Getting Started

```bash
cd backend && pip install -r requirements.txt
python app.py
```

### Docker

```bash
docker build -t fhir-validator-web .
docker run -p 5000:5000 fhir-validator-web
```

## License

See [LICENSE](./LICENSE) for details.
