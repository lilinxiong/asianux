FROM ccr.ccs.tencentyun.com/lilinxiong/asianux:cu100_base_7
LABEL maintainer "lilinxiong <lilinxiong1997@gmail.com>"

RUN rpm --rebuilddb && yum install -y \
        cuda-libraries-$CUDA_PKG_VERSION \
        cuda-nvtx-$CUDA_PKG_VERSION && \
    rm -rf /var/cache/yum/*

