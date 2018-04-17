# Proxy at Work

Configure proxy settings for GIT, npm, chocolatey, yarn, nuget, bower and manny other.
You can write your proxy data settings like host:port username, password using most common sources.

## Features
Configure easily a big list of applications
* GIT - https://git-scm.com
* NPM - https://www.npmjs.com
* Chocolatey - https://chocolatey.org
* Yarn - https://yarnpkg.com
* Nuget - https://www.nuget.org
* Bower - https://bower.io
* Ruby gen - https://rubygems.org
* Gradle - https://gradle.org/
* Ionic - https://ionicframework.com
* Cordova - https://cordova.apache.org
* Android SDK - https://developer.android.com/studio
* Visual Studio - https://www.visualstudio.com
* Angular CLI - https://cli.angular.io
* Yoeman - http://yeoman.io
* All browsers - https://en.wikipedia.org/wiki/List_of_web_browsers
* And much more

## Behavior

> Only the variable **PROXY_HOST** and **PROXY_PORT** are required the others varibles are optional.

> Add Windows and Generic credentials at control panel

> Configure proxy and exceptions at Internet Settings on control panel

> Optionally install an cntlm windows service to relay NTLMv2 authentication on 127.0.0.1:3128 (localhost)

> You can use special characters in your password that the application will encode automatically when being necessary.

## Future implementation
* Add Visual studio code user settings
* Cntlm

## Sources available

* Command line arguments
* Environment Variables
* INI files
* Json files
* XML configuration files

### Use with command line argument
```html
proxy-at-work.exe PROXY_DOMAIN=<type-proxy-host> PROXY_USERNAME=[type-proxy-username] PROXY_PASSWORD=[type-proxy-password] PROXY_HOST=<type-proxy-port> PROXY_EXCEPTIONS=[type-proxy-url-exceptions]
```

You can use the example **run.cmd** file to run the application and also create copy of this for differents profiles.
```html
run.cmd
```

### Use with environment variable
1. Access control panel
2. System and Security
3. System
4. Advanced system settings
5. Environment variables
6. Add follow the variables
    * PROXY_DOMAIN
    * PROXY_USERNAME
    * PROXY_PASSWORD
    * PROXY_HOST
    * PROXY_PORT
    * PROXY_EXCEPTIONS
7. Ok (twice)
8. Run the application `proxy-at-work.exe`


### INI file
1. Open the file settings.ini
2. Fill the follow the variables
    * PROXY_DOMAIN
    * PROXY_USERNAME
    * PROXY_PASSWORD
    * PROXY_HOST
    * PROXY_PORT
    * PROXY_EXCEPTIONS
3. Run the application `proxy-at-work.exe`

### Json file
1. Open the file settings.json
2. Fill the follow the variables
    * PROXY_DOMAIN
    * PROXY_USERNAME
    * PROXY_PASSWORD
    * PROXY_HOST
    * PROXY_PORT
    * PROXY_EXCEPTIONS
3. Run the application `proxy-at-work.exe`

### XML configuration file
1. Open the file proxy-at-work.exe.config
2. Fill the follow the variables at appSettings section
    * PROXY_DOMAIN
    * PROXY_USERNAME
    * PROXY_PASSWORD
    * PROXY_HOST
    * PROXY_PORT
    * PROXY_EXCEPTIONS
3. Run the application `proxy-at-work.exe`
yo 
## Releases

Get the portable version
* Version 1.3.0 - https://github.com/jefersonsv/proxy-at-work/releases/tag/1.3.0

## What's cntlm?
Cntlm is an NTLM / NTLMv2 authenticating HTTP/1.1 proxy. It caches auth'd connections for reuse, offers TCP/IP tunneling (port forwarding) thru parent proxy and much much more. It's in C, very fast and resource-efficient. Go to http://cntlm.sf.net/

## Who I am?
* http://linkedin.com/in/jefersontenorio

## License

Apache-2.0 https://github.com/jefersonsv/proxy-at-work/blob/master/LICENSE

## Thanks to
* https://github.com/aloneguid/config
* https://github.com/Tyrrrz/CliWrap
* https://github.com/NLog/
* https://stackoverflow.com/questions/197725/programmatically-set-browser-proxy-settings-in-c-sharp
* http://credentialmanagement.codeplex.com/
* http://cntlm.sf.net/