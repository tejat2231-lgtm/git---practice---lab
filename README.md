from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.edge.service import Service
import time

service = Service("C:\\msedgedriver.exe")
driver = webdriver.Edge(service=service)

driver.get("https://www.google.com")
time.sleep(2)

search_box = driver.find_element(By.NAME, "q")
print("Search box found:", search_box)

driver.quit()
