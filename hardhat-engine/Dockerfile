# Gunakan nodejs versi 20.10
FROM node:20.10

# Tentukan direktori kerja
WORKDIR /app

# Salin semua file dan folder ke dalam direktori kerja
COPY . .

# Install Truffle lts secara global
RUN npm install hardhat

# Compile smart contracts menggunakan hardhat
RUN npx hardhat compile

RUN npx hardhat test

RUN npx hardhat run scripts/deploy.js





# Expose port 9545 untuk Truffle develop
EXPOSE 9545
EXPOSE 24012


