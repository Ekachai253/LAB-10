###นายเอชัย ภมรสุขนิรันดิ์ 57030253
#ใบงานที่ 10
##การเขียนโปรแกรมกราฟฟิกส์ด้วย GDI+ (2)
##กล่าวนำ
ใบงานนี้ มีวัตถุประสงค์ เพื่อให้นักศึกษา ได้รู้จักกับ GDI+ ซึ่งจะช่วยให้นักษาสามารถ
* วาดรูปร่างต่างๆ โดยใช้ GDI+ ได้


## การวาดเส้นตรง
การวาดเส้นตรง เป็นการเชื่อมต่อระหว่างจุด จำนวน 2 จุด  โดยใช้ออบเจกต์ Pen เป็นตัวกำหนดลักษณะของเส้น 

แก้ไข code ต่อไปนี้ในฟังก์ชัน private void Form1_Paint(object sender, PaintEventArgs e)
* [Graphics.DrawLine Method](https://msdn.microsoft.com/en-us/library/system.drawing.graphics.drawline(v=vs.110).aspx)

<p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-1.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/1.jpg)


## การวาดเส้นตรงด้วย pen style และ brush
* [PenType Enumeration](https://msdn.microsoft.com/en-us/library/system.drawing.drawing2d.pentype(v=vs.110).aspx)
 <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-2.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/2.jpg)


## การกำหนดจุดปลายของเส้นตรงด้วย style แบบต่างๆ

* [LineCap Enumeration](https://msdn.microsoft.com/en-us/library/system.drawing.drawing2d.linecap(v=vs.110).aspx)
<p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-3.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/3.jpg)


##การวาดเส้นโค้ง
การวาดเส้นโค้ง ทำได้โดยการกำหนดจุดไว้ใน array ของ point แล้วส่งให้กับฟังก์ชัน DrawCurve ดังตัวอย่างต่อไปนี้
<p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-4.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/4.jpg)

## การวาดเส้นโค้งด้วย Graphics path
 <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-5.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/5.jpg)

## การวาดรูปทรงสี่เหลี่ยม
### การวาดสี่เหลี่ยมครั้งละรูปเดียว
  <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-6.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/6.jpg)

###การวาดสี่เหลี่ยมพร้อมกันครั้งละหลายๆ รูป
  <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-7.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/7.jpg)


## การวาดวงกลมและวงรี
วงรีต่างจากวงกลมตรงที่เส้นผ่านศูนย์กลางในแกนตั้งและแกนนอนจะไม่เท่ากัน ในภาษาโปรแกรมส่วนใหญ่จะมีเฉพาะฟังก์ชันวาดวงรี ถ้าต้องการวาดวงกลม ให้กำหนดเส้นผ่านศูนย์กลางในแกนตั้งและแกนนอนให้เท่ากัน
   <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-8.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/8.jpg)


## การวาดส่วนโค้ง (Arc)
   <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-9.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/9.jpg)

## การวาดรูป Pie
  <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-10.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/10.jpg)

## การสร้าง graphics path จากรูปต่างๆ 
  <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-11.png">

![](https://github.com/Ekachai253/LAB-10/blob/e86e9f0d35f8d28d16173e0c9d08161decdd89a3/imgs/11.jpg)
#แบบฝึกหัด
ให้วาดรูปวิว โดยใช้รูปร่างต่างๆ ที่ทำการทดลองใน Lab นี้

##รูปวิว
![](https://github.com/Ekachai253/LAB-10/blob/3a2a3cc1e31fa6d364b3963f5359a17e09736b56/imgs/12.jpg)

##เอกสารอ้างอิง
### [Graphics Methods](https://msdn.microsoft.com/en-us/library/system.drawing.graphics_methods(v=vs.110).aspx)
### [System.Drawing Namespace](https://msdn.microsoft.com/en-us/library/system.drawing(v=vs.110).aspx)
### [GDI+ .NET Color & HatchStyle Chart](https://drewnoakes.com/snippets/GdiColorChart/)

