# Gunakan nodejs versi 14.17
FROM node:14.17

# Tentukan direktori kerja
WORKDIR /app

# Salin semua file dan folder ke dalam direktori kerja
COPY . .

# Install dependencies dengan npm
RUN npm install

# Jalankan perintah npm start
CMD ["npm", "start"]

# Expose port 3000
EXPOSE 3000
