FROM ubuntu:16.04
RUN mkdir /etc/site
WORKDIR /etc/site
COPY ./pages .
RUN apt update	&& \
	apt install -yf \
	stunnel && \
	mv /etc/site /etc/stunnel && \
        mv /etc/stunnel/site/stunnel.conf /etc/stunnel/stunnel.conf
# COPY ./pages .
# EXPOSE 80
CMD ["ls"]
