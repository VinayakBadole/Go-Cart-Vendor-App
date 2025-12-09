# Go-Cart Vendor App

## 📦 Overview  
The Go Cart Vendor App is the vendor-side application for Go Cart App
It allows vendors who sell vegetables via carts or electric vehicles to manage their inventory, update their live location, and serve orders to customers in real time.

With this vendor app, vendors can: add or update vegetables, manage stock and prices, update their availability & live location — so users using the user-side app can discover and order from them.

---

## ✨ Key Features  

### 📍 Live Location / Status Updates  
- Vendors can enable location sharing to broadcast live location via map.  
- Users can see vendors’ real-time movement within a certain radius (e.g. 2 km).  

### 🥕 Inventory Management  
- Add new vegetable items (name, price, quantity, image, etc.)  
- Update existing items — price, quantity, description  
- Remove items when sold out or not available  

### 🛒 Order & Stock Sync  
- Sync inventory with central database (e.g. Firebase Firestore)  
- On customer order: inventory reduces, status updates to “pending” or “completed”  
- Real-time updates ensure accurate stock and order handling  

### 🔄 CRUD + Sync via Firebase / Backend  
- Real-time read & write of vendor data: inventory, location, availability  
- Smooth operations: add / update / delete with immediate effect  

### 🧑‍💼 Vendor Profile & Management  
- Maintain vendor details: name, contact / identifier, status  
- Optionally, rating & reviews (if implemented)  

---

## 📁 Project Structure  
```
/app
/assets
/components
/context or state management
/screens / views
/services     # Backend / Firebase / Location & map services
/utils
package.json
```

---

## 🚀 Getting Started  

### Prerequisites  
- Node.js  
- Expo CLI (if React Native / Expo) or relevant mobile framework  
- Backend setup (e.g. Firebase project & configuration)  

### Installation  
```bash
git clone https://github.com/VinayakBadole/Go-Cart-Vendor-App.git  
cd Go-Cart-Vendor-App  
npm install         # or yarn install  
npm start           # or yarn start  
```  

### Environment Variables / Config (if any)  
```
 
EXPO_PUBLIC_FIREBASE_API_KEY=
EXPO_PUBLIC_FIREBASE_AUTH_DOMAIN=
EXPO_PUBLIC_PROJECT_ID=
EXPO_PUBLIC_STORAGE_BUCKET=
EXPO_PUBLIC_MESSAGING_SENDER_ID=
EXPO_PUBLIC_APP_ID=
EXPO_PUBLIC_MEASUREMENT_ID=
EXPO_PUBLIC_MAPBOX_KEY=
EXPO_SECRET_MAPBOX_KEY=
MAPBOX_MAPS_DOWNLOAD_TOKEN=
EXPO_PUBLIC_SUPABASE_URL = 
EXPO_PUBLIC_SUPABASE_ANON_KEY =

```
---

## 🗂 Files to Exclude / .gitignore (Important)  
Your `.gitignore` should exclude:  
```
node_modules/
.expo/             # if using Expo  
.env               # environment / secret keys  
.vscode/ or IDE configs  
android/ / ios/    # builds or native project files  
build/ / dist/     # compiled output  
```

---

## 📄 Tech Stack 
- React Native (Expo) or relevant mobile framework  
- Backend: Firebase (Firestore + Auth) or equivalent  
- Real time data & location services (e.g. Firestore + Mapbox / native location API)  
- JavaScript / TypeScript  

---

## 🔧 Workflow / Usage (Vendor)  
1. Vendor logs into the app 
2. Enables location sharing / sets availability status  
3. Adds or updates vegetable items and stock  
4. Waits for incoming orders from users  
5. When an order arrives: confirms, updates inventory & status  
6. Vendor moves — app updates live location on map  

---

## 🚀 Future Improvements / Features to Add  
- In-app notifications for new orders  
- Order history & management (completed / pending)  
- Vendor rating & reviews  
- Payment integration (if needed)  
- Better UI / UX for inventory & order management  
- Offline support & sync  

---

