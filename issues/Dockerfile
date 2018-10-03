FROM elixir:1.7.3

WORKDIR '/build'

COPY mix.exs .
RUN mix deps.get

COPY lib lib
COPY test test
COPY config config

CMD ["mix", "test"]