# <h1>Part 1: Create and build a website</h1>
## open on your local machine:

control panel --> programs and features --> add or cancel windows features --> acitvate Internet Information Services --> restart

## install visual studio 2019 and other necessary componets for building your first website

https://visualstudio.microsoft.com/

## install .NET

https://dotnet.microsoft.com/download

## Open Visaul Studio 2019 and Create “ASP.NET Core Web App” project

Check your csproj content --> Add “Newtonsoft.Json” --> Check your csproj again, what changed? --> Restore Nuget Packages --> Compile (rebuild) your project
-->Which files and folders were created? --> Publish your application

## Open IIS on your local machine

create a new application pool without managed code --> add a new website --> mark a physical path --> port number -->browse your website

# Part 2: Create website on your Microsoft server 2019 machine 

## istall IIS to your windows server

Start --> server mananger --> manage --> add roles and features --> next --> next --> web server ( IIS ) --> next --> install --> restart

## Copy you published project 

from C:\Users\User\source\repos\user\user\bin\Release\net5.0\publish to C:\inetpub\wwwroot\user\ of your windows server machine.

## Open IIS

Create a new IIS application pool --> Create website (use port 5100 and your new application pool) -->Copy your website to your windows server --> Browse to “http://localhost:5100/” from your microsoft machine

In some cases things don't work properly and you might get a message


![image text](http://i.stack.imgur.com/vUhK3.png)


if it happens, then follow instructions 

https://forums.asp.net/t/2172068.aspx?ASP+NET+Core+MVC+deploying+to+IIS+Error+Http+Error+500+19+

![image_text](https://img0.etsystatic.com/012/0/5416189/il_570xN.452124294_8p7d.jpg)
