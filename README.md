# Clean_Architecture_HelloWorld_MySQL


      optionsBuilder.UseMySql(
          _configuration.GetConnectionString("DefaultConnection"),
          ServerVersion.AutoDetect(_configuration.GetConnectionString("DefaultConnection")),
          x => x.MigrationsHistoryTable("__EFMigrationsHistory")
        );


{
  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft": "Warning",
      "Microsoft.Hosting.Lifetime": "Information"
    }
  },
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Database=CleanArchitecture;User=root;Password=IOTCloudRobomatics;TreatTinyAsBoolean=true;"
  },
  "AllowedHosts": "*"
}




CREATE TABLE Person (
    Id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
    FirstName VARCHAR(100) NOT NULL,
    LastName VARCHAR(100) NOT NULL,
    Active BOOLEAN NOT NULL,
    CreatedBy INT NOT NULL,
    CreatedOn DATETIME NOT NULL,
    ModifiedBy INT,
    ModifiedOn DATETIME
);

https://localhost:5001/api/v1.0/people

[{"id":1,"firstName":"Brandon","lastName":"Smith","active":true,"createdBy":1,"createdOn":"2023-11-22T02:52:37","modifiedBy":null,"modifiedOn":null}]

![image](https://github.com/junxian428/Clean_Architecture_HelloWorld_MySQL/assets/58724748/2d9dca59-3e91-4b5a-98cb-7586f3cb3853)

![image](https://github.com/junxian428/Clean_Architecture_HelloWorld_MySQL/assets/58724748/cdc44ff5-7253-49b6-9a5f-53bd3cbfacf3)
