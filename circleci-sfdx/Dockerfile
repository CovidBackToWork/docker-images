FROM cimg/base:stable
# https://circleci.com/blog/announcing-our-next-generation-convenience-images-smaller-faster-more-deterministic/

LABEL maintainer="workops@salesforce.com" version="0.0.1-beta"

RUN wget -O /tmp/sfdx.tar.xz https://developer.salesforce.com/media/salesforce-cli/sfdx-linux-amd64.tar.xz \ 
    && mkdir ~/sfdx && tar xJf /tmp/sfdx.tar.xz -C ~/sfdx --strip-components 1 \
    && ~/sfdx/install && sfdx --version