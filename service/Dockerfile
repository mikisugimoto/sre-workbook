FROM mcr.microsoft.com/dotnet/sdk:5.0 AS build-env

COPY /src/ToDoApi/ToDoApi.csproj /src/ToDoApi/ToDoApi.csproj
RUN dotnet restore /src/ToDoApi/ToDoApi.csproj

COPY src src
WORKDIR /src
RUN dotnet build ./ToDoApi/ToDoApi.csproj -c Release -o /app/build
RUN dotnet publish ./ToDoApi/ToDoApi.csproj -c Release -o /app/publish

FROM mcr.microsoft.com/dotnet/aspnet:5.0 as final
WORKDIR /app

COPY --from=build-env /app/publish .

ENTRYPOINT ["dotnet"]
CMD ["ToDoApi.dll"]
