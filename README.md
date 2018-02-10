# Docker image of Supervisor
Docker image based on Alpine Linux 3.7 with Supervisor

For try run you application need create configuration file: **example.ini**  

Run the image:
`docker run -d --name supervisor -v $(pwd):/etc/supervisor.d vendelev/supervisor`

Run the image (with port for access for internal "inet_http_server"):
`docker run -d --name supervisor -v $(pwd):/etc/supervisor.d -p 9999:9999 vendelev/supervisor`

By default, the image exposes the 9999 port.