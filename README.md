# MsSQL_Docker
Trainee_Setup

## Docker script (in cmd)
docker run -e "ACCEPT_EULA=Y" -e 'MSSQL_SA_PASSWORD=<YourStrong!Passw0rd>' -p 1433:1433 -v C:/Users/<your_USER_NAME>/Documents/MsSQL/data:/var/opt/mssql/data -v C:/Users/<your_USER_NAME>/Documents/MsSQL/log:/var/opt/mssql/log -v C:/Users/<your_USER_NAME>/Documents/MsSQL/secrets:/var/opt/mssql/secrets -d mcr.microsoft.com/mssql/server:2022-latest

- Vervang <YourStrong!Passw0rd> door een password met 10 karakters en minimaal 1 leesteken, 1 hoofdletter, 1 cijfers
- Vervang *3x* <your_USER_NAME> door je gebruikersnaam

In de map documenten vind je nu een map MsSQL met hierin de data van de container, maak je een nieuwe container aan, dan moet je deze mappen ook verwijderen, anders wordt er weer oude data gebruikt.
