# REST

ทดสอบการใช้งาน REST โดยใช้ PHP จำลองการรับค่า name ผ่าน url
เช่น Request มาเป็น http://localhost/REST/?name=php จะได้ Return เป็น {"status":200,"status_message":"book found","data":267}

กรณีที่ไม่พบข้อมูลที่กำหนดมาใน name
จะได้ return กลับเป็น 
{
status: 200,
status_message: "book not found",
data: null
}

กรณีที่เรียก URL ไม่ถูกต้อง
http://localhost/REST/?a

{
status: "400",
status_message: "Invalid Request",
data: null
}
