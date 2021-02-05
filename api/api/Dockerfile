# Build Stage
FROM mcr.microsoft.com/dotnet/sdk:3.1 AS build-env
WORKDIR /api

COPY api.csproj .
RUN dotnet restore

COPY . .
RUN dotnet publish -c Release -o /out

# Runtine Image Stage
FROM mcr.microsoft.com/dotnet/aspnet:3.1
WORKDIR /out
COPY --from=build-env /out .
ENTRYPOINT [ "dotnet", "api.dll" ]