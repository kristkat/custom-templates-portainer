# Creating your own templates in portainer

## Resources
* [Deploy Portainer](https://portainer.readthedocs.io/en/latest/deployment.html)
* [Documentation](https://portainer.readthedocs.io)

## Ways to create your own templates
1. Create JSON file where you can describe your templates. 
  How to write this file you can find here: https://portainer.readthedocs.io/en/latest/templates.html
2. Upload this file in GitHub for example so that you can access it with URL
3. my example of templares.json you can find here: https://raw.githubusercontent.com/kristkat/custom-templates-portainer/master/templates.json

### Using the settings section in Portainer UI 
* **Starting Portainer:**
1. docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer
2. access Portainer by pointing your web browser at http://DOCKER_HOST:9000
3. in portainer UI you go in Settings and write URL with your templates
<p align="center">
  <img title="portainer" src='https://raw.githubusercontent.com/kristkat/custom-templates-portainer/master/settings.png' />
</p>

### Using --templates flag 
* **Starting Portainer:**
1. docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer --templates http://my-host.my-domain/templates.json
On the place of  http://my-host.my-domain/templates.json you should write URL with your JSON file. 
This way of adding your templates in portainer works without going to settings in portainer UI.
Documentation about it you find here: https://portainer.readthedocs.io/en/latest/configuration.html#use-your-own-templates 

## Result
<p align="center">
  <img title="portainer" src='https://raw.githubusercontent.com/kristkat/custom-templates-portainer/master/result1.png' />
</p>
<p align="center">
  <img title="portainer" src='https://raw.githubusercontent.com/kristkat/custom-templates-portainer/master/result2.png' />
</p>

