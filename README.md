# custom-templates-portainer
# Creating your own templates in portainer

##Resources
* [Deploy Portainer](https://portainer.readthedocs.io/en/latest/deployment.html)
* [Documentation](https://portainer.readthedocs.io)

##Ways to create your own templates
#Using the settings section in Portainer UI 
* Create JSON file where you can describe your templates. 
  How to write this file you can find here: https://portainer.readthedocs.io/en/latest/templates.html
* Upload this file in GitHub for example so that you can access it with URL
  **Starting Portainer :**
* docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer
* access Portainer by pointing your web browser at http://DOCKER_HOST:9000
* in portainer UI you go in Settings and write URL with your templates
  <img src="https://raw.githubusercontent.com/kristkat/my-template-portainer/master/2017-08-22.png" width="77%"/>
