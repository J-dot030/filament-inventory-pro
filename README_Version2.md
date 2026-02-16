# Filament Inventory Pro - Auto-Lookup Edition

A smart inventory management system for 3D printer filament that **automatically looks up product information** from QR codes. No manual data entry needed!

## 🎯 How It Works

### The Smart Workflow:
1. **Print QR Code Labels** for each unique filament type (brand, color, material)
2. **Add to Product Database** - Define what each QR code represents (do this once)
3. **Scan to Add** - Scan the QR code, enter only the quantity, done!
4. **System Automatically** pulls all product info from your database

### Two-Part System:
- **Product Database**: Master list of all your filament types (Prusament Red PLA, MatterHackers Blue PETG, etc.)
- **Inventory**: Your actual spools with quantities

## ✨ Key Features

✅ **Automatic Product Lookup** - Scan QR code, system finds all details automatically
✅ **Quantity-Only Entry** - Just enter how many spools you're adding
✅ **Product Database Management** - Easy UI to manage product information
✅ **QR Code Generator Ready** - Use QR code generator to create labels
✅ **Low Stock Alerts** - Visual warnings with customizable thresholds
✅ **Statistics Dashboard** - Real-time inventory metrics
✅ **Dark Mode** - Easy on the eyes
✅ **Search & Filter** - Find items by brand or name
✅ **Data Export** - JSON and CSV formats
✅ **Bulk Import** - Import multiple inventory items at once
✅ **Responsive Design** - Works on mobile and desktop

## 🚀 Quick Start

### Live Demo:
https://j-dot030.github.io/Filament-Inventory/

### Initial Setup:

1. **Go to "Product DB" Tab**
2. **Add Your Filament Types:**
   - Generate or write down QR codes for each unique filament
   - Click "Add New Product"
   - Enter: QR Code ID, Brand, Color, Material Type, Threshold
   - Save

3. **Print QR Code Labels**
   - Use any QR code generator (e.g., qr-server.com)
   - Print and stick labels on your filament spools

4. **Start Scanning**
   - Click "SCAN FILAMENT SPOOL"
   - Point camera at QR code label
   - Enter quantity you have
   - Done! System auto-fills everything else

## 📋 Detailed Instructions

### Setting Up Product Database

Each "Product" represents a unique filament type. Example:
- **QR Code ID**: `QR-PRUSAMENT-RED-PLA`
- **Brand**: Prusament
- **Color**: Red
- **Material Type**: PLA
- **Threshold**: 2 (alert when below 2 spools)

### Creating QR Code Labels

1. Go to https://qr-server.com/qr-code-generator/
2. Enter the QR Code ID (e.g., `QR-PRUSAMENT-RED-PLA`)
3. Download and print
4. Stick on your filament spool

### Scanning Workflow

1. Click **"SCAN FILAMENT SPOOL"**
2. Allow camera access
3. Point camera at the QR code on your spool
4. Dialog appears with product details auto-filled
5. Enter quantity (1, 2, 3, etc.)
6. Click "Add to Inventory"
7. Done! Your inventory updates automatically

### Data Management

**Export Data:**
- Click "Export JSON" for backup
- Click "Export CSV" for spreadsheet use

**Import Inventory:**
- Click "Bulk Import"
- Format: `[{"id":"QR-123","qty":2},{"id":"QR-456","qty":1}]`
- Paste and import

## 🏗️ Technical Details

### Data Structure:

**Products** (master list):
```json
{
  "id": "QR-PRUSAMENT-RED-PLA",
  "brand": "Prusament",
  "color": "Red",
  "type": "PLA",
  "threshold": 2
}