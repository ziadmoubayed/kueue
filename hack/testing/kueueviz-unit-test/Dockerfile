FROM node:25-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install ALL dependencies (including dev dependencies needed for tests)
RUN npm install

# Copy source files
COPY . .

CMD ["npm", "test"]
