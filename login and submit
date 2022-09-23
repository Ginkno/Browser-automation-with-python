from selenium import webdriver
from selenium.webdriver.firefox.service import Service as FirefoxService
from webdriver_manager.firefox import GeckoDriverManager
from selenium.webdriver.common.by import By
from selenium.webdriver.support import expected_conditions
from selenium.webdriver.support.ui import WebDriverWait
from selenium.common.exceptions import NoSuchElementException
from selenium.common.exceptions import StaleElementReferenceException
from selenium.common.exceptions import TimeoutException
from selenium.webdriver.common.keys import Keys


''' 
Here were used selenium webdriver packages to manage error outputs and 
default key inputs.
inputs and outputs hidden.
If you use this code for similar purposes, replace the 'xxxxx' with your info.

'''

driver = webdriver.Firefox(service=FirefoxService(GeckoDriverManager().install()))
driver.get('https://xxxxx.com')
driver.implicitly_wait(3)
login_ = driver.find_element(By.LINK_TEXT, "Login")
driver.implicitly_wait(3)
login_.click()
Usuario = driver.find_element(By.NAME, 'login')
Usuario.send_keys('xxxxxxx')
driver.implicitly_wait(3)
Senha = driver.find_element(By.NAME, 'senha')
Senha.send_keys('xxxxxxx')
driver.implicitly_wait(4)
Entrada = driver.find_element(By.XPATH, '//input[@type=\"submit\"]')
Entrada.click()
driver.implicitly_wait(5)
driver.switch_to.new_window()
driver.get('https://www.xxxxxx.com')
driver.implicitly_wait(3)
Us_Gmail = driver.find_element(By.ID, 'identifierId')
Us_Gmail.send_keys('xxxxxxxxxx')

'''
# driver.switch_to.window(driver.window_handles[0])
# driver.switch_to.window(driver.window_handles[1])
# driver.switch_to.window(driver.window_handles[0])
# driver.switch_to.window(driver.window_handles[1])

Here some tests on handling new open tabs – with .switch_to.new_window() command. As seen, it's possible to change between tabs with handles command, which are managed through an array.
'''


ignored_exceptions = (NoSuchElementException, StaleElementReferenceException, TimeoutException)
