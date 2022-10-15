# ESP-IDF FreeRTOS API Reference 정리

## EventGroupHandle_t xEventGroupCreate(void)
<b>Header</b> : /freertos/FreeRTOS-Kernel/include/freertos/event_groups.h
<br>
<b>Parameter</b>
<br>
　　void
<br>
<b>Description</b> : 새로운 RTOS 이벤트 그룹 생성. 이벤트 그룹이 필요한 메모리는 함수 내에서 동적으로 할당됨
<br>
<b>Return</b>
<br>
　　EventGroupHandle_t Handle : 이벤트 그룹 핸들러
<br>
　　NULL : Heap 메모리 부족
<br>
<br>
