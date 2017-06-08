# http-test

## How to use it:

# - create a new-project
> # oc new-project s2i-http

# - create the ImageStream from the template s2i-is.json
> # oc create -f s2i-is.json 
 
# - create the app using index.html in the repo
> # oc new-app httpd:2.4~https://github.com/niconosenzo/http-test.git --strategy=source --name=httpd-test


