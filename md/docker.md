This Dockerfile is for running a Streamlit app inside a Docker container.

It is very important to run like this so that it can communicate with the outside world.

CMD ["streamlit", "run", "main.py", "--server.port=8080", "--server.address=0.0.0.
0"]  

This start Streamlit app.
0.0.0.0 is important so the app can be accessed outside container.
Port 8080 is the port Streamlit listen inside container.

How to run:

!docker build -t <your repo name><name of the image><tag> .
!docker run -p 8080:8080 <your repo name><name of the image><tag>

and to push it to the hub

! docker push <your repo name><name of the image><tag>

We push it to the hub because a picture of a pod was taken from the hub
