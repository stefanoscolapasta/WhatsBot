from selenium import webdriver
from selenium.webdriver.common.keys import Keys
nome = input('Nome gruppo/utente: ')
messaggio = input('Messaggio da inviare: ')
count = int(input('Numero di volte che vuoi inviare il messaggio: '))

browser = webdriver.Chrome('C:\\Python\\chromedriver')
browser.get('https://web.whatsapp.com/')
browser.implicitly_wait(50)
user_group = browser.find_element_by_xpath('//span[@title = "{}"]'.format(nome))
browser.implicitly_wait(5)
user_group.click()
msg_box = browser.find_element_by_class_name('_13mgZ')
browser.implicitly_wait(5)
for i in range(count):
    msg_box.click()
    browser.implicitly_wait(5)
    msg_box.send_keys(messaggio)
    send_button = browser.find_element_by_class_name('_3M-N-')
    browser.implicitly_wait(5)
    send_button.click()

