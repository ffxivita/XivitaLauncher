# Warning! You will be unable to use `dotnet run` when developing inside of a container
# Due to not being able to access the host machine's windowing system.


FROM mcr.microsoft.com/dotnet/sdk:7.0@sha256:bd1ccc2332fc03c6df1659ed125f67f02666f9f188947a80cec4e7afd3c7f98d

# Optout of telemtry.
ENV DOTNET_CLI_TELEMETRY_OPTOUT=1
ENV DOTNET_SKIP_FIRST_TIME_EXPERIENCE=1

# Create a non-root dev user.
RUN adduser --disabled-password --gecos "" dev
