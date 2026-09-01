# Node.js + React in Ubuntu (Termux)

Install Ubuntu 24.04 with `proot-distro`, then install Node.js using NVM.

## 1. Install Ubuntu

```bash
pkg install proot-distro
proot-distro install ubuntu:24.04
proot-distro login ubuntu
```

## 2. Install NVM + Node.js

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
source ~/.bashrc
nvm --version
nvm install --lts
```

## 3. Check Node.js

```bash
node -v
npm -v
```

## 4. Test npm

```bash
mkdir test-node
cd test-node
npm init -y
```

## 5. Create React + Vite

```bash
npm create vite@latest my-react-app
```
```bash
cd my-react-app
npm install
npm run dev
```

