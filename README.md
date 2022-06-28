#giải phương trình bậc 2 có dạng ax^2 + b x + c = 0

print("Giải phương trình bậc 2: ax^2 + bx + c = 0")
a = float(input("Nhập a: "))
b = float(input("Nhập b: "))
c = float(input("Nhập c: "))
import math
if a == 0:
    if b == 0:
        if c == 0:
            print("Phương trình vô số nghiệm!")
        else:
            print("Phương trình vô nghiệm!")
    else:
        if c == 0:
            print("Phương trình có 1 nghiệm x = 0")
        else:
            print("Phương trình có 1 nghiệm x = ", -c / b)
else:
    delta = b ** 2 - 4 * a * c

    if delta < 0:
        print("Phương trình vô nghiệm!")
    elif delta == 0:
        print("Phương trình có 1 nghiệm x = ", -b / (2 * a))
    else:
        print("Phương trình có 2 nghiệm phân biệt!")
        print("x1 = ", ((-b - math.sqrt(delta)) / (2 * a)))
        print("x2 = ", ((-b + math.sqrt(delta)) / (2 * a)))
print("tổng của 2 nghiệm=",(-b/(2*a)))
print("hiệu của 2 nghiệm=",(-c/(2*a)))   
