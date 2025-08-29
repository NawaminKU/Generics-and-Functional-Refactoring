# Generics-and-Functional-Refactoring
ส่วนที่ 0: ไฟล์เริ่มต้น
    - นิสิตจะได้รับโปรเจกต์ที่มี 3
ไฟล์: Product.java, ProductAnalytics.java, และ ProductAnalyticsTest.java
(ซึ่งมีเทสต์ที่สมบูรณ์อยู่แล้ว)

ส่วนที่ 1: สร้าง Generic Class
    - สร้างไฟล์ใหม่ Pair.java
    - สร้าง Generic Class ชื่อ Pair<K, V> ที่สามารถเก็บอ็อบเจกต์ได้ 2 ชนิด (Key และ Value)
    - Rep: มีฟิลด์ private final K key; และ private final V value;
    - Constructor: รับ key และ value
    - Getters: สร้างเมธอด getKey() และ getValue()
 
  - สร้างไฟล์ทดสอบ: สร้างคลาส PairTest ที่มีเมธอด main เพื่อทดลองสร้าง
Pair<String, Integer> และ Pair<Product, Boolean>
เพื่อพิสูจน์ว่าคลาสของคุณทำงานได้กับทุกชนิดข้อมูล

ส่วนที่ 2: Refactoring to Functional Style (75 นาที)
    - เปิดไฟล์ ProductAnalytics.java
    - Refactor เมธอดทั้ง 4 ในคลาสให้เปลี่ยนมาใช้ Stream API แทน for loop
        findProductsByCategory
        getProductNamesWithPriceLessThan
        calculateTotalStockValueForCategory
        hasProductOutOfStock
