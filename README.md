docker run -d -t	\ 
	--name mongodb	\ 
	-p 27017:27017	\ 
	-p 28017:28017	\ 
	-v /docker-shares:/docker-shares	\ 
	-v /docker-data/mongodb:/var/lib/mongodb	\ 
	--restart=on-failure:100	\ 
	matteoredaelli/docker-mongodb-rpi
