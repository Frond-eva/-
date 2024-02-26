bank_cad=input('Your bankcard number:')
def bank_card(card):
    dec=card.split(' ')
    for i in range (len(dec)):
         del dec[i:3]
        dec.append('----')
    dec.reverse()
    return ' '.join(dec)
            
  def get_bank(card):
    print('You want see to u card?')
    if (w:=input().lower()) == 'yes':
        return(f'{bank_cad[0:4]}-{bank_cad[5:9]}-{bank_cad[10:14]}-{bank_cad[15:19]}')
    else:
        return ('Доступ запрещен')
print(bank_card(bank_cad))    
print(get_bank(bank_cad))  
