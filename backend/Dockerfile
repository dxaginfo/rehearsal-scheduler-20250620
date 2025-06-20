FROM node:18-alpine

WORKDIR /app

# Copy package files
COPY package*.json ./
RUN npm ci

# Generate Prisma client
COPY prisma ./prisma/
RUN npx prisma generate

# Copy application code
COPY . .

# Set environment variables
ENV NODE_ENV=production

# Expose the port
EXPOSE 4000

# Run database migrations and start the server
CMD npx prisma migrate deploy && npm start