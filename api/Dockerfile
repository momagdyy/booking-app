FROM node:16-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and yarn.lock to the working directory
COPY package.json yarn.lock ./

# Install dependencies using yarn
RUN yarn install

# Copy the rest of the application code to the container
COPY . ./

# Expose the port your Express app runs on
EXPOSE 5000

# Define the command to run your app
CMD ["yarn", "start"]
