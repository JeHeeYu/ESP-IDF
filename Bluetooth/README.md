# ESP-IDF Bluetooth Reference 정리

## esp_err_t esp_bt_controller_init(esp_bt_controller_config_t *cfg)
<b>Header</b> : components/bt/include/esp32/include/esp_bt.h
<br>
<b>Parameter</b>
<br>
　　cfg : BT 컨트롤러의 초기 구성
<br>
<b>Description</b> : 태스크 및 기타 리소스를 할당하기 위해 BT 컨트롤러를 초기화하는 함수이다.
<br>
　　　　　　다른 BT 함수가 호출되기 전 호출되어야 하며, 한 번만 호출되어야 한다. 
      <br>
　　　　　　BT_CONTROLLER_INIT_CONFIG_DEFAULT 매크로 함수로 BT 컨트롤러의 Default 값을 매개변수로 전달한다.
<br>
<b>Return</b>
<br>
　　ESP_OK : 성공
<br>
　　Other : 실패
<br>
<br>

## esp_err_t esp_bt_controller_enable(esp_bt_mode_t mode)
<b>Header</b> : components/bt/include/esp32/include/esp_bt.h
<br>
<b>Parameter</b>
<br>
　　mode : BT활성화 모드(BLE/BT/BTDM)으로, esp_bt_controller_Init()의 cfg 매개변수의 모드와 같아야 함
<br>
<b>Description</b> : BT 기능을 활성화하는 함수이다.
<br>
　　　　　　다른 모드로 변경 시에는 esp_bt_controller_disable() 호출 후 다시 enable 함수를 호출하여야 한다.
<br>
<b>Return</b>
<br>
　　ESP_OK : 성공
<br>
　　Other : 실패
<br>
<br>

## esp_err_t esp_bluedroid_init(void)
<b>Header</b> : components/bt/include/esp32/include/esp_bt.h
<br>
<b>Parameter</b>
<br>
　　void
<br>
<b>Description</b> : 블루투스 사용하기 전 블루투스 초기화 함수이다.
<br>
　　　　　　함수 호출 후 esp_bluedroid_enable() 함수를 호출하여 블루투스를 활성화 할 수 있다.
<br>
<b>Return</b>
<br>
　　ESP_OK : 성공
<br>
　　Other : 실패
<br>
<br>

## esp_err_t esp_bluedroid_enable(void)
<b>Header</b> : components/bt/include/esp32/include/esp_bt.h
<br>
<b>Parameter</b>
<br>
　　void
<br>
<b>Description</b> : 블루투스를 사용할 수 있도록 활성화하는 함수이다.
<br>
　　　　　　함수 호출 전 esp_bluedroid_init() 함수를 먼저 호출해야 한다.
<br>
<b>Return</b>
<br>
　　ESP_OK : 성공
<br>
　　Other : 실패
<br>
<br>

## esp_err_t esp_ble_gatts_register_callback(esp_gatts_cb_t callback)
<b>Header</b> : components/bt/include/esp32/include/esp_bt.h
<br>
<b>Parameter</b>
<br>
　　callback : 실행할 콜백 함수
<br>
<b>Description</b> : GATT 이벤트를 처리하는 핸들러를 등록하는 함수이다.
<br>
<b>Return</b>
<br>
　　ESP_OK : 성공
<br>
　　Other : 실패
<br>
<br>

## esp_err_t esp_ble_gap_register_callback(esp_gap_cb_t callback)
<b>Header</b> : components/bt/include/esp32/include/esp_bt.h
<br>
<b>Parameter</b>
<br>
　　callback : 실행할 콜백 함수
<br>
<b>Description</b> : GAP 이벤트를 처리하는 핸들러를 등록하는 함수이다.
<br>
<b>Return</b>
<br>
　　ESP_OK : 성공
<br>
　　Other : 실패
<br>
<br>
