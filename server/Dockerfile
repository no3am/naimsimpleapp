FROM alpine:3.5

# Update
RUN apk add --update python py-pip
RUN pip install --upgrade pip

# Install app dependencies
RUN pip install -U web.py
RUN pip install -U pathlib

# Bundle app source
COPY server.py /src/server.py
COPY user_data.xml /src/user_data.xml


EXPOSE  8080
CMD ["python", "/src/server.py"]
