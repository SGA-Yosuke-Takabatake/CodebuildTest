FROM public.ecr.aws/docker/library/node:lts

RUN mkdir /home/test

# install jq
# RUN wget http://stedolan.github.io/jq/download/linux64/jq -O jq
# RUN chmod 755 jq
# RUN mv jq /usr/local/bin/
RUN apt update && apt install -y \
    jq \
    && apt clean \
    && rm -rf /var/lib/apt/lists/*

# run hubot
CMD ["jq", "--help"]
