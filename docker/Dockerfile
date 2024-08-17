FROM ghcr.io/moritzlerch/pretix-manualseats as pretix_manualseats

FROM pretix/standalone:stable

COPY --from=pretix_manualseats /pretix-manualseats /pretix-manualseats

RUN pip install -e /plugins/pretix_manualseats