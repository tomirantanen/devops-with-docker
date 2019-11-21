FROM ruby:2.6.0-alpine

RUN apk add --update build-base sqlite-dev nodejs tzdata

COPY . .
RUN bundle install
RUN rails db:migrate

EXPOSE 3000
CMD [ "rails", "s" ]
