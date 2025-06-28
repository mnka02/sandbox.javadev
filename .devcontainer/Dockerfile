FROM maven:3.9.6-eclipse-temurin-17

# install fundamental tools
RUN apt-get update && apt-get install -y \
    curl \
    git

# set up user for vscode remote dev
RUN useradd -ms /bin/bash devuser
# set up root directory for development
RUN mkdir -p /home/devuser/workspace && chown devuser:devuser /home/devuser/workspace
USER devuser
WORKDIR /home/devuser/workspace

# Expose port for remote debugging (optional)
EXPOSE 5005
