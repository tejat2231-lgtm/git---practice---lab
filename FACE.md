from selenium import webdriver
from selenium.webdriver.edge.service import Service
import time

# Edge driver path
service = Service(r"C:\Users\TEMP.MITS.046\Desktop\msedgedriver.exe")

# Browser open
driver = webdriver.Edge(service=service)

# Facebook open
driver.get("https://www.facebook.com")

# 5 seconds wait
time.sleep(5)

# Browser close
driver.quit()
