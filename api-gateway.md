# API GATEWAY 
-> Koneksi ke sistem backend

## Cara yang simple dengan url saja
    api.perusahaan.com/inventory
    api.perusahaan.com/finance
    ..

## Bagaimana dari domain bisa nembak ke aplikasi aslinya
    jadi routingnya memakai PROXY SERVER (Nginx ApacheHttp Hproxy)
    Jadi ini sudah bisa disebut API Gateway

## Authentication
    Centralize Authentication -> Ontetikasi berada di API Gateway jangan di backend service supaya tidak ribet
    Banyak jenis Authentication seperti  Oauth mobile, Session, Basic Ontentation, dll jadi cukup 1 saja di API Gateway

## Authorization
    Dimana ada Authentication disana ada Authorization.
    di API Gateway dibikin Roles System. Jadi tidak perlu menaruh Authorization di setiap backend

##Rate Limited
    Agar Request Masuk disesuikan dengan Servicenya
    per total request atau per user

## Orchestrator
    Jadi Backend service tidak saling terkengantungan seperti Employee System dengan Payroll System 
    API Gateway berfungsi merequest ke kedua service tersebut dan dikembalikan dengan cara mengabungkan keduanya

## Standard API => Transform data ke satu bahasa di API Gate Way
    JSON
    RCP
    XML
    SOAP


## Backend for Frondend =>
    API untuk masing masing sistem ? NO 
    Third Party System, Mobile, Web 

    Solution-> API Gateway saja yang berbeda 
    Graph QL <- implementasi yang sudah ada implementasinya dari backend for Frondend

Sumber : https://www.youtube.com/watch?v=aZWbBcgS16s&fbclid=IwAR3CC0iiwOCWJeMV7zCfyOhqwzKp6whuRcieygkOTGHdEASCJNpep3a8wGM