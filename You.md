from selenium import webdriver
from selenium.webdriver.common.by import By
import time

driver = webdriver.Chrome()

driver.get("https://www.youtube.com")
time.sleep(3)

search = driver.find_element(By.NAME, "search_query")
search.send_keys("DevOps tutorial")
search.submit()

time.sleep(5)
driver.quit()
