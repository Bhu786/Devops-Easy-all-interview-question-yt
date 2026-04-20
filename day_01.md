
# entrypoint vs cmd

**ENTRYPOINT vs CMD (short):**

* **ENTRYPOINT** → Fixed main command (container = executable)
* **CMD** → Default arguments or fallback command

**Key Difference:**

* ENTRYPOINT **always runs**
* CMD **can be overridden**

**Best Practice:**

* Use **ENTRYPOINT** for main app
* Use **CMD** for default parameters

👉 Example:

```dockerfile
ENTRYPOINT ["node"]
CMD ["app.js"]
```

Run → `node app.js`
Override → `docker run img server.js` → `node server.js`



write a dockerfile using a linux and a webserver?

what is dokcer home directory 
==> /var/lib/docker

how you will integrate a docker server in jenkins ?
==> add it as a agent to run tasks on the docker server


jenkins :

what is the diff b/w continuous delivery and deployment

how to run a particular stage in jenkins pipelines?

git :
 what will happens if u do git fetch ?

 git fetch + git merge = git pull

 

 
















