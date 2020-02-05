FROM lancern/cxxdev:stretch
ARG LLVM_VER
WORKDIR /

ADD http://releases.llvm.org/${LLVM_VER}/llvm-${LLVM_VER}.src.tar.xz ./
RUN tar -xf llvm-${LLVM_VER}.src.tar.xz && \
    mv llvm-${LLVM_VER}.src llvm && \
    rm llvm-${LLVM_VER}.src.tar.xz
