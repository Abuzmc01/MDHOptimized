# MDHOptimized

Plugin optimasi untuk server Paper: pre-generate chunk pintar (chunk yang sudah ada dilewati), clear lag terjadwal,
limit redstone & entity per chunk, dan notifikasi lokasi masalah ke console/operator.

## Build
Butuh Java 17+ dan Maven.

    mvn package

Hasilnya: `target/MDHOptimized.jar`

Dikompilasi terhadap `paper-api 1.20.1` supaya jalan di Paper 1.20.1 sampai versi terbaru.

## Struktur
- `MDHOptimized.java` : main class, command /mdho, pembacaan config
- `Monitor.java`      : limit redstone/piston/hopper, limit spawn entity, scan entity & tile entity, TPS
- `Cleaner.java`      : clear lag terjadwal dan manual
- `Pregen.java`       : pre-generate chunk spiral, skip chunk yang sudah ada, simpan/lanjutkan progres
- `Alerts.java`       : notifikasi + daftar peringatan + teleport

Dokumentasi lengkap: `DOCUMENTATION.md`

