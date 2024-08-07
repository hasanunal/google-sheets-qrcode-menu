Hello,

In this article, we will explore how to integrate a menu created in Google Sheets (Google Excel) into our website, giving it a menu-like appearance. We can quickly set up a menu without the need for a database or additional coding.

### Working Mechanism

We create a table in Google Sheets and publish it publicly. After sharing, there is a parameter available that allows us to access this file remotely in JSON format. We use this parameter to process the data with JavaScript and display it on our page.

### 1) Creating Google Sheets

- [Google Drive](https://drive.google.com/) > New + > Google Sheets > Blank spreadsheet

| Ürün Adı | Ürün Açıklaması | Ürün Fiyatı | Ürün Resmi | Kategori |
|----------|-----------------|-------------|------------|----------|
| Milk Shake | (çikolata - beyaz çikolata) | 130₺ | resim linki | Soğuk İçecekler |
| Limonata | El Yapımı | 120₺ | resim linki | Soğuk İçecekler |
| Çay |  | 120₺ | resim linki | Sıcak İçecekler |

### 2) Creating a Share Link and Obtaining the ID

- Share > Anyone with the link *(Viewer)*
- Copy link

```

https://docs.google.com/spreadsheets/d/${id}/

```

We extract the part where `${id}` is and assign it to a variable:

```javascript

const id = 'id';

```

We assign it to the relevant variable.

Next, let's complete our script code.

### Bonus: Publishing
If you don't have hosting and want to publish quickly, you can use one of the following services:

- [GitHub](https://github.com/) > Create New Repo > Upload Code > Publish with GitHub Pages

- [Netlify](https://www.netlify.com/) > Create New Site > GitHub > Deploy

- [Vercel](https://vercel.com/) > Create New Site > GitHub > Deploy

Good luck. 🚀
*[hasanunal.org](https://hasanunal.org/)*
