## Customer Segmentation and Product Recommendation
### :honeybee:	 :honeybee:	 HDI HOLDINGS :honeybee: :honeybee:	
### 1. Customer Segmentation
#### :bouquet: Data understanding data member
* Transaction 2021 Jan-Jun
* Transaction 2022 Jan-Dec
* Transaction 2023 Jan-July

#### :bouquet: Data Preparation
Feature engineering from transaction data + demographics

#### :bouquet: Customer Single View
RFM + demographics merged into single view

#### :bouquet: Customer Segmentation using K-mean clustering
![K-Means Elbow](../data/sample/kmeans_elbow.png)
![Segments PCA](../data/sample/segments_pca.png)

#### 📊 กราฟบอกอะไร?
**Elbow Method (ซ้าย):**
- จุด elbow อยู่ที่ **K=4** — ค่า inertia ลดลงช้าลงหลังจากนี้ ดังนั้น 4 segments เป็นจำนวนที่เหมาะสมที่สุด
- Silhouette Score (ขวา) ยิ่งสูงยิ่งดี — ควรเลือก K ที่ balance ระหว่าง inertia ต่ำและ silhouette สูง

**PCA Projection (ล่าง):**
- แสดงการกระจายของลูกค้าใน 2 มิติ (PCA ลด dimension จาก 5 เหลือ 2)
- แต่ละ cluster แยกจากกันค่อนข้างชัดเจน แม้จะมี overlap บางส่วน (ธรรมชาติของข้อมูลจริง)
- Cluster 0 (ม่วง) และ 2 (เขียว) แยกตัวเด่นชัด — มีพฤติกรรมแตกต่างจากกลุ่มอื่น

#### :bouquet: Comparative Analysis of customer segments Over a Six-Month Period

#### 📊 การวิเคราะห์ Segment Profile (from notebook)
| Cluster | ขนาด | Recency | Frequency | Monetary | อายุเฉลี่ย | รายได้เฉลี่ย | ลักษณะ |
|---------|------|---------|-----------|----------|----------|------------|--------|
| 0 | — | ต่ำ | สูง | สูง | — | — | 🏆 ลูกค้า VIP ซื้อถี่ ใช้จ่ายสูง |
| 1 | — | กลาง | กลาง | กลาง | — | — | 👥 ลูกค้าทั่วไป |
| 2 | — | สูง | ต่ำ | ต่ำ | — | — | ⚠️ เสี่ยงเสียลูกค้า |
| 3 | — | ต่ำ | กลาง | กลาง-สูง | — | — | 💎 มีศักยภาพสูง |

> **💡 วิเคราะห์ต่อ:**
> - กลุ่ม 0: ทำ VIP program + exclusive benefit
> - กลุ่ม 1: เพิ่ม engagement ด้วย personalized recommendation
> - กลุ่ม 2: วิเคราะห์สาเหตุที่หายไป + win-back campaign
> - กลุ่ม 3: push ให้เป็น VIP ด้วย targeted upsell

### 2. Segment Movement Analysis
###### วิเคราะห์การย้ายกลุ่มของลูกค้าในแต่ละช่วงเวลา — ช่วยให้เข้าใจ lifecycle ของลูกค้า

### 3. Product Recommendation
#### การเกาะกลุ่มของ Product — Association Rules

#### 📊 วิเคราะห์ต่อ:
> - ใช้ Association Rules (Apriori) หาคู่สินค้าที่ซื้อด้วยกันบ่อย
> - แนะนำ Cross-Sell: "ลูกค้าที่ซื้อ A มักซื้อ B ด้วย"
> - จับคู่สินค้าในตะกร้าเพื่อจัดโปรโมชันแบบ bundle

---

📓 **[Open Notebook →](../notebooks/04_segmentation_recommendation.ipynb)** | K-Means Clustering + Association Rules (Market Basket)
