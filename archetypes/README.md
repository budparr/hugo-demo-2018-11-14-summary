_Hugo Static Site Generator v0.51/extended darwin/amd64_

I notice that the behavior for `.Summary` is different depending on how it is initiated. If the user adds a `<!--more-->` tag to their content, the `.Summary` is generated in HTML, but if it is automatically generated (by virtue of the fact that the `.Summary` tag is used) it is generated in plain text. 

Because we can't then add the HTML back into the `.Summary` tag, this causes inconsistent results on the front-end and makes certain things (like creating a .Content without .Summary tag) impossible unless one just wants all of their content unformatted. 
