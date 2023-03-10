import selenium
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC
import time


driver = webdriver.Chrome('./chromedriver')
driver.get("https://egzamin-programista.pl/testy-inf04-projektowanie-programowanie-i-testowanie-aplikacji/")
time.sleep(10)
tab = driver.find_elements(By.CLASS_NAME, "rezultatB")
for element in tab:
    driver.execute_script("arguments[0].setAttribute('value', 'Tak jest, Twoja odpowiedź jest poprawna!')", element)
    driver.execute_script("arguments[0].setAttribute('class', 'rezultatY')", element)

print(tab)
input()

