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



![image](https://user-images.githubusercontent.com/41032041/135622938-4b69de6c-7d6a-4fdd-b0cd-696a1a1ec559.png)


![image](https://user-images.githubusercontent.com/41032041/135624153-6272c911-3d10-4e0f-9a64-35f2f5335091.png)

# Add Newtonsoft.Json

![Newtonsoft json](https://user-images.githubusercontent.com/41032041/135624835-1aa9212e-8de5-40cd-bf03-c3caee0cc41e.png)

## Publish the application

![image](https://user-images.githubusercontent.com/41032041/135626511-df29fab2-4735-4beb-b51f-7d30a1f1462f.png)

![image](https://user-images.githubusercontent.com/41032041/135626998-c45ff38a-4546-41da-bc7f-67229d28d8a5.png)

#### ont the server we install IIS and dotnet-hosting-5.0.10-win, create an application Pool, 

![application pool](https://user-images.githubusercontent.com/41032041/135628580-90178bcb-d055-4023-8829-96bde3728226.png)

#### adding the website

![add website](https://user-images.githubusercontent.com/41032041/135629365-27cce754-8f52-4b7b-92c5-e7e5499c957e.png)

![choosing the application pool](https://user-images.githubusercontent.com/41032041/135630277-92912d4f-9ea3-4cd7-a1b9-dea472718bc3.png)

![add website2](https://user-images.githubusercontent.com/41032041/135631904-c8ae2489-53fa-4480-9d0f-9d41ef2903a4.png)



### Running with IIS and after compilation the code is up.

![image](https://user-images.githubusercontent.com/41032041/135627218-953d8d6f-e502-42f1-933a-a967cdc4c2c6.png)


![image_text](https://img0.etsystatic.com/012/0/5416189/il_570xN.452124294_8p7d.jpg)
