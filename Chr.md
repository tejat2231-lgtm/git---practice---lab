from selenium import webdriver
from selenium.webdriver.common.by import By

driver = webdriver.Edge()

driver.get("https://www.google.com")

# Inspect search box
search_box = driver.find_element(By.NAME, "q")

print("Element found:", search_box)

driver.quit()
