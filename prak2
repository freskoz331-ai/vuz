#1
# #символы - a, b, c, d, e, значит минимальная длина кодового слова - 3
# code = {'a': '000', 'b': '001', 'c': '010', 'd': '011', 'e': '100'}
# message = "abcdeaabd"
# encode = ''.join(code[x] for x in message)
# print(encode)#кодированное соо
# print(len(encode))#обьем
# # 000001010011100000000001011
# # 27

#2
# code = {'a': '00', 'b': '01', 'd': '11', 'e': '100', 'c': '101'}
# message = "abcdeaabd"
# encode = ''.join(code[x] for x in message)
# print(encode)#кодированное соо
# print(len(encode)/len(message))#средняя длина
# # 00011011110000000111
# # 2.2222222222222223

#3
# message = "abcdeaabd"
# #через утф:
# # encode = message.encode('utf8')
# # bn = ''.join([format(x, '08b') for x in encode])
# # v = len(encode)
# # print(bn)
# # print(v*8)
# # # 011000010110001001100011011001000110010101100001011000010110001001100100
# # # 72
# #сами
# code = {'a': '00000000', 'b': '00000001', 'd': '00000011', 'e': '00000100', 'c': '00000101'}
# encode = ''.join(code[x] for x in message)
# print(encode)
# print(len(encode))
# # 000000000000000100000101000000110000010000000000000000000000000100000011
# # 72

#4
code = {'a': '000', 'b': '001', 'c': '010', 'd': '011', 'e': '100'}
message = '000001010011100000000001011'
decode = ''
for i in range(0, len(message), 3):#перебираем полученное сообщение деля его по 3
    pol = message[i:i+3]#берем промежуток равный 3 тк код фиксированный
    for buk in code:#смотрим есть ли такой набор в алфавите
        if code[buk] == pol:
            decode += buk#если есть то добавляем к расшифрованному сообщению
print(decode)

