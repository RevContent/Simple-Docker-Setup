### Docker Setup
This is a simple docker setup for running a basic nginx server. To get started, install [docker desktop](https://www.docker.com/get-started).

Next, go into the command line and enter the proxy folder, then run `docker-compose up -d` to build the reverse proxy for resolving test urls. Once that has completed, go back out to the root working directory and run `docker-compose up -d` again to build the docker container

NOTE: You will need to add `my-app.local` to your hosts file. You can edit this by running `sudo vi /etc/hosts` on a mac or finding `C:\Windows\System32\Drivers\etc\hosts` in Windows. Make sure this is pointing to 127.0.0.1

Once that is done, you should be able to go to `my-app.local` in your browser and see the test page. You can change this domain to whatever you desire, but it must be done prior to creating the second docker container or you must run `docker-compose up -d` again after changing it.
Once that is done, you should be able to go to `my-app.local` in your browser and see the test page. You can change this domain to whatever you desire, but it must be done prior to creating the second docker container or you must run `docker-compose up -d` again after changing it.
