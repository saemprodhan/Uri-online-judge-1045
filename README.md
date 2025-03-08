# Uri-online-judge-1045
X = list(map(float, input().split()))
A, B, C = sorted(X, reverse=True)

if A >= B + C:
    print("NAO FORMA TRIANGULO") 
else:
    if A**2 == B**2 + C**2:
        print("TRIANGULO RETANGULO")  
    if A**2 > B**2 + C**2:
        print("TRIANGULO OBTUSANGULO") 
    if A**2 < B**2 + C**2:
        print("TRIANGULO ACUTANGULO")  
    if A == B == C:
        print("TRIANGULO EQUILATERO") 
    elif A == B or A == C or B == C:
        print("TRIANGULO ISOSCELES")
