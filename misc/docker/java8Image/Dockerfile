FROM debian:experimental

# A few problems with compiling Java from source:
#  1. Oracle.  Licensing prevents us from redistributing the official JDK.
#  2. Compiling OpenJDK also requires the JDK to be installed, and it gets
#       really hairy.

ENV JAVA_VERSION 8u40

RUN apt-get update && apt-get install -y curl openjdk-8-jdk="$JAVA_VERSION"* unzip wget

# If you're reading this and have any feedback on how this image could be
#   improved, please open an issue or a pull request so we can discuss it!
