#Project2 - Programming IS601

[Basics of Python programming - Project2](http://projectpython.eastus.azurecontainer.io)

Build and Push to Azure steps:
1.docker context create aci myacicontext
2. docker context use default
3. docker build -t mh637/projectpython .
4. docker push mh637/projectpython
5. docker context use myacicontext
6. docker run --domainname projectpython -dp 80:80 mh637/projectpython