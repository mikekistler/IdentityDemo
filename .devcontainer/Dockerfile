ARG VARIANT=1-9.0
FROM mcr.microsoft.com/devcontainers/dotnet:${VARIANT}

# Install .NET 10.0 nig

# TODO: Find a way to get the latest .NET 10.0 preview 2 version
# https://github.com/dotnet/sdk/blob/main/documentation/package-table.md#table
ARG VERSION="10.0.100-preview.2.25126.21"

RUN wget https://dot.net/v1/dotnet-install.sh -O dotnet-install.sh \
    && chmod +x dotnet-install.sh \
    && sudo ./dotnet-install.sh --version ${VERSION} --install-dir /usr/share/dotnet \
    && rm dotnet-install.sh
