ARG LLVM_VER
FROM lancern/llvm-src:${LLVM_VER}-stretch AS llvm-src
FROM lancern/cxxdev:stretch
COPY --from=llvm-src /llvm /llvm
WORKDIR /llvm-build

RUN cmake -G Ninja -DCMAKE_BUILD_TYPE=Release /llvm && \
    cmake --build . && \
    cmake --build . --target install 

WORKDIR /
RUN rm -rf /llvm /llvm-build

