# Project 1 | Classify gender from text

- Machine Learning accuracy 96 %
- Use LogisticRegression

## Tools / Modules

- sklearn
- pythainlp
- numpy
- pandas
- Twint

## API

```http
  GET https://classifygenderthai.herokuapp.com/?word=${word}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `word`      | `string` | **Required**. word to fetch |

## Website
![Max5000_30](./Pic/webpage.png)
**ทดลอง Machine Learning นี้ >> คลิ้กลิ้งด้านล่าง**
- [https://classifygenderthai.netlify.app/](https://classifygenderthai.netlify.app/)

## Data collection
ดึงข้อมูลมาจาก Twitter ด้วย Twint จำนวนประมาณ 250,000 ข้อความ แต่เนื่องด้วยข้อจำกัดทางอุปกรณ์และ Server จึงนำข้อมูลมาใช้เพียง 5,000 ข้อความ และใช้ feature 10,000 feature ( 1 feature ต่อ 1 คำ ) ในการจำแนก

## Data visualization
![Max5000_30](./Pic/Max5000_30.jpg)
นี่คือคำที่ถูกพิมพ์มากที่สุด 30 คำจาก 5000 ข้อความ พบว่าส่วนใหญ่เป็นคำพื้นฐาน บางคำเป็นสัญลักษณ์
![menmost30](./Pic/menmost30.jpg)
นี่คือคำที่ผู้ชายพิมพ์มากที่สุด 30 คำจาก 5000 ข้อความ พบว่าส่วนใหญ่เป็นคำลงท้ายประโยค บางคำเป็นสัญลักษณ์
![womenmost30](./Pic/womenmost30.jpg)
นี่คือคำที่ผู้หญิงพิมพ์มากที่สุด 30 คำจาก 5000 ข้อความ พบว่าส่วนใหญ่เป็นคำลงท้ายประโยค บางคำเป็นสัญลักษณ์
![womenreletive30](./Pic/womenreletive30.jpg)
นี่คือคำที่สัมพันธ์กับผู้ชายมากที่สุดเทียบกับคำที่ผู้ชายพิมพ์มากที่สุด พบว่าส่วนใหญ่เป็นคำลงท้ายประโยค บางคำเป็นสัญลักษณ์ บางคำเป็นชื่อ Account
- คำที่สัมพันธ์กับผู้ชายมากที่สุด 30 คำ ได้แก่ 'ครับ', 'ค้าบ', 'คับ', '@', 'ผม', 'บบ', 'คับบ', 'บ', 'ครับผม', 'cwrnew','บบบ', 'ฝันดี', 'จัง', 'บบบบ', 'mynameis', 'yim', 'หน่อย', 'eln','kulthip2', 'งดัง', 'best', 'ohmpawatt', 'leader', 'คับๆ', 'dr', 'น่า','เลีย', 'blackla55564262', 'ยินดีต้อนรับ', 'ครับๆ' ตามลำดับ
![womenreletive30](./Pic/womenreletive30.jpg)
นี่คือคำที่สัมพันธ์กับผู้หญิงมากที่สุดเทียบกับคำที่ผู้หญิงพิมพ์มากที่สุด พบว่าส่วนใหญ่เป็นคำลงท้ายประโยค บางคำเป็นสัญลักษณ์ บางคำเป็น Link
- คำที่สัมพันธ์กับผู้หญิงมากที่สุด 30 คำ ได้แก่ 'ค่ะ', 'นะคะ', 'คะ', 'ค่า', '#', 'ตลาดนัด', 'ได้', 'ส่ง', 'ไม่','เรา', '.', 'https', '://', 'co', 't', '/', 'ราคา', 'การ์ด', 'มี','ที่', 'ใบ', '-', 'nct', 'เพิ่มเติม', 'กด', 'สอบถาม', 'แต่', 'ให้','เลย', 'พร้อม' ตามลำดับ

## Authors

- [@NineNatthanarong](https://github.com/NineNatthanarong)