#ใบงานที่ 4
# นายวีรภัทร	แก่นจันทร์	57030222
เรื่อง การใช้งานคำสั่งเกี่ยวกับการแสดงผลบน Text Mode ขั้นพื้นฐานในภาษา C#
##วัตถุประสงค์
1. เพื่อให้นักศึกษาบอกชื่อ method ที่ใช้ในการแสดงผลบน Text Mode ขั้นพื้นฐานในภาษา C# ได้
2. เพื่อให้นักศึกษาสามารถใช้คำสั่งแสดงผลทางหน้าจอ เบื้องต้นได้

##ลำดับขั้นการทดลอง
###การเตรียมการก่อนการทดลอง
  * เปิดโปรแกรม Visual Studio 
  *  เลือก File >>New Project >> เลือก Console Application 
![P1](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P1.png)
  *  ช่อง Name ใส่ชื่อของ project (ในที่นี้คือ Lab4)
  *  ช่อง Location ใส่ชื่อ folder ที่เป็นที่ตั้งของ Project (ในที่นี้ สมมติเป็น E:\vslab)
  *  ช่อง Solution name ให้ใส่ชื่อ Solution โดยปกติก็ให้ปล่อยไว้อย่างนั้น 
  *  กดปุ่ม OK โปรแกรม Visual Studio จะสร้าง project ชื่อ “lab4”ภายใต้ solution “lab4” และไฟล์ lsb4.cs ซึ่งมี source code ดังรูป 

![P2](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P2.png)

ส่วนสำคัญของโปรแกรม lab4.cs  คือบรรทัดที่ 1 “using System” และเมธอด Main(string[] args)


 *  ให้ลบ source code ในบรรทัดที่ 2-5 ออกไปก่อน เนื่องจากเป็น assembly ที่ไม่จำเป็นต่อการทำงานของโปรแกรม 

## 1. การทดลองเมดธอด Console.Write()
* ให้เพิ่ม บรรทัดต่อไปนี้ลงไปในในเมธอด Main()
```csharp 
    Console.Write(“Hello”);
```
ดังปรากฏในบรรทัดที่ 9 ของรูปด้านล่าง 

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P3.png)
 
 * สั่ง Run โปรแกรม เพื่อดูผลการทดลอง 

####บันทึกผลการทดลอง

![](https://github.com/weerapat1995/LAB-04/blob/master/imgs/4.1.png)

หน้าจอจะแสดงคำว่า Hello ตามที่พิมพ์

แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้    

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P4.png)

 * สั่ง Run โปรแกรมและบันทึกผลที่ได้จากการรันโปรแกรม
 * การรันแล้วทำให้หน้าจอ console ยังคงแสดงผลค้างอยู่นั้น ให้เลือกเมนู Debug -> Start Without Debugging (Ctrl+F5) มิฉะนั้น หน้าจอ console จะหายไปอย่างรวดเร็ว
 
![](https://github.com/weerapat1995/LAB-04/blob/master/imgs/4.2.png)

หน้าจอจะแสดงคำว่า Hello World ตามที่พิมพ์

### คำถาม 4.1 

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร  จงอธิบาย

เป็นอย่างที่คิดไว้ เมื่อใช้คำสั่ง Console.Write แล้วตามด้วยคำที่ต้องการโปรแกรมก็จะแสดงผลตามที่พิมพ์ลงไป 


## 2. การทดลองเมดธอด Console.WriteLine()

แก้โปรแกรมในเมดธอด Main() ให้เป็นดังรูปต่อไปนี้

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P5.png)

 * สั่ง Run โปรแกรม เพื่อดูผลการทดลอง 

บันทึกผลที่ได้จากการรันโปรแกรม

![](https://github.com/weerapat1995/LAB-04/blob/master/imgs/4.3.png)

หน้าจอจะแสดงคำว่า Hello และเว้นลงไปหนึ่งบรรทัด

แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P6.png)

 * สั่ง Run โปรแกรมและบันทึกผลที่ได้จากการรันโปรแกรม
 
![](https://github.com/weerapat1995/LAB-04/blob/master/imgs/4.4.png)

หน้าจอจะแสดงคำว่า Hello World แต่จะเว้นบรรทัดทุกๆคำสั่ง  

###คำถาม 4.2

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร  จงอธิบาย

เป็นอย่างที่คิด โดยที่หน้าจอจะแสดงคำ ตามคำสั่งที่พิมพ์ลงไปแล้วเมื่อเสร็จสิ้นคำสั่งก็จะเว้นบรรลงหนึ่งบรรทัด

### คำถาม 4.3 

จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()

Console.Write() จะแสดงคำตามที่พิมพ์ต่อกันไปเรื่อยๆ แต่ Console.WriteLine() เมื่อจบคำสั่งจะเว้นบรรทัด

##สรุปผลการทดลอง

จากการทดลองทั้ง Console.Write() และ Console.WriteLine() เป็นคำสั่งที่ใช้ในการแสดงคำตามที่ต้องการ โดยจะพิมพ์คำสั่งต่อกันไปเรื่อยๆ Console.Write() ก็จะแสดงผลตามที่พิมพ์ต่อกันไป
แต่ Console.WriteLine() จะเว้นบรรทัดหลังจากแสดงคำเสร็จ ในแต่ละคำสั่ง

# นายวีรภัทร	แก่นจันทร์	57030222
