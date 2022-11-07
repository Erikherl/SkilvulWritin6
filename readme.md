# Writing Front-end Week 2

## 1. React JS Lanjutan

<br>

### **Prop Types**

<br>

Prop types adalah sebuah data props yang dikirim kemudian dicek apakah sudah sesuai dengan tipe yang diberikan menggunakan sebuah lib, jika tidak sesuai akan memunculkan sebuah error

![Gambar 1](./1%20Lanjutan/PropTypes.png)

*Gambar 1. PropTypes Error*

Untuk cara setup Prop Types cukup mudah, jalankan `npm install prop-types` pada terminal project ReactJS

![Gambar 2](./1%20Lanjutan/Installing.png)

*Gambar 2. Installing Prop Types*

Dengan begitu project sudah terinstall Prop-Types pada ReactJS, Untuk penggunaannya cukup mudah

![Gambar 3](./1%20Lanjutan/PropTypes2.png)

*Gambar 3. Passing Data*

Pada aplikasi utama, kita akan mempassing data dari App.js ke Screen.js, dengan method prop types. Disini kita menggunakan komponen Screen.js sebagai contoh, dan dari App.js kita mengirimkan nama dan umur ke dalam se buah komponen

![Gambar 4](./1%20Lanjutan/PropTypes3.png)

*Gambar 4. Prop Types*

Pada Screen.js kita akan menaruh sebuah prop-types yang memiliki tujuan untuk mevalidasi props tersebut apakah name itu sebuah string, sedangkan age adalah sebuah number. Apabila dia salah, maka aka memunculkan sebuah error seperti pada Gambar 1


<br>

### **React Hooks**

<br>

Hooks ini berfungsi untuk memudahkan penggunaan functional components agar bisa menggunakan salah satu method state dan juga lifecycle yang sudah dijelaskan sebelumnya dalam penggunaan componentDidMount

![Gambar 5](./1%20Lanjutan/Hooks.jpg)

*Gambar 5 Logo React Hooks*

