# Warning! You will be unable to use `dotnet run` when developing inside of a container
# Due to not being able to access the host machine's windowing system.


FROM mcr.microsoft.com/dotnet/sdk:7.0@sha256:e049e6a153619337ceb4edd040fb60a220d420414d41d6eb39708d6ce390bc7c

# Optout of telemtry.
ENV DOTNET_CLI_TELEMETRY_OPTOUT=1
ENV DOTNET_SKIP_FIRST_TIME_EXPERIENCE=1

# Create a non-root dev user.
RUN adduser --disabled-password --gecos "" dev
