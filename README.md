part 0.4

![image](https://user-images.githubusercontent.com/7853541/188973993-a35fff1e-ac1a-4022-a74a-6418f9df62bf.png)

  Browser->Server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note 
  note over Browser: Browser:payload:  textfield data 
  Server-->Browser: HTTP status code 302 

  Browser->Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes 
  Server-->Browser: HTML-code 
  Browser->Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css 
  Server-->Browser: main.css 
  Browser->Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js 
  Server-->Browser: main.js 

  note over Browser:
  browser starts executing js-code
  that requests JSON data from server 
  end note

  Browser->Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
  Server-->Browser: [Json Data]




part 0.5

![image](https://user-images.githubusercontent.com/7853541/188973924-ca6b44ba-1b78-4592-93df-2a5c0568843f.png)

  browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa
  server-->browser: HTML-code
  browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
  server-->browser: main.css
  browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa.js
  server-->browser: spa.js
  note over browser:
  browser starts executing js-code
  that requests JSON data from server 
  end note
  browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
  server-->browser: json data


part 0.6

![image](https://user-images.githubusercontent.com/7853541/188974275-15eaeefa-d69c-4a95-898e-8a289d1fca4e.png)

  browser->server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
  note over browser:
  payload: json {content:...,date:....}
  end note
  note over browser:
  browser starts executing js-code to render changes on state change
  end note



