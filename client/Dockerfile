FROM alpine:3.5

# Update
RUN apk add --update python3

# Bundle app source
COPY client.py /src/client.py


ENTRYPOINT ["python3", "/src/client.py"]
