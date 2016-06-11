# Dockerfile of gollum - A git-based Wiki
#
# https://github.com/gollum/gollum
#
# The recipe of this Dockerfile is from  
# https://github.com/gollum/gollum/wiki/Gollum-via-Docker
#
FROM ruby
RUN apt-get -y update && apt-get -y install libicu-dev
RUN gem install gollum
RUN gem install redcarpet org-ruby 
VOLUME /wiki
WORKDIR /wiki
# Set your gollum options here
CMD ["gollum", "--port", "80"]
EXPOSE 80

