# Use the official Golang image as the base image
FROM golang:1.23-alpine

# Install necessary packages
RUN apk add --no-cache git

# Install Air for hot-reloading
RUN go install github.com/air-verse/air@latest

# Set the Current Working Directory inside the container
WORKDIR /app



# Download all dependencies. Dependencies will be cached if the go.mod and go.sum files are not changed
RUN go mod download

