# dotnet-core-5
Dotnet core 5 web.config file setup for publish hosting asp.net

```
<?xml version="1.0" encoding="utf-8"?>
<configuration>
  <location path="." inheritInChildApplications="false">
    <system.webServer>
      <handlers>
        <add name="aspNetCore" path="*" verb="*" modules="AspNetCoreModuleV2" resourceType="Unspecified" />
      </handlers>
      <aspNetCore processPath="dotnet" arguments=".\ECOMMERCE.dll" stdoutLogEnabled="true" stdoutLogFile=".\logs\stdout" hostingModel="inprocess" />
      <modules runAllManagedModulesForAllRequests="true">
        <remove name="WebDAVModule" />
      </modules>
    </system.webServer>
  </location>
  <system.web>
    <compilation tempDirectory="D:\Inetpub\vhosts\e-hishabkhata.com\tmp" />
  </system.web>
</configuration>
<!--ProjectGuid: 5D950EB1-BCCA-4155-B5F6-60CF6A0129D7-->
```
