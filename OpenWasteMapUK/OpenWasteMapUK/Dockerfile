FROM mcr.microsoft.com/dotnet/core/sdk
ENV ASPNETCORE_URLS=http://+:5000
ENV ASPNETCORE_ENVIRONMENT=”development”
EXPOSE 5000
WORKDIR /app
COPY . .
RUN dotnet restore && dotnet dev-certs https
# ENTRYPOINT ["dotnet", "run"]