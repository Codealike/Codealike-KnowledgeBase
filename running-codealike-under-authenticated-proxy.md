##Running Codealike under an authenticated proxy##

Locate the Codealike extension directory. [[1]](https://github.com/Codealike/Codealike-KnowledgeBase/blob/master/locate-codealike-extension.md)

Open the `web.config` file and add the following:

```
<system.net> 
    <defaultProxy useDefaultCredentials="true" /> 
</system.net> 
```

Make sure that the proxy credentials are also stored in Internet Explorer. While it may seem strange, the issue is that there is currently not known way to store the internet proxy credentials system-wide if they are not being setup by IE.

 We would be grateful to know further if you find a workaround. 