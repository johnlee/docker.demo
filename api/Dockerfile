FROM microsoft/aspnetcore:2

WORKDIR /app
COPY bin/Debug/netcoreapp2.0/publish .

# the following code is to build the dotnet app inside the container
#COPY . .
#RUN dotnet restore
#RUN dotnet publish -o /publish

ENTRYPOINT ["dotnet", "api.dll" ]