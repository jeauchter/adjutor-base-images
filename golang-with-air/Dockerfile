# Use the official Golang image as the base image
FROM golang:1.23-alpine
LABEL org.opencontainers.image.source=https://github.com/jeauchter/adjutor-base-images

# Install necessary packages
RUN apk add --no-cache git

# Install Air for hot-reloading
RUN go install github.com/air-verse/air@latest

# Set the Current Working Directory inside the container
WORKDIR /app


