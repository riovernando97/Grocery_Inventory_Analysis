# Grocery_Inventory_Analysis
## Project Objective
Menganalisis kinerja penjualan, efisiensi manajemen stok, serta kinerja supplier dari data inventori toko grosir untuk membantu pengambilan keputusan operasional yang lebih efisien.

## Dataset
- <a href = https://github.com/riovernando97/Documenting_Example/blob/73565fb63e79686b927651447e1b84c19bdaaaa7/CoffeeSalesData.xlsx>Coffee_Sales_Dataset</a>
  
## Questions (KPI)
  - Produk dan kategori mana yang paling laku dan menguntungkan ?
  - Apakah stok barang dikelola dengan efisien (tidak overstock/understock) ?
  - Supplier mana yang paling andal dalam memenuhi kebutuhan toko ?
  - Bagaimana tingkat perputaran stok (inventory turn over rate) di setiap gudang ?
  - Produk mana yang mendekati masa kadaluarsa dan perlu promosi ?
  
## Process
  - Data cleaning dan data transform menggunakan excel (ubah format tanggal, anomali data, pengurutan, dan missing values)
  - Menambah kolom kalkulasi baru :
    - <b>Total_Sales</b> = Unit_Price * Sales_Volume
    - <b>Stock_Values</b> = Unit_Price * Stock_Quantity
    - <b>Profit</b> = Total_Sales * Percentage
    - <b>Days_to_Expire</b> = Expiration_Date - TODAY()

## KPI Metrics
  - Total Sales
    - Mengukur total pendapatan
  - Inventory Turnover Rate
    - Efisiensi rotasi stok
  - Stock availability Rate
    - Ketersediaan produk
  - Reorder Date
    - Mengidentifikasi kebutuhan produk
  - Gross Profit Margin
    - Mengukur profitabilitas
  - Average Shelf Life Remaining
    - Melihat umur stok tersisa

## Dashboard (Tableau)
  <img>https://github.com/riovernando97/Grocery_Inventory_Analysis/blob/d2b2cc1c2ae9213dbeb028ac58abfd7d1c35b8ae/Grocery%20Inventory%20Analysis%20Dashboard.jpg</img>

## Project Insight
-	Produk dengan kategori <b>Beverages</b> memiliki margin keuntungan tertinggi (rata-rata 16%).
-	Kategori <b>Fruits & Vegetables</b> menyumbang 26% total penjualan namun memiliki resiko kadaluarsa tertinggi.
-	Efisiensi perputaran stok lebih stabil pada tahun 2024 dan mengalami fluktuasi pada tahun 2025.
-	Gudang dengan kategori <b>Dairy</b> menjadi gudang yang paling efisien.
-	Pada supplier <b>Katz</b>, turnover tinggi stok cepat berpindah dan kemungkinan stok tidak stabil atau demand fluktuatif.

## Final Conclusion :
-	Tingkatkan reorder otomatis untuk produk-produk katagori <b>Beverages</b> dengan turnover tinggi (misalnya diatas 70%).
-	Promosikan produk yang mendekati kadaluarsa atau yang mudah kadaluarsa untuk menghindari kerugian.
-	Evaluasi supplier yang sering memiliki status "Backordered".
-	Optimalkan distribusi stok antar gudang untuk menghindari overstock.
-	Fokus promosi produk dengan margin tinggi (misal <b>Beverages</b>, <b>Fruits & Vegetables</b>).

  
