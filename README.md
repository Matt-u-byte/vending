#vending
print("Vending Machine\n---------------")

def vending_coinage():
    while(True):
        amount_due = 50
        try:
            vending_coin = int(input("Insert Coin:"))
            if vending_coin == 10:
                amount_due -= 10
            elif vending_coin == 1:
                amount_due -= 1
            elif vending_coin == 5:
                amount_due -= 5
            elif vending_coin == 25:
                amount_due -= 25
                continue
            else:
                break
        except:
            continue
    return amount_due
