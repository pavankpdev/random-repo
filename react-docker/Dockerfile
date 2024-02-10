FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package.json ./

# Install dependencies with pnpm
RUN npm install -g pnpm && pnpm install

# Copy remaining application files
COPY . .

EXPOSE 5173

# Define command to run the application
CMD ["pnpm", "dev"]
