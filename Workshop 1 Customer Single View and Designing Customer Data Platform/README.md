## Customer Single View and Designing Customer Data Platform
##### :family_woman_woman_girl_girl:	 ออกแบบการเก็บข้อมูลในรูปแบบทุกอย่างของลูกค้า 1 คนให้เหลือข้อมูลเพียงแค่ 1 record ซึ่งเป็นการออกแบบ Single View ของบริษัท X Property Co.Ltd.,

#### DATA SOURCE
- ข้อมูลลูกค้า (customers.csv): demographic + registration
- ข้อมูลธุรกรรม (transactions.csv): การซื้อขาย 8,000 records
- ข้อมูลสินค้า (products.csv): 25 SKUs 5 categories

#### FEATURE ENGINEERING
- **Recency**: จำนวนวันตั้งแต่ซื้อล่าสุด
- **Frequency**: จำนวนครั้งที่ซื้อ
- **Monetary**: ยอดใช้จ่ายรวม
- **Channel Preference**: ช่องทางที่ลูกค้าใช้บ่อยที่สุด
- ข้อมูลประชากร: age, income, city

#### CUSTOMER SINGLE VIEW
![CSV Distributions](../data/sample/csv_distributions.png)

---

📓 **[Open Notebook →](../notebooks/01_customer_single_view.ipynb)** | สร้าง Customer Single View ด้วย Pandas + Feature Engineering
