FROM pblop/devkitpro-toolchain-base

MAINTAINER Dave Murphy <davem@devkitpro.org>

RUN ln -s /proc/mounts /etc/mtab


RUN dkp-pacman -Syyu --noconfirm switch-dev && \
    dkp-pacman -S --needed --noconfirm switch-portlibs && \
    dkp-pacman -S --needed --noconfirm devkitARM && \
    yes | dkp-pacman -Scc

ENV DEVKITARM=/opt/devkitpro/devkitARM

