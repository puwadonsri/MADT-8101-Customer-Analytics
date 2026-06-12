## Churn Scoring and Campaign Response Scoring

#### :shopping: CURRENTLY FOCUS BEAUTY PASS TIER ON SPEND PER 12 MONTH ONLY

#### :shopping: Current Scoring
## CV = Purchase value

#### :shopping: New scoring
#### > เมื่อลูกค้าเขียนรีวิวบนเว็บไซต์ และมีการเข้ามาอ่านรีวิว ส่งผลให้ยอดขายเพิ่มขึ้นโดยพฤติกรรมลูกค้าส่วนใหญ่จะอ่านรีวิวก่อนซื้อทุกครั้ง
#### > สินค้าแนะนำมีความแม่นยำมากขึ้น
#### > ลูกค้าใช้บริการของในร้านเดียวเพื่อสะสมพ้อยมากขึ้นทำให้พ้อยกระจายไปยังร้านอื่น ๆ น้อยลง

#### :shopping: Scoring Model
#### > :basket: Spend per 12 months 50%
#### > :basket: Point form review on website 10%
#### > :basket: Buy exclusive product 20%
#### > :basket: Training base on product 20%

#### CHURN MODEL — ROC Curve
![ROC Curve](../data/sample/churn_roc.png)

#### Feature Importance
![Feature Importance](../data/sample/churn_feature_importance.png)

#### Campaign Priority Scoring
![Campaign Priority](../data/sample/campaign_priority.png)

---

📓 **[Open Notebook →](../notebooks/03_churn_scoring.ipynb)** | Churn Prediction (Random Forest) + Campaign Response Scoring
