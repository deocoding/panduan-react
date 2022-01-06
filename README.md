<h1 align="center">Tutorial REACT</h1>

React merupakan library JavaScript untuk pengembangan UI.

<h2 align="center">Studi Kasus -> Web Tesla Clone</h2>

### Instalasi Node JS di Windows 10

Node JS merupakan JavaScript runtime yang dibangun untuk `Chrome V8 JavaScript engine`.

- Download installer `Node.js` pada alamat `nodejs.org`, versi yang digunakan adalah versi `16.13.1 LTS`. Kemudian klik untuk menginstallnya.
- Install installer yang telah didownload.

### Buat aplikasi React baru

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

### Mulai pengembangan aplikasi React

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
