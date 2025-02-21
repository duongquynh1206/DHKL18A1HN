# Cau 1.
thang = int(input("Nhập tháng (1-12): "))
nam = int(input("Nhập năm: "))
if thang < 1 or thang > 12:
    print("Tháng không hợp lệ!")
else:
    so_ngay_trong_thang = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
    if thang == 2:
        if (nam % 4 == 0 and nam % 100 != 0) or (nam % 400 == 0):
            ngay = 29
        else:
            ngay = 28
    else:
        ngay = so_ngay_trong_thang[thang - 1]
    print(f"Tháng {thang} năm {nam} có {ngay} ngày.")


# Cau 2.
import math
def giai_pt_bac_hai(a, b, c):
    if a == 0:
        if b == 0:
            if c == 0:
                return "Phương trình có vô số nghiệm"
            else:
                return "Phương trình vô nghiệm"
        else:
            return f"Phương trình có một nghiệm: {-c / b}"
    else:
        delta = b**2 - 4*a*c
        if delta > 0:
            x1 = (-b + math.sqrt(delta)) / (2*a)
            x2 = (-b - math.sqrt(delta)) / (2*a)
            return f"Phương trình có hai nghiệm phân biệt: x1 = {x1}, x2 = {x2}"
        elif delta == 0:
            x = -b / (2*a)
            return f"Phương trình có nghiệm kép: x = {x}"
        else:
            return "Phương trình vô nghiệm"
a = float(input("Nhập hệ số a: "))
b = float(input("Nhập hệ số b: "))
c = float(input("Nhập hệ số c: "))
ket_qua = giai_pt_bac_hai(a, b, c)
print(ket_qua)


# Cau 3.
ngay_trong_tuan = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"]

thu = int(input("Nhập vào thứ (1-7): "))
if thu == 1:
    print(f"Thứ {thu} là {ngay_trong_tuan[thu - 1]}")
elif thu == 2:
    print(f"Thứ {thu} là {ngay_trong_tuan[thu - 1]}")
elif thu == 3:
    print(f"Thứ {thu} là {ngay_trong_tuan[thu - 1]}")
elif thu == 4:
    print(f"Thứ {thu} là {ngay_trong_tuan[thu - 1]}")
elif thu == 5:
    print(f"Thứ {thu} là {ngay_trong_tuan[thu - 1]}")
elif thu == 6:
    print(f"Thứ {thu} là {ngay_trong_tuan[thu - 1]}")
elif thu == 7:
    print(f"Thứ {thu} là {ngay_trong_tuan[thu - 1]}")
else:
    print("Thứ không hợp lệ! Vui lòng nhập lại.")


# Cau 4.

so_nguyen = int(input("Nhập vào một số nguyên: "))
so_nguyen = abs(so_nguyen)
so_nguyen_str = str(so_nguyen)
if len(so_nguyen_str) < 3:
    chu_so_hang_tram = 0
else:
    chu_so_hang_tram = so_nguyen_str[-3]  
print(f"Chữ số hàng trăm của số {so_nguyen} là: {chu_so_hang_tram}")


# Cau 5.

thang_trong_nam = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"]
thang = int(input("Nhập vào tháng (1-12): "))
if thang == 1:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 2:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 3:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 4:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 5:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 6:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 7:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 8:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 9:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 10:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 11:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
elif thang == 12:
    print(f"Tháng {thang} là {thang_trong_nam[thang - 1]}")
else:
    print("Tháng không hợp lệ! Vui lòng nhập lại và chạy lại chương trình.")



# Cau 6.
so_nguyen = int(input("Nhập vào một số nguyên có ba chữ số: "))


