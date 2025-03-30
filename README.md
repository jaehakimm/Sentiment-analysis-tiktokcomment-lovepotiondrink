# Thai TikTok Comments Sentiment Analysis 🎭📊

🔍 **วิเคราะห์ความคิดเห็นจากคอมเมนต์ใน TikTok ด้วย AI**  
โปรเจกต์นี้เป็นการใช้โมเดล AI เพื่อวิเคราะห์ความคิดเห็นของผู้ใช้ TikTok ที่คอมเมนต์บนวิดีโอ โดยใช้ **โมเดลวิเคราะห์อารมณ์ภาษาไทย** และ **OpenAI GPT-3.5-turbo** เพื่อเปรียบเทียบผลลัพธ์

🔍 **Update add scb10x/llama-3.2-typhoon-t1-3b-research-preview  **  
เพื่อ model scb10x/llama-3.2-typhoon-t1-3b-research-preview มาด้วย

---

## 📂 โครงสร้างของโปรเจกต์

- **`dataset_tiktok-comments-scraper_2025-03-24_03-33-35-788.csv`** - ไฟล์ข้อมูลคอมเมนต์จาก TikTok  
- **`sentiment_results.csv`** - ผลลัพธ์การวิเคราะห์อารมณ์จากโมเดลไทย  
- **`sentiment_results_openai.csv`** - ผลลัพธ์การวิเคราะห์อารมณ์จาก OpenAI GPT  
- **`Thai_TikTok_Comments_Sentiment_Analysis.ipynb`** - โค้ด Jupyter Notebook สำหรับการวิเคราะห์  

---

## 🛠️ ข้อกำหนดของระบบ

- **Python** เวอร์ชัน 3.7 ขึ้นไป  
- **ไลบรารีที่ใช้:**  
  - `pandas`
  - `transformers`
  - `torch`
  - `seaborn`
  - `matplotlib`
  - `openai`

---

## 📌 ติดตั้งและใช้งาน

### 🔧 **ติดตั้งไลบรารีที่จำเป็น**
```bash
pip install pandas transformers torch seaborn openai matplotlib

🔑 ตั้งค่า API Key สำหรับ OpenAI
สมัครบัญชีที่ OpenAI

สร้าง API Key และนำไปใส่ใน Notebook

🚀 วิธีการใช้งาน
1️⃣ โหลดข้อมูลคอมเมนต์
อ่านไฟล์ dataset_tiktok-comments-scraper_2025-03-24_03-33-35-788.csv

2️⃣ วิเคราะห์อารมณ์ด้วยโมเดลไทย
ใช้โมเดล airesearch/wangchanberta-base-att-spm-uncased

จำแนกความคิดเห็นเป็น บวก (Positive), กลาง (Neutral), ลบ (Negative)

บันทึกผลลัพธ์ลงใน sentiment_results.csv

3️⃣ วิเคราะห์อารมณ์ด้วย OpenAI GPT
ใช้ GPT-3.5-turbo เพื่อจำแนกอารมณ์ของคอมเมนต์

บันทึกผลลัพธ์ลงใน sentiment_results_openai.csv

4️⃣ สร้างกราฟสรุปผล
ใช้ Seaborn และ Matplotlib ในการวิเคราะห์และแสดงผลข้อมูล

📊 ผลลัพธ์ของโปรเจกต์
เปรียบเทียบผลลัพธ์ของโมเดล
การวิเคราะห์ช่วยให้เราเห็นแนวโน้มของความคิดเห็น เช่น คอมเมนต์ในเชิงบวกหรือลบมากกว่ากัน

ช่วยให้ธุรกิจเข้าใจลูกค้า
สามารถนำไปใช้วิเคราะห์ความพึงพอใจและปรับกลยุทธ์ทางการตลาดให้เหมาะสม

🎥 ตัวอย่างวิดีโอ TikTok สาธิตการใช้งาน

<blockquote class="tiktok-embed" cite="https://www.tiktok.com/@nabeeai6/video/7485275317171424519" data-video-id="7485275317171424519" style="max-width: 605px;min-width: 325px;"> <section> <a target="_blank" title="@nabeeai6" href="https://www.tiktok.com/@nabeeai6?refer=embed">@nabeeai6</a> @iamsungstarwin ขออนุญาตน้องซุงในการทำคลิปสำรวจความเห็นคนจากคอมเม้นท์ <a title="sentimentanalysis" target="_blank" href="https://www.tiktok.com/tag/sentimentanalysis?refer=embed">#sentimentanalysis</a> <a title="lovepotion" target="_blank" href="https://www.tiktok.com/tag/lovepotion?refer=embed">#lovepotion</a> <a title="sungstarwin" target="_blank" href="https://www.tiktok.com/tag/sungstarwin?refer=embed">#sungstarwin</a> <a target="_blank" title="♬ เสียงต้นฉบับ - nabeeai" href="https://www.tiktok.com/music/เสียงต้นฉบับ-nabeeai-7485275614493805328?refer=embed">♬ เสียงต้นฉบับ - nabeeai</a> </section> </blockquote> <script async src="https://www.tiktok.com/embed.js"></script>
💡 ข้อสรุป
AI ช่วยให้เราวิเคราะห์ความคิดเห็นจากโซเชียลมีเดียได้อย่างแม่นยำ

สามารถใช้เพื่อติดตามและตอบสนองความต้องการของลูกค้าได้แบบเรียลไทม์

เปรียบเทียบผลลัพธ์จากโมเดลที่แตกต่างกันเพื่อให้ได้ข้อมูลที่แม่นยำที่สุด
