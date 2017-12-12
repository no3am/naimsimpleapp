FROM alpine:3.1

# Update
RUN apk add --update python py-pip

# Install app dependencies
RUN pip install -U urllib.request
RUN pip install -U json
RUN pip install -U sys

# Bundle app source
COPY client.py /src/client.py


CMD ["python", "/src/client.py"]
