FROM pretix/standalone:stable as base

COPY ./plugins/pretix-manualseats /plugins/pretix_manualseats

USER root

RUN pip install -e /plugins/pretix_manualseats

FROM base as runner

USER pretixuser