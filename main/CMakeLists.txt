set(srcs "main.c"
         "gatt_svr.c")

idf_component_register(SRCS "${srcs}"
                       INCLUDE_DIRS "."
                       PRIV_REQUIRES driver nvs_flash bt esp_adc)
