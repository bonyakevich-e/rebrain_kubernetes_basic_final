### :trophy: Final task of course Kubernetes Basic by Rebrain

#### :scroll: ЗАДАНИЕ: 
Развернуть в Kubernetes приложение Librespeed (https://github.com/librespeed/speedtest)

Ситуация типичная: Вам дали репозиторий, который нужно задеплоить в кубер. Информации ноль, позвонить и узнать, как работает приложение некому (если автор не вкоммитил свой номер телефона где-то в репозитории).
Требуется итоговый набор манифестов, чтобы кто-то сделал `kubectl apply -f .` и приложение заработало.

#### :pencil2: ОПИСАНИЕ ВЫПОЛНЕНИЯ:
В данном репозитории три манифеста:
- `local-path-storage.yaml` - поднимает local-path-provisioner (https://github.com/rancher/local-path-provisioner)
- `mysql.yaml` - поднимает СУБД Mysql в отдельном namespace
- `librespeed.yaml` - поднимает приложение Librespeed в режиме frontend
  
Для развёртывания приложения копируем репозиторий и выполняем:
```
kubectl apply -f .
```
#### :camera: СКРИНЫ ВЫПОЛНЕННОГО ЗАДАНИЯ:
![скриншот приложения](https://github.com/user-attachments/assets/4aad0c08-6d70-466f-b244-d3af5c0562d8)
![kubectl get](https://github.com/user-attachments/assets/80594943-b1d0-4f08-b33f-f17eb537d8b2)
![субд](https://github.com/user-attachments/assets/e47dd8b0-4792-4a88-818a-0660708a8f4e)

:white_check_mark: :date: 2025
