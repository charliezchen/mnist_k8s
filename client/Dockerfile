# Start with a Linux micro-container to keep the image tiny
FROM python:3.8

RUN pip3 --no-cache-dir install requests

# Add the code as the last Docker layer because it changes the most
COPY test.png .
COPY client.py .


# Run the service
CMD [ "python3", "client.py"] 
