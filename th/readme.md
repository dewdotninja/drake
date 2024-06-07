## รวบรวมโน๊ตบุคที่แปลเป็นภาษาไทย

### ปัญหาที่พบ

#### 7 มิย. 2567

จากวีดีโอแสดงการติดตั้ง

https://youtu.be/FbjwCow3tiI?si=NDbYN36ExCRvqz1z

เมื่อรันตัวอย่าง dynamical_systems.ipynb จาก tutorial มีเซลล์หนึ่งที่เกิด error ไม่สามารถแสดง diagram ได้เนื่องจากหาโปรแกรม dot ไม่เจอ วิธีแก้ไข (หาได้จาก stack overflow) คือลงโปรแกรม graphviz ใน terminal

```console
sudo apt install graphviz
sudo apt install graphviz-dev
```
แล้วทดลองตรวจสอบโดยคำสั่ง
```
dot -V
``` 
จะเห็นข้อความทำนองนี้ 
```
dot - graphviz version 2.43.0 (0)
```
หลังจากนี้ก็จะสามารถแสดง diagram ได้ 

https://stackoverflow.com/questions/65493246/graph-write-png-doesnt-work-on-linux-dot-not-found-in-path-graphviz-and-pyd

บน MAC-OSX ใช้
```
brew install graphviz
```




