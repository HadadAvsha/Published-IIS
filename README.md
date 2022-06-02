# Published IIS
# followd this guide :https://docs.microsoft.com/en-us/visualstudio/get-started/csharp/tutorial-aspnet-core?view=vs-2022
# install VS> Create New Project> (ASP.NET Core Web App)[![asp-net.png](https://i.postimg.cc/FKgwD8WB/asp-net.png)](https://postimg.cc/Z9nfq7h8) in C# for windows platform for web.>assign a project name> Choose .NET 6.0 Framwork
# view code and test by run>ok, if so >publish!
# right click on webapp name and select publish 
# we choose folder> assign location> publish!
# then we go to 'server manager' or to type 'Turn Windows features on or off' in search > add Web Server (IIS) functionality. [![add-IIS.png](https://i.postimg.cc/vm0wGCr6/add-IIS.png)](https://postimg.cc/t1nM5SmX).
# launch IIS Manager create new application pool [![app-pool.png](https://i.postimg.cc/GhDKFNpw/app-pool.png)](https://postimg.cc/56x81svn).
# right click on sites and create add website> name the site> select previously created pool and assign path to app (i created new user for the sole purpose of the site)>test settings> bind address and port.  [![site.png](https://i.postimg.cc/c1929VZv/site.png)](https://postimg.cc/WtZ5tYdV).
# go to the site folder location and right click> properties> security >edit and add the 'IIS AppPool\<myappoolname>' 
[![sec.png](https://i.postimg.cc/vBLhRxpY/sec.png)](https://postimg.cc/KkjBBjGw).
# check the website on http://localhost:5100/ [![done.png](https://i.postimg.cc/BZPYQtHC/done.png)](https://postimg.cc/QVskf86B).