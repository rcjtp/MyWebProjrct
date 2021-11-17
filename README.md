# WinWin
โปรเจคMoblie Application เป็นระบบวินมอเตอร์ไซค์รับ-ส่งลูกค้าผ่าน Application จัดทำโดย จตุพร เรือนฟ้า
### Features
- ปักหมุดสถานที่ที่ต้องการจะไป และ สถานที่ที่ตนเองอยู่
- กดเรียกรถเพื่อให้วินมอเตอร์ไซค์เข้าไปรับ-ส่ง
- เลือกชำระเงินด้วยเงินสดหรือผ่าน Mobile Banking
- สามารถรู้ราคาค่าโดยสารหลังจากที่ปักหมุด
### Exmple Code
```
         child: Column(
          children: <Widget>[
            Image.asset(
              'asset/image/logo.png',
              width: 250,
              height: 300,
            ),
            Text(
              'เข้าสู่ระบบของคุณ',
              style: TextStyle(
                fontSize: 22,
                color: Colors.black,
              ),
            ),
            Container(
              margin: EdgeInsets.fromLTRB(90, 10, 20, 0),
              padding: new EdgeInsets.only(top: 0),
            ),
            Container(
              margin: EdgeInsets.only(),
              padding: EdgeInsets.fromLTRB(20, 7, 20, 3),
              child: TextFormField(
                decoration: new InputDecoration(
                  filled: true,
                  fillColor: Colors.orangeAccent.shade100,
                  labelText: "Username",
                  border: OutlineInputBorder(
                    borderRadius: BorderRadius.circular(10),
                  ),
                ),
                controller: getName,
              ),
            ),
            Container(
              margin: EdgeInsets.only(),
              padding: EdgeInsets.fromLTRB(20, 7, 20, 3),
              child: TextFormField(
                obscureText: _obscureText,
                decoration: new InputDecoration(
                  filled: true,
                  fillColor: Colors.orangeAccent.shade100,
                  labelText: "Password",
                  border: OutlineInputBorder(
                    borderRadius: BorderRadius.circular(10),
                  ),
                  suffixIcon: IconButton(
                      icon: Icon(_obscureText
                          ? Icons.visibility
                          : Icons.visibility_off),
                      onPressed: () {
                        setState(() {
                          _obscureText = !_obscureText;
                        });
                      }),
                ),
                controller: getPass,
              ),
            ),
```            
  ## Credit
  610107030014@dpu.ac.th
  ## License
