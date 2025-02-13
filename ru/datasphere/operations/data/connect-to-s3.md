# Подключение к хранилищу S3

Вы можете управлять подключением к объектному хранилищу [S3](../../../glossary/s3.md) в интерфейсе {{ ml-platform-name }} на странице проекта с помощью ресурса **Коннектор S3**.

{% note info %}

Старайтесь не использовать хранилище S3 в режиме [FUSE](https://ru.wikipedia.org/wiki/FUSE_(модуль_ядра)) для работы в бакете с одноуровневыми (нерекурсивными) каталогами с большим количеством файлов. Такой сценарий использования вызывает существенное снижение производительности хранилища.

{% endnote %}

## Создать коннектор S3 {#create}

1. Получите ключ доступа у вашего S3-провайдера. Чтобы сделать это в {{ objstorage-full-name }}:
  1. [Создайте сервисный аккаунт](../../../iam/operations/sa/create.md).
  1. [Назначьте](../../../iam/operations/sa/assign-role-for-sa.md) созданному аккаунту [роль](../../../storage/security/), которая разрешит либо только чтение, либо чтение и запись.
  1. [Создайте ключ доступа](../../../iam/operations/sa/create-access-key.md) для сервисного аккаунта.
1. {% include [find project](../../../_includes/datasphere/ui-find-project.md) %}
1. Если вы создаете подключение к бакету {{ objstorage-name }}, в настройках проекта [укажите](../projects/update.md) сервисный аккаунт, от имени которого {{ ml-platform-name }} будет подключаться к нему.
1. (опционально) В правом верхнем углу нажмите кнопку **Создать ресурс**. Во всплывающем окне выберите **Секрет** и [создайте секрет](secrets.md#create) с секретной частью статического ключа доступа для сервисного аккаунта. Вы также сможете создать секрет при создании подключения S3.
1. В правом верхнем углу нажмите кнопку **Создать ресурс**. Во всплывающем окне выберите **Коннектор S3**.
1. Заполните поля:
   * **Имя** — имя создаваемого коннектора.
   * (Опционально) **Описание** создаваемого коннектора.
   * **Эндпоинт** — хост хранилища. Для {{ objstorage-full-name }} это `https://{{ s3-storage-host }}/`.
   * **Бакет** — имя бакета в хранилище.
     
     {% note warning %}

     Не используйте для подключения бакеты, содержащие точку в имени. [Подробнее о бакетах](../../../storage/concepts/bucket.md).

     {% endnote %}

   * **Имя раздела при подключении** — название тома при монтировании бакета в файловую систему проекта.
   * **Идентификатор статического ключа доступа**, который используется для подключения к хранилищу. 
   * **Статический ключ доступа** — выберите из списка [секрет](../../concepts/secrets.md), содержащий секретную часть статического ключа доступа, или создайте новый секрет.
   * **Режим работы** — режим доступа к объектному хранилищу: **Только чтение** или **Чтение и запись**.
   * **Бэкенд** — режим бэкенда: **По умолчанию**, **GeeseFS** или **s3fs**.
1. Нажмите кнопку **Создать**.

## Подключить хранилище S3 к проекту {#mount}

Перейдите на страницу коннектора S3 и нажмите кнопку **Активировать**. После активации бакет будет доступен в интерфейсе {{ jlab }}Lab в списке на вкладке **S3 Mounts** ![S3 Mounts](../../../_assets/datasphere/bucket.svg), и его можно будет просматривать как файловую систему.

## Использовать хранилище S3 в проекте {#usage}

Вы можете обращаться к файлам в подключенном бакете из кода проекта. Выберите нужный файл в подключенном хранилище S3 во вкладке **S3 Mounts** ![S3 Mounts](../../../_assets/datasphere/bucket.svg), нажмите на него правой кнопкой мыши и выберите **Copy path**. Путь к файлу будет скопирован в буфер обмена. Вставьте скопированный путь в нужное место проекта.

## Отключить хранилище S3 {#unmount}

1. На странице проекта в разделе **Ресурсы** нажмите **Коннектор S3**. 
1. Выберите коннектор и перейдите на страницу ресурса.
1. Нажмите кнопку **Деактивировать** в правом верхнем углу страницы.

Вы сможете повторно подключить хранилище S3 к проекту, когда это будет необходимо.