set(COMPONENT_SRCS
    "app_main.c"
    "app_settings.c"
    "app_illuminator.c"
    "app_camera.c"
    "app_wifi.c"
    "app_fonts.c"
    "app_camera_httpd.c"
    "app_lcd.c"
    "app_sntp.c"
    "app_weather.c"
    "app_mqtt_baidubce.c"
    "app_mqtt_aliyun"
    "app_epd3in9.c"
    "app_sht11.c"
)

set(COMPONENT_ADD_INCLUDEDIRS "include" "fonts")

set(COMPONENT_REQUIRES
    esp32-camera
    esp-idf-ssd1306
    mdns
    nvs_flash
    esp_http_server
    weather_seniverse
    mqtt
    app-aliyun
    epd3in9
    esp-sht11
)

set(COMPONENT_EMBED_FILES
    "www/index.html.gz"
    "www/style.css.gz"
    "www/script.js.gz"
    "iot_eclipse_org.pem"
)

register_component()
