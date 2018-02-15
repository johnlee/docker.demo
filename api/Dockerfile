FROM microsoft/aspnetcore:2

WORKDIR /app
COPY bin/Debug/netcoreapp2.0/publish .

ENTRYPOINT ["dotnet", "api.dll" ]

# # copy csproj and restore as distinct layers
# COPY *.csproj ./
# RUN dotnet restore

# # copy everything else and build
# COPY . ./
# RUN dotnet publish -c Release -o out

# # build runtime image
# FROM microsoft/dotnet:2.0-runtime 
# WORKDIR /app
# COPY --from=build-env /app/out ./
# ENTRYPOINT ["dotnet", "api.dll"]