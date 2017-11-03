# Vue JS Documentation

## Setup Project Vue
``` bash
# Install vue cli
npm install -g vue-cli

# Init Project
vue init webpack {{nama project}}
cd {{nama project}}
npm install

# run project
npm run dev

# build project
npm run build
```

## Struktur Project
```
{{nama project}}
-- node_modules
-- src
    -- assets
    -- components
        -- HelloWorld.vue
    -- router
        -- router.js
    -- App.vue
    -- main.js
-- index.html
-- package.json
```
Keterangan : 
- package.json = file yang berisi list dependency/library
- index.html = main endpoint, dari sini kita bisa mapping template dari banyak `Top Level Compenent`. 
- main.js = file untuk setting top level component yang akan dimapping ke index.html.
- App.vue = salah satu Top level component.
- router.js = file setting perutean setiap `Component`. Nantinya akan dipanggil di Top Level Component menggunakan `<router-view/>`.
- components = folder yang berisi component yang akan dirute tiap halaman. Contoh : HelloWorld.vue

Tambahan : 
- Dalam 1 project vue dapat memiliki lebih dari 1 buah top level component. Misal App.vue sebagai tempat content, lalu ada lagi Header.vue untuk header, Sidebar.vue untuk sidebar.
