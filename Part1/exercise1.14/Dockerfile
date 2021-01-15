FROM ruby:2.6.0
WORKDIR /myapp
COPY rails-example-project .
RUN apt-get update 
RUN apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs
RUN gem install bundler
RUN bundle install
RUN rails db:migrate
CMD ["rails","s"]
