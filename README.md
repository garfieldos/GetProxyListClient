[![Build status](https://ci.appveyor.com/api/projects/status/nhq4kqtgkgofkgn8?svg=true)](https://ci.appveyor.com/project/garfieldos/getproxylistclient)

# GarfSG.GetProxyListClient
Simple C#/.Net Standard wrapper for https://getproxylist.com/ API

## Get it on NuGet:
```
PM> Install-Package GarfSg.GetProxyListClient
```

## Usage
```
var apiKey = "apiKeyFromGetProxyListCom";
var proxyData = new GetProxyListClient(apiKey).GetProxy(new GetProxySearchCriteria
                {
                    AllowsHttps = true,
                    Protocol = new[] { ProtocolEnum.Http }
                });
```

List of all criteria parameters are available here: https://getproxylist.com/#the-api
