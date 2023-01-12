# 2022_2023-introduction_to_distributed_technologies-k4112c-buchenkov_e_e

EXAM
--
Q3) Kubernetes — это портативная расширяемая платформа с открытым исходным кодом для управления контейнеризованными рабочими нагрузками и сервисами, которая облегчает как декларативную настройку, так и автоматизацию.
При развёртывании Kubernetes вы имеете дело с кластером.

Кластер Kubernetes cluster состоит из набор машин, так называемые узлы, которые запускают контейнеризированные приложения. Кластер имеет как минимум один рабочий узел.
В рабочих узлах размещены поды, являющиеся компонентами приложения. Плоскость управления управляет рабочими узлами и подами в кластере. В промышленных средах плоскость управления обычно запускается на нескольких компьютерах, а кластер, как правило, развёртывается на нескольких узлах, гарантируя отказоустойчивость и высокую надёжность.
Компоненты панели управления отвечают за основные операции кластера (например, планирование), а также обрабатывают события кластера (например, запускают новый под, когда поле replicas развертывания не соответствует требуемому количеству реплик).

Компоненты панели управления могут быть запущены на любой машине в кластере. Однако для простоты сценарии настройки обычно запускают все компоненты панели управления на одном компьютере и в то же время не позволяют запускать пользовательские контейнеры на этом компьютере

![image](https://user-images.githubusercontent.com/43411372/212014465-198bf1e7-e7cd-4507-8d73-5f58f6c6a750.png)

Работающий кластер Kubernetes включает в себя агента, запущенного на нодах (kubelet) и компоненты мастера (APIs, scheduler, etc), поверх решения с распределённым хранилищем. Приведённая схема показывает желаемое, в конечном итоге, состояние, хотя все ещё ведётся работа над некоторыми вещами, например: как сделать так, чтобы kubelet (все компоненты, на самом деле) самостоятельно запускался в контейнере, что сделает планировщик на 100% подключаемым.

--

Q17) Блокчейн — это перечень записей данных, которые работают как децентрализованный цифровой реестр. Данные хранятся в блоках в хронологическом порядке и защищены с помощью криптографии. 

Майнинг – это процесс, при котором транзакции с криптовалютами между пользователями проверяются и добавляются в блокчейн. Майнинг также отвечает за добавление новых монет в существующее обращение.

В контексте криптовалют блокчейн состоит из стабильной цепочки блоков, каждый из которых содержит перечень ранее подтвержденных транзакций. Поскольку сеть блокчейна поддерживается множеством компьютеров по всему миру, она функционирует как децентрализованная база данных, или реестр. Это означает, что каждый участник (нода) хранит у себя копию данных блокчейна и взаимодействует с другими нодами, чтобы подтвердить совпадение информации в блоках.
Таким образом, транзакции блокчейна происходят в глобальной одноранговой сети, и именно это делает Биткоин децентрализованной цифровой валютой, не имеющей ограничений и устойчивой к цензуре. Кроме того, большинство систем блокчейна не требуют доверия и не контролируются единым органом управления.
В основе почти каждого блокчейна лежит процесс майнинга, основанный на алгоритмах хеширования. Биткоин использует алгоритм SHA-256 (алгоритм безопасного хеширования 256 бит). Он принимает вход произвольной длины и генерирует выход с фиксированной длиной. Выходные данные называются хешем и, в этом случае, всегда состоят из 64 символов (256 бит).

Характеристики:

Неизменность данных: это самая важная функция, поскольку она гарантирует, что данные не будут повреждены. Как это работает - каждый узел в системе имеет копию главного блока. Таким образом, чтобы изменить какие-либо данные, должно быть изменение каждого узла. Это делает блокчейн безопасным и прозрачным.

Децентрализованность: Блокчейн децентрализован, что означает, что никакая власть или правительство, группа лиц или отдельный человек не контролирует эту технологию. Скорее, это группа узлов, которые управляют всей транзакцией.

Единый источник правды: В блокчейне есть только один источник правды - распределенный реестр. Итак, чтобы узнать, кому что принадлежит, или изучить конкретную транзакцию, вам нужно всего лишь зайти в одно место.

Прозрачность или происхождение: каждая транзакция, будь то материальная или нематериальная, может быть прослежена от начала до конца с помощью блокчейна.

Алгоритм консенсуса: чтобы транзакция была принята и записана в блокчейне, все участники или узлы должны согласиться следовать одним и тем же правилам.

Анонимность: Это правда, что каждая транзакция прозрачна и открыта для общественности, но реальные лица остаются анонимными через адреса. Например, предположим, что человек отправляет денежную сумму, получатель будет знать, что отправитель связан с биткойн-адресом, но он не будет знать фактического адреса. Для этого есть несколько причин – одна из них - конфиденциальность.