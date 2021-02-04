FROM mcr.microsoft.com/dotnet/sdk:3.1

WORKDIR /api

COPY . .

RUN dotnet restore

RUN dotnet publish -o /publish

WORKDIR /publish

ENTRYPOINT [ "dotnet", "/publish/api.dll" ]