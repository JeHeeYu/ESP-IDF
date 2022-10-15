# ESP-IDF WIFI Reference 정리

## esp_err_t esp_wifi_init(const wifi_init_config_t *config)
<b>Header</b> : components/esp_wifi/include/esp_wifi.h
<br>
<b>Parameter</b>
<br>
　　config : WiFi 초기화 구성 정보를 담고있는 wifi_init_config_t 포인터 변수
<br>
<b>Description</b> : WiFi 드라이버에 대한 리소스를 할당하는 함수로 다른 WiFI API가 호출되기 전에 가장 먼저 호출되어야 한다.
<br>
　　　　　　함수 호출 전 WIFI_INIT_CONFIG_DEFAULT 매크로 함수를 호출해서 구성값을 초기화 해야 한다.
<br>
<b>Return</b>
<br>
　　ESP_OK : WiFi Intialize 성공
<br>
　　ESP_ERR_NO_MEM : 메모리 부족
<br>
　　Other : esp_err.h Error Code 참조
<br>
<br>

## esp_err_t esp_wifi_set_mode(wifi_mode_t mode)
<b>Header</b> : components/esp_wifi/include/esp_wifi.h
<br>
<b>Parameter</b>
<br>
　　mode : WiFi가 작동할 모드
<br>
<b>Description</b> : Station Mode, AP Mode, Station + AP Mode로 설정할 수 있으며 Default 값은 Station Mode로 설정
<br>
<b>Return</b>
<br>
　　ESP_OK : 모드 설정 성공
<br>
　　ESP_ERR_WIFI_NOT_INIT : esp_wifi_init 함수에 의해 WiFi 초기화가 되지 않았음
<br>
　　ESP_ERR_INVALID_ARG : 잘못된 인자
<br>
　　Other : esp_err.h Error Code 참조
<br>
<br>
<br>
<br>

## esp_err_t esp_wifi_set_mode(wifi_mode_t mode)
<b>Header</b> : components/esp_wifi/include/esp_wifi.h
<br>
<b>Parameter</b>
<br>
　　mode : WiFi가 작동할 모드
<br>
<b>Description</b> : Station Mode, AP Mode, Station + AP Mode로 설정할 수 있으며 Default 값은 Station Mode로 설정
<br>
<b>Return</b>
<br>
　　ESP_OK : 모드 설정 성공
<br>
　　ESP_ERR_WIFI_NOT_INIT : esp_wifi_init 함수에 의해 WiFi 초기화가 되지 않았음
<br>
　　ESP_ERR_INVALID_ARG : 잘못된 인자
<br>
　　Other : esp_err.h Error Code 참조
<br>
<br>
