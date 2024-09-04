# capacitacion-netcore
Proyecto para Capacitacion de NetCore

## Comandos utilizados

### EF Migrations

Add
- dotnet ef  migrations add Change --project .\Demo.InfraEstructure --startup-project .\Demo.API (OK)

Update
- dotnet ef database update --project .\Demo.InfraEstructure --startup-project .\Demo.API  (OK)

Remove
- dotnet ef  migrations remove --project .\Demo.InfraEstructure --startup-project .\Demo.API (ok - borrar de la bd primero el registro)

### Coverlet
- dotnet test --collect:"XPlat Code Coverage"
- dotnet test /p:CollectCoverage=true /p:CoverletOutputFormat=opencover

### ReportGenerator
- reportgenerator -reports:"*\TestResults\*\coverage.cobertura.xml" -targetdir:"coveragereport" -reporttypes:Html 