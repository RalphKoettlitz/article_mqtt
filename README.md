# This repo is a supplement to an article

It's practical to run mosquitto with docker. The option -v maps the folder broker to the image folder mosquitto, so that the config can be read. 

```
docker run -it -p 1883:1883 -v $(pwd)/broker:/mosquitto/ eclipse-mosquitto

= broker +
		  + config +
		           | mosquitto.conf
				   
				  
```

mosquitto.conf

```
allow_anonymous true
```
