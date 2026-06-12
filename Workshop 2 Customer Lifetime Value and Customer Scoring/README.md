## Customer Lifetime Value and Customer Scoring
#### :bookmark:	 Customer's Analytic Data Discovery
###### Analyze data for discuss with business user and agree for next topic for detail analysis. Analyzing shopping time allows businesses to segment customers based on their shopping patterns and behavior. Businesses can personalized offers to each segment

#### :bookmark: Data Limitation
###### Only data with customer_code and Ignore null value

#### :key:	Insight 1 CLV Distribution
![CLV Distributions](../data/sample/clv_distributions.png)

#### 📊 กราฟบอกอะไร?
- **Historical CLV** (ซ้าย): เบ้ขวามาก — ลูกค้าส่วนใหญ่ (tail ด้านซ้าย) มี CLV ต่ำ มีกลุ่มใช้จ่ายสูงอยู่ไม่กี่ราย (pareto principle)
- **Predicted CLV 12mo** (ขวา): กระจายตัวใกล้เคียง historical แต่峰值 shift ไปทางขวาเล็กน้อย แสดงถึงโอกาสในการเพิ่มมูลค่า
- **Insight**: กลุ่ม top 20% น่าจะสร้างรายได้ 60-80% ให้ธุรกิจ — จำเป็นต้อง identify และรักษากลุ่มนี้

> **💡 วิเคราะห์ต่อ:** หาก CLV distribution แยกเป็นหลาย peak อาจมี hidden segments ที่ควรแยกวิเคราะห์เพิ่มเติม

#### :key:	Insight 2 Customer Tier & Spending
![Tier Spending](../data/sample/tier_spending.png)

#### 📊 กราฟบอกอะไร?
- **Bronze**: spending ต่ำ median อยู่ใกล้ 0 — ลูกค้าไม่ active ต้องกระตุ้น
- **Silver**: spending ปานกลาง มีความผันผวนสูง (outliers เยอะ) — โอกาสในการ upsell
- **Gold**: spending สูงขึ้น เริ่มเห็นความสม่ำเสมอ
- **Platinum**: spending สูงที่สุด median ชัดเจน — กลุ่มนี้คือรายได้หลัก ควรรักษาเป็นพิเศษ
- **Box overlap**: ระหว่าง Silver-Gold มี overlap มาก ควรปรับ scoring model ให้แยกกลุ่มชัดเจนขึ้น

> **💡 แนวทางต่อยอด:**
> - Bronze → ส่ง campaign reactivation (ส่วนลดพิเศษ)
> - Silver → upsell membership tier
> - Gold → บริการพิเศษเพื่อเลื่อนเป็น Platinum
> - Platinum → VIP program + referral incentive

#### :key:	Insight 3 When did the customer last purchase ?
###### Focus on continued customer and analyze lose customer

#### :key:	Insight 4 Product Hierachy by Life Stage
###### Track to focus item by life's stage

---

📓 **[Open Notebook →](../notebooks/02_clv_scoring.ipynb)** | RFM Analysis + CLV Calculation + Customer Scoring
