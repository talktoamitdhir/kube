FROM mcr.microsoft.com/dotnet/aspnet:3.1

WORKDIR /api

COPY bin/Debug/netcoreapp3.1/publish .

ENTRYPOINT [ "dotnet", "/api/api.dll" ]