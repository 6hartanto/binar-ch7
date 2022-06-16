# fsw-challenge-ch7
Binar FSW Challenge Chapter 7

Before using this program:
1. Install all necessary module => `npm install`
2. Set the `config.json` file based on your environtment
3. Migrate the database => `sequelize db:migrate`
4. Seed the datasbe => `sequelize db:seed:all`

Petunjuk Penggunaan:
1. Secara default program dijalankan pada `http://localhost:3000`
2. Pengaturan akun dapat dilakukan pada :
    -> Register Akun => `http://localhost:3000/api/v1/auth/register`
        dengan menyiapkan form dengan method POST berisi :
            * username (string)
            * password (string)
    -> Login Akun => `http://localhost:3000/api/v1/auth/login`
        dengan menyiapkan form dengan method POST berisi: 
            *username (string)
            *password (string)
        jika `username` dan `password` benar, maka akan ditampilkan data `id`,`username`, dan `accessToken`
    -> Login Token => `http://localhost:3000/api/v1/auth/login-token`
        digunakan untuk melakukan cek apakah token tersebut berfungsi