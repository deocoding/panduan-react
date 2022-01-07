<h1 align="center">Tutorial REACT - "Web Tesla Clone"</h1>

React merupakan library JavaScript untuk pengembangan UI.

## Instalasi Node JS di Windows 10

Node JS merupakan JavaScript runtime yang dibangun untuk `Chrome V8 JavaScript engine`.

- Download installer `Node.js` pada alamat `nodejs.org`, versi yang digunakan adalah versi `16.13.1 LTS`. Kemudian klik untuk menginstallnya.
- Install installer yang telah didownload.

## Buat aplikasi React baru

- Pastikan bahwa `Yarn` telah terinstall. Jika belum jalankan perintah :

  ```bash
  npm install -g yarn
  ```

- Verifikasi bahwa `Yarn` telah terinstall.

  ```bash
  yarn -v
  ```

- Install aplikasi `React` dengan nama proyek `tesla-clone` dan menggunakan template `redux`.

  ```bash
  npx create-react-app tesla-clone --template redux
  ```

- Arahkan ke folder `tesla-clone` dan uji coba server.

  ```bash
  cd tesla-clone
  yarn start
  ```

- Buka VS Code.

  ```bash
  code .
  ```

- Buka terminal pada VS Code dan jalankan server lokal menggunakan `yarn`.

  ```bash
  yarn start
  ```

## Mulai pengembangan aplikasi React

- Buka file `src/App.js` dan hapus komponen `<header ...>` untuk menghapus tampilan default.
- Buka file `src/index.css` dan hapus semua isinya.
- Buat folder `components` pada folder `src`. Tambahkan file komponen layout sesuai dengan desain yang anda inginkan, misal file `Header.js`.
- Pada file `Header.js`, ketik perintah `rfce` dan tekan enter maka format komponen React akan otomatis dibuat.

  ```javascript
  import React from "react";

  function Header() {
    return <div></div>;
  }

  export default Header;
  ```

- Import komponen pada file `src/App.js` untuk dapat dilakukan pemanggilan.

  ```javascript
  import React from "react";
  import logo from "./logo.svg";
  import { Counter } from "./features/counter/Counter";
  import "./App.css";
  // import komponen Header.js
  import Header from "./components/Header";

  function App() {
    return (
      <div className="App">
        {/* pemangilan komponen Header.js */}
        <Header />
      </div>
    );
  }

  export default App;
  ```

- Tambahkan kode-kode css berikut pada file `src/index.css`.

  ```css
  * {
    box-sizing: border-box;
    font-family: "Rubik", sans-serif;
    color: #393c41;
    margin: 0;
    padding: 0;
  }

  body {
    width: 100%;
  }
  ```

- Buat komponen baru dengan nama `Home` seperti cara sebelumnya.
- Tambahkan library `styled-components` pada terminal dan lakukan import pada file `Home`.

  ```bash
  yarn add styled-components
  ```

  ```javascript
  import styled from "styled-components";
  ```

- Jika ada error saat mengcompile, jalankan perintah berikut :

  ```bash
  npm install --legacy-peer-deps
  ```

- Menambahkan Material UI

  ```bash
  yarn add @mui/material @emotion/react @emotion/styled
  yarn add @mui/icons-material
  ```

- Menambahkan Animasi dengan mengetik keyword `react reveal` pada google search dan install

  ```bash
  yarn add react-reveal
  ```

  > Muncul error pada console, perlu diperbaiki

<br/>

<h1 align="center">Tutorial REACT - "Web Disney+ Clone"</h1>

## Pembersihan Awal

- Hapus component `<header>` & baris `import logo from "./logo.svg";` pada file `App.js`.
- Hapus semua isi pada file `App.css`.
- Hapus file `App.test.js` & `logo.svg`.

## Mulai Coding

- Buat folder `components` didalam folder `src`. Letakkan semua komponen difolder ini.
