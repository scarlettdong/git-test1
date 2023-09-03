# Use an official Node.js runtime as the base image
FROM node:16

# Set the working directory inside the container
WORKDIR /app

# Install express directly since we are not using package.json
RUN npm install express

# Copy the index.js and other necessary sources
COPY . .

# Set the environment variable for the port
ENV PORT=8080

# Inform Docker that the container listens on the specified port at runtime
EXPOSE 8080

# Define the command to run the app directly with node
CMD ["node", "index.js"]
