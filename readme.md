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

Penggunaan useState pada React Hooks dapat dilihat pada bagian bawah ini

```js
const [first, setFirst] = useState(5)  
```

Dimana `first` adalah sebuah value utamanya, dan `setFirst` merupakan variabel editor untuk value utamanya. Kedua variabel tersebut dicakup dalam sebuah array

Pada sebelah kanan terdapat `5` dimana ini adalah inisialisasi value pertama kalinya, dan dapat diinput dengan string, boolean, object, number dan lain lainnya

![Gambar 6](./1%20Lanjutan/useState.png)

*Gambar 6 useState*

Kemudian, kita juga dapat mengupdate state tersebut

![Gambar 7](./1%20Lanjutan/setState.png)

*Gambar 7 update State*

Selanjutnya apabila kita ingin sebuah state tersebut berasal dari API, maka dapat menggunakan useEffect yang dimana sudah dijelaskan pada minggu sebelumnya

<br>

### **React Router**

<br>

React memungkinkan kita untuk mengakses sebuah website dalam satu halaman. Dengan menggunakan React Router akan memudahkan hal tersebut karena disini kita hanya perlu mengarahkan rute tersebut dalam program kita

![Gambar 8](./1%20Lanjutan/Contoh%20Router.png)

*Gambar 8 Contoh React Router*

Gambar hanya contoh yang dimana saat kita mengakses sebuah halaman lain atau bagian tertentu kita akan berpindah url, yang dimana itu bisa saja dalam satu halaman tanpa berpindah pindah

Untuk cara instalasi React Router dapat dilihat pada gambar berikut

![Gambar 9](./1%20Lanjutan/Router.png)

*Gambar 9 Installing Router*

Penggunaan Browser Router untuk mengaplikasikan React Router pada file yang dituju atau yang dibungkus

![Gambar 10](./1%20Lanjutan/BrowserRouter.png)

*Gambar 10 Browser Router*

Selanjutnya adalah penggunaan routes dan route pada aplikasi utama kita, disini kita dapat mengimport beberapa file lainnya sebagai contoh untuk navigasinya

![Gambar 11](./1%20Lanjutan/Router2.png)

*Gambar 11 Routes in App*

Routes disini untuk membungkus bagian mana yang menjadi untuk pengaplikasikan sebuah React Route

Langkah selanjutnya kita dapat memodifikasi `routes` menjadi bisa diaplikasikan pada tampilan website biasanya, seperti pada gambar berikut

![Gambar 12](./1%20Lanjutan/Router4.png)

*Gambar 12 Routes pada website*

Selanjutnya akan menggunakan dari penggunaan params, dimana apabila kita melihat sebuah website e-commerce terdapat berbagai barang pada suatu website. Apabila diklik akan memunculkan seperti pada gambar 13

![Gambar 13](./1%20Lanjutan/Tokopedia.png)

*Gambar 13 Tokopedia Website*

Pada gambar 13, kita dari homepage ke barang tersebut, ada beberapa data yang dikirimkan sehingga barang tersebut bisa muncul seperti itu

Pada React Router ini menggunakan yang namanya params

![Gambar 14](./1%20Lanjutan/Params.png)

*Gambar 15. Membuat Data*

Pertama kita membuat data yang muncul pada home, kemudian kita membuat sebuah function yang dapat mempassing data tersebut ke sebuah halaman `/detail` dengan menggunakan `useNavigate`

![Gambar 16](./1%20Lanjutan/Params2.png)

*Gambar 16. Membuat Function dengan useNavigate*

Dan hasilnya adalah kita akan mendapatkan ID pada halaman detail

![Gambar 17](./1%20Lanjutan/Params3.png)

*Gambar 17. Halaman Detail dengan ID*

Dan untuk menangkap ID tersebut, kita dapat jadikan seperti pada gambar berikut, dengan menggunakan `useParams`

![Gambar 18](./1%20Lanjutan/Params4.png)

*Gambar 18. Penggunaan UseParams*

![Gambar 19](./1%20Lanjutan/Params5.png)

*Gambar 19. Hasil useParams*

Inilah yang dinamakan dengan dynamic routes

Selanjutnya mengenai nested routes yang digunakan untuk apabila kita memiliki sebuah dua halaman dalam satu cabang. Contohnya

```js
about\home
about\school
```

Kedua hal tersebut apabila dituliskan dalam route satu persatu akan menjadi sedikit panjang, nah caranya adalah menggunakan nested routes

![Gambar 20](./1%20Lanjutan/nested.png)

*Gambar 20. Penggunaan Nested*

Untuk nested pada gambar 20, kita perlu memasukkan sebuah route pada isi dari route parentsnya, disini kita menggunakan route `/book` sebagai utamanya

Kemudian, kita juga perlu menambahkan `Outlet` pada route yang berkaitan dengan `/book` agar dia dapat memuat child parentsnya

![Gambar 21](./1%20Lanjutan/nested2.png)

*Gambar 21. Outlet pada BookList*

Dan hasilnya akan seperti berikut

![Gambar 22](./1%20Lanjutan/nested3.png)

*Gambar 22. Nested Route*

Terakhir, mengenai nested routes, apabila kita menambahkan atribute `index` pada routes yang nested, dia akan otomatis membuat halaman tersebut menjadi default ketika terbuka

![Gambar 23](./1%20Lanjutan/nested4.png)

*Gambar 23. Index Nested Routes*

Jadi setiap kali dibuka `/book` dia akan otomatis memuat halaman `AboutAuthor` karena dia dijadikan sebagai index

<br>

### **React Redux**

<br>

Apa itu Redux? redux itu sering digunakan ketika kita ingin mengatur sebuah state pada ReactJS, Redux itu sendiri adalah sebuah library yang mengatur khusus untuk hal itu pada sebuah aplikasi berbasis ReactJS ataupun juga Angular, Vue, dan lainnya

Pada Redux, kita akan mengenal 4 konsep utama, Reducers, actions, action creation, dan store

![Gambar 24](./1%20Lanjutan/Redux.png)

*Gambar 24. Gambaran kasar mengenai Redux*

Untuk memulainya kita dapat menginstall terlebih dahulu React Redux, ada dua cara, cara yang pertama menginstall dengan template kosongan, dan yang satu lagi mengaplikasikan pada project React yang sudah ada

![Gambar 25](./1%20Lanjutan/Installing%20Redux.png)

*Gambar 25. Installing Redux*

Setelah melakukan instalasi, kita dapat langsung mengkonfigurasi index.js menjadi seperti pada gambar 26

![Gambar 26](./1%20Lanjutan/Redux2.png)

*Gambar 26. Setup Redux*

Memiliki tujuan untuk mensetup store atau storage yang akan digunakan pada React Redux ini

Selanjutnya kita dapat membuat sebuah reducer yang fungsinya seperti sebuah rak barang

![Gambar 27](./1%20Lanjutan/Reducer.png)

*Gambar 27. Reducer Function*

Selanjutnya setelah membuat reducer pada sebuah file lain, kita kembali ke index.js untuk memasukkan reducer tersebut ke store

![Gambar 28](./1%20Lanjutan/Reducer2.png)

*Gambar 28. Reducer to Store*

Setelah reducer, apabila kita lihat pada gambar 27, terdapat "action" dimana ini adalah sebuah aksi yang akan digunakan untuk penggunaan conditional switch tersebut. 