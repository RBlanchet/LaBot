FROM python:3.7-alpine
RUN apk update && \
    apk add bash && \
    apk add openjdk8 && \
    apk add unzip
RUN wget https://github.com/jindrapetrik/jpexs-decompiler/releases/download/nightly1939/ffdec_14.4.0_nightly1939.zip
RUN unzip ffdec_14.4.0_nightly1939.zip -d jpexs
COPY . /app
WORKDIR /app
# RUN pip install -r requirements.txt
