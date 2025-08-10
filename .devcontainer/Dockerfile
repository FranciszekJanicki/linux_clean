FROM archlinux:base-devel

RUN pacman -Syu --noconfirm \
    build-essentials cmake make git \
    && pacman -Scc --noconfirm

RUN pacman -Syu --noconfirm nano \
    && pacman -Scc --noconfirm

USER devuser
WORKDIR /home/devuser

SHELL ["/bin/bash", "-c"]

ENTRYPOINT ["/bin/bash"]
