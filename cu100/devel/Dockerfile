FROM ccr.ccs.tencentyun.com/lilinxiong/asianux:cu100_runtime_7
LABEL maintainer "lilinxiong <lilinxiong1997@gmail.com>"

 RUN rpm --rebuilddb && yum install -y \
	  cuda-libraries-dev-$CUDA_PKG_VERSION \
	  cuda-nvml-dev-$CUDA_PKG_VERSION \
	  cuda-minimal-build-$CUDA_PKG_VERSION \
	  cuda-command-line-tools-$CUDA_PKG_VERSION && \
	  rm -rf /var/cache/yum/*

ENV LIBRARY_PATH /usr/local/cuda/lib64/stubs

