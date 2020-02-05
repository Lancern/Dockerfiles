FROM lancern/llvm-src:debian-stretch-slim AS llvm-src
FROM lancern/cxxdev:debian-stretch-slim
COPY --from=llvm-src /llvm /
WORKDIR /llvm-build

RUN cmake -G Ninja -DCMAKE_BUILD_TYPE=Release /llvm && \
    cmake --build . && \
    cmake --install .
