# Filament Inventory Pro - Feature Documentation

## 1. Dashboard & Inventory Grid
- Visual tile layout of all filament spools
- Real-time quantity display
- Brand and color identification
- Low-stock visual indicators with pulsing animation
- One-click quantity adjustment (+ and -)

## 2. QR Code Scanning
- Uses html5-qrcode for browser-based scanning
- Automatic item registration on first scan
- Quantity increment on subsequent scans
- Mobile-friendly camera interface
- Works with any QR code format

## 3. Inventory Management
### Add Items
- Manual entry form with brand, color, material type
- Customizable stock thresholds
- Auto-generated QR code IDs
- Preset default threshold from settings

### Edit Items
- Click pencil icon on any tile to edit
- Update all properties including quantity
- Change threshold levels dynamically

### Delete Items
- One-click deletion with confirmation
- Automatic activity log entry
- Prevents accidental loss of data

## 4. Search & Filter
- Real-time search by any text
- Brand-based filtering via dropdown
- Combined search + filter capabilities
- Instant results as you type

## 5. Data Export
### JSON Export
- Complete data backup format
- Suitable for data sharing
- Preserves all item properties
- Timestamped filenames

### CSV Export
- Spreadsheet-compatible format
- Includes: Brand, Color, Type, Quantity, Threshold, QR ID
- Easy import into Excel/Google Sheets
- Human-readable format

## 6. Bulk Import
- Import multiple items at once
- JSON array format input
- Validation and error handling
- Activity log tracking
- Append mode (doesn't delete existing items)

## 7. Statistics Dashboard
### Metrics Displayed
- **Total Items**: Number of unique filament spools
- **Total Quantity**: Sum of all spool quantities
- **Low Stock Items**: Count of items below threshold
- **Unique Brands**: Number of different manufacturers

### Future Enhancements
- Category breakdown charts
- Usage trends over time
- Projected stock depletion dates

## 8. Activity Log
- Timestamped entries for all actions
- Last 100 entries maintained
- Includes: scans, additions, deletions, edits
- Colorized with emojis for quick scanning
- Scrollable history view

## 9. Dark Mode
- Toggle button in header
- Full theme support for all elements
- Preference saved to localStorage
- Easy on the eyes for night use
- Maintains readability and contrast

## 10. Settings & Customization
### User Settings
- **User Name**: Display name for profiles
- **Default Threshold**: Auto-filled for new items
- **Cloud Sync Email**: Ready for future cloud features

### Data Management
- **Clear All Data**: Nuclear option with confirmation
- **Save Settings**: Persists to localStorage

## 11. Multi-User Support
- Settings per-user configuration
- Future ready for cloud sync
- Individual user preferences
- Activity attribution capability

## 12. Cloud Sync (Framework Ready)
- Email field for sync configuration
- Structure for future cloud integration
- Data export capability for manual sync
- JSON format compatible with APIs

## 13. Barcode/Label Printing (Framework Ready)
- QR code ID field for each item
- Export data contains all label info
- Ready for integration with label printing APIs
- Brand, color, and type info available for custom labels

## 14. Low Stock Alerts
- Configurable per-item threshold
- Visual pulsing animation
- "LOW STOCK" warning badge
- Red border highlighting
- Distinct background color

## 15. Responsive Design
- Mobile-first approach
- Grid layout adapts to screen size
- Touch-friendly buttons and controls
- Full-width on small screens
- Multi-column on larger screens

## Future Enhancement Ideas
1. Camera QR code generation for sharing inventory
2. Weight tracking (grams of filament used)
3. Cost per item tracking
4. Supplier information storage
5. Print history and usage statistics
6. Push notifications for low stock
7. Collaborative sharing via cloud
8. API integration for automatic orders
9. Integration with 3D slicer software
10. Printer compatibility tagging