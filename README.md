🛠️ 1. Dasar Project Laravel
Fungsi	Perintah
Membuat project baru	laravel new nama-project
(butuh Laravel installer)
Atau (via composer)	composer create-project laravel/laravel nama-project
Menjalankan server lokal	php artisan serve
Cek versi Laravel	php artisan --version

🧪 2. Artisan Commands Penting
Fungsi	Perintah
Melihat semua perintah Artisan	php artisan list
Clear semua cache (wajib saat error aneh)	php artisan optimize:clear
Clear route cache	php artisan route:clear
Clear config cache	php artisan config:clear
Buat secret key .env	php artisan key:generate

🔍 3. Route
Fungsi	Perintah
Lihat semua route	php artisan route:list
Lihat route API saja	php artisan route:list --path=api
Route web saja	php artisan route:list --path=web

🗃️ 4. Migration & Database
Fungsi	Perintah
Membuat file migration	php artisan make:migration create_nama_table
Jalankan semua migration	php artisan migrate
Rollback 1 step	php artisan migrate:rollback
Rollback semua	php artisan migrate:reset
Refresh semua (drop + migrate ulang)	php artisan migrate:refresh
Seeding data	php artisan db:seed
Buat seeder baru	php artisan make:seeder NamaSeeder
Jalankan seeder tertentu	php artisan db:seed --class=NamaSeeder

👷‍♂️ 5. Model, Controller, Resource
Fungsi	Perintah
Buat model	php artisan make:model NamaModel
Buat model + migration	php artisan make:model NamaModel -m
Buat controller	php artisan make:controller NamaController
Buat controller resource	php artisan make:controller NamaController --resource
Buat API resource (transformer)	php artisan make:resource NamaResource

👤 6. Auth (Jetstream/Breeze/etc.)
Fungsi	Perintah
Install Breeze	composer require laravel/breeze --dev
php artisan breeze:install
Install Jetstream	composer require laravel/jetstream
php artisan jetstream:install livewire
Jalankan npm & vite	npm install && npm run dev

📦 7. Cache & Config
Fungsi	Perintah
Cache config	php artisan config:cache
Cache route	php artisan route:cache
Cache view	php artisan view:cache
Clear semua cache	php artisan optimize:clear

⚙️ 8. Queue & Schedule (opsional)
Fungsi	Perintah
Jalankan queue worker	php artisan queue:work
Cek queue failed	php artisan queue:failed
Jalankan task scheduler (cron)	php artisan schedule:run

🧼 9. File Storage / Symlink
Fungsi	Perintah
Buat link ke storage (wajib untuk upload)	php artisan storage:link

📁 10. File Log
bash
Salin
Edit
tail -f storage/logs/laravel.log
Melihat log Laravel real-time (saat debug error).

Kalau kamu mau saya buatkan alias terminal Laravel (biar cepat ngetik), tinggal bilang ya!