if 100 <= so_nguyen <= 999 or -999 <= so_nguyen <= -100:
    
    so_nguyen = abs(so_nguyen)

    
    tram = so_nguyen // 100
    chuc = (so_nguyen // 10) % 10
    don_vi = so_nguyen % 10

    
    if tram == 1:
        ket_qua = "một trăm"
    elif tram == 2:
        ket_qua = "hai trăm"
    elif tram == 3:
        ket_qua = "ba trăm"
    elif tram == 4:
        ket_qua = "bốn trăm"
    elif tram == 5:
        ket_qua = "năm trăm"
    elif tram == 6:
        ket_qua = "sáu trăm"
    elif tram == 7:
        ket_qua = "bảy trăm"
    elif tram == 8:
        ket_qua = "tám trăm"
    elif tram == 9:
        ket_qua = "chín trăm"
    
    
    if chuc == 0 and don_vi != 0:
        ket_qua += " linh"
        if don_vi == 1:
            ket_qua += " một"
        elif don_vi == 2:
            ket_qua += " hai"
        elif don_vi == 3:
            ket_qua += " ba"
        elif don_vi == 4:
            ket_qua += " bốn"
        elif don_vi == 5:
            ket_qua += " năm"
        elif don_vi == 6:
            ket_qua += " sáu"
        elif don_vi == 7:
            ket_qua += " bảy"
        elif don_vi == 8:
            ket_qua += " tám"
        elif don_vi == 9:
            ket_qua += " chín"
    elif chuc == 1:
        ket_qua += " mười"
        if don_vi == 1:
            ket_qua += " một"
        elif don_vi == 2:
            ket_qua += " hai"
        elif don_vi == 3:
            ket_qua += " ba"
        elif don_vi == 4:
            ket_qua += " bốn"
        elif don_vi == 5:
            ket_qua += " lăm"
        elif don_vi == 6:
            ket_qua += " sáu"
        elif don_vi == 7:
            ket_qua += " bảy"
        elif don_vi == 8:
            ket_qua += " tám"
        elif don_vi == 9:
            ket_qua += " chín"
    elif chuc > 1:
        if chuc == 2:
            ket_qua += " hai mươi"
        elif chuc == 3:
            ket_qua += " ba mươi"
        elif chuc == 4:
            ket_qua += " bốn mươi"
        elif chuc == 5:
            ket_qua += " năm mươi"
        elif chuc == 6:
            ket_qua += " sáu mươi"
        elif chuc == 7:
            ket_qua += " bảy mươi"
        elif chuc == 8:
            ket_qua += " tám mươi"
        elif chuc == 9:
            ket_qua += " chín mươi"
        
        if don_vi == 1:
            ket_qua += " mốt"
        elif don_vi == 2:
            ket_qua += " hai"
        elif don_vi == 3:
            ket_qua += " ba"
        elif don_vi == 4:
            ket_qua += " bốn"
        elif don_vi == 5:
            ket_qua += " lăm"
        elif don_vi == 6:
            ket_qua += " sáu"
        elif don_vi == 7:
            ket_qua += " bảy"
        elif don_vi == 8:
            ket_qua += " tám"
        elif don_vi == 9:
            ket_qua += " chín"
    else:
        ket_qua += ""

    
    print("Cách đọc:", ket_qua)
else:
    print("Vui lòng nhập một số nguyên có ba chữ số.")


# Cau 7.

diem_tk = float(input("Nhập vào điểm tổng kết (0.0 - 10.0): "))
if 0.0 <= diem_tk <= 3.0:
    hoc_luc = "Kém"
elif diem_tk == 4.0:
    hoc_luc = "Yếu"
elif 5.0 <= diem_tk <= 6.0:
    hoc_luc = "Trung bình"
elif 7.0 <= diem_tk <= 8.0:
    hoc_luc = "Khá"
elif 9.0 <= diem_tk <= 10.0:
    hoc_luc = "Giỏi"
else:
    hoc_luc = "Điểm không hợp lệ!"
print(f"Học lực của học sinh: {hoc_luc}")


# Cau 8.
# Cau8.
luong_can_ban = 1350000
TNCT = int(input("Nhập vào thâm niên công tác (số tháng): "))
if TNCT < 12:
    he_so = 2.34
elif 12 <= TNCT < 36:
    he_so = 3.33
elif 36 <= TNCT < 60:
    he_so = 3.66
else: 
    he_so = 3.99
luong = he_so * luong_can_ban
print(f"Lương của nhân viên là: {luong} đồng")


# Cau 9.

so_kw = int(input("Nhập số KW điện tiêu thụ: "))
if 0 <= so_kw <= 100:
    tien_dien = so_kw * 2000
elif 101 <= so_kw <= 200:
    tien_dien = 100 * 2000 + (so_kw - 100) * 2500
elif 201 <= so_kw <= 300:
    tien_dien = 100 * 2000 + 100 * 2500 + (so_kw - 200) * 3000
elif so_kw > 300:
    tien_dien = 100 * 2000 + 100 * 2500 + 100 * 3000 + (so_kw - 300) * 5000
else:
    tien_dien = 0
    print("Số KW không hợp lệ!")
print(f"Số tiền điện phải trả là: {tien_dien} đồng")


# Cau 10.


# Cau 11.
ngay = int(input("Nhập ngày: "))
thang = int(input("Nhập tháng: "))
if thang < 1 or thang > 12:
    print("Tháng không hợp lệ!")
elif thang == 1:
    if ngay < 1 or ngay > 31:
        print("Ngày không hợp lệ!")
    elif ngay == 31:
        ngay_tiep_theo = 1
        thang_tiep_theo = 2
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 2:
    if ngay < 1 or ngay > 28:
        print("Ngày không hợp lệ!")
    elif ngay == 28:
        ngay_tiep_theo = 1
        thang_tiep_theo = 3
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 3:
    if ngay < 1 or ngay > 31:
        print("Ngày không hợp lệ!")
    elif ngay == 31:
        ngay_tiep_theo = 1
        thang_tiep_theo = 4
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 4:
    if ngay < 1 or ngay > 30:
        print("Ngày không hợp lệ!")
    elif ngay == 30:
        ngay_tiep_theo = 1
        thang_tiep_theo = 5
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 5:
    if ngay < 1 or ngay > 31:
        print("Ngày không hợp lệ!")
    elif ngay == 31:
        ngay_tiep_theo = 1
        thang_tiep_theo = 6
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 6:
    if ngay < 1 or ngay > 30:
        print("Ngày không hợp lệ!")
    elif ngay == 30:
        ngay_tiep_theo = 1
        thang_tiep_theo = 7
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 7:
    if ngay < 1 or ngay > 31:
        print("Ngày không hợp lệ!")
    elif ngay == 31:
        ngay_tiep_theo = 1
        thang_tiep_theo = 8
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 8:
    if ngay < 1 or ngay > 31:
        print("Ngày không hợp lệ!")
    elif ngay == 31:
        ngay_tiep_theo = 1
        thang_tiep_theo = 9
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 9:
    if ngay < 1 or ngay > 30:
        print("Ngày không hợp lệ!")
    elif ngay == 30:
        ngay_tiep_theo = 1
        thang_tiep_theo = 10
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 10:
    if ngay < 1 or ngay > 31:
        print("Ngày không hợp lệ!")
    elif ngay == 31:
        ngay_tiep_theo = 1
        thang_tiep_theo = 11
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 11:
    if ngay < 1 or ngay > 30:
        print("Ngày không hợp lệ!")
    elif ngay == 30:
        ngay_tiep_theo = 1
        thang_tiep_theo = 12
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
elif thang == 12:
    if ngay < 1 or ngay > 31:
        print("Ngày không hợp lệ!")
    elif ngay == 31:
        ngay_tiep_theo = 1
        thang_tiep_theo = 1
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
    else:
        ngay_tiep_theo = ngay + 1
        thang_tiep_theo = thang
        print(f"Ngày tiếp theo là: {ngay_tiep_theo}/{thang_tiep_theo}")
else:
    print("Tháng không hợp lệ!")
