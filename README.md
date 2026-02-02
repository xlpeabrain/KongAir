## API Ops sample project for Kong EE

Prerequisites:
- Running Kong Enterprise
- Pre-created a workspace called flights-team
- RBAC token created for user with write access to Kong workspace
- Running a self-hosted runner tagged as 'self-hosted'

The folders to note are:

.github/workflows - contains the definitions of the pipeline jobs
flight-data/*/openapi.yaml - the OpenAPI specifications (Swagger) for the application services
platform/kong - this folder contains the kong entities that the platform team would define, eg global plugins
PRD/kong - pipeline jobs will generate the complete workspace definition here 
