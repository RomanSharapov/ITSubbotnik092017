Imagine yourself on an inhabitant server. You have:
- ./jenkins_home folder with 770 permissions and owner:group 1001:1001
- No root access to the server
- Only one docker image. New images creation allowed

You need to start and login to the instance with itsubbotnik:Pa$$w0rd! credentials. This user creds stored in Jenkins's user database.

Try to start with:
docker run -p 8080:8080 -p 50000:50000 -v `pwd`/jenkins_home:/var/jenkins_home romansharapov/itsubbotnik:jenkins

Developers are waiting. Hurry up!