# Gunakan nodejs versi 16
FROM node:16

# Tentukan direktori kerja
WORKDIR /app

# Salin semua file dan folder ke dalam direktori kerja
COPY . .

# Install Truffle lts secara global
RUN npm install -g truffle@5.5
RUN npm install @truffle/hdwallet-provider

# Compile smart contracts menggunakan Truffle
RUN truffle compile

# Jalankan perintah Truffle develop
CMD ["truffle", "develop"]



# Expose port 9545 untuk Truffle develop
EXPOSE 9545

