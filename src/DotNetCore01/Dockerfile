FROM microsoft/dotnet
COPY . /app
WORKDIR /app
 
RUN dotnet restore
RUN dotnet publish -c Release -o .

EXPOSE 5000
ENV ASPNETCORE_URLS http://*:5000

ENTRYPOINT ["dotnet", "run", "./dotnetapp.dll"]