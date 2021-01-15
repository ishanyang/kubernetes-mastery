FROM ruby:alpine
RUN gem sources --add https://gems.ruby-china.com/ --remove https://rubygems.org/ 
RUN gem sources -l
RUN apk add --update build-base curl
RUN gem install sinatra
RUN gem install thin
ADD hasher.rb /
CMD ["ruby", "hasher.rb"]
EXPOSE 80
