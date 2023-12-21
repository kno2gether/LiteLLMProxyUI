![](http://kno2gether.com/wp-content/uploads/2023/09/cropped-ideogram-4_clipdrop-background-removal_clipdrop-relight.png)

This app is built using Appsmith by Kno2gether. This is a simple UI to manage LiteLLM Proxy configuration. This UI is designed to simplify and ease developer life to manage their AI API locally through LiteLLM through UI.
More features are to be added, such as KEY MANAGEMENT, Budget Management. 

PR is Welcome.

** Installation Steps (Using Docker)

* Step-1
Install AppSmith community Edition (For Free).
Create a folder(For eg. LLMProxyUI)
Go inside LLMProxyUI
```
cd LLMProxyUI
```
create a docker-compose.yml file
```
version: "3"
services:
   appsmith:
     image: index.docker.io/appsmith/appsmith-ce
     container_name: appsmith
     ports:
         - "8081:80"
         - "8443:443"
     volumes:
         - ./stacks:/appsmith-stacks
     restart: unless-stopped
```
This will ensure when docker will be run, your appsmit instance will be available in 8081 or 8443 (https) port.

* Step-2
  Start Appsmith.
  ```
  docker-compose up -d
  ```
* Step-3
Clone this repository
```
git clone https://github.com/kno2gether/LiteLLMProxyUI.git
```

* Step-4
Load AppSmith on your browser http://localhost:8081


*Step-5
Finish up the sign up process and then click on the App menu on Right Top using (...) then click Import and then Select ```LiteLLM Proxy UI by Kno2gether.json``` file from cloned repository.
![](https://github.com/kno2gether/LiteLLMProxyUI/blob/master/appsmith_import.png)

*Step-6
Now your App is ready. Just Click Deploy.

*Step-7
Provide LiteLLM Proxy URL and Optional UserKey and then you can use the UI to manade Models and routes of your LiteLLM Proxy using this simple UI.


[For more detailed Tutorial check out the video in our youtube Channel. ](https://www.youtube.com/watch?v=-Wo025I-_I4)


![](https://raw.githubusercontent.com/appsmithorg/appsmith/release/static/images/integrations.png)

• [Our Website](https://kno2gether.com)  • [Tutorials](https://www.youtube.com/watch?v=-Wo025I-_I4) • [Youtube]([https://www.youtube.com/channel/UCxgkN3luQgLQOd_L7tbOdhQ])

