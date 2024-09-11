@startuml
left to right direction
actor "Клиент" as client
rectangle "Платежная система" as ps
rectangle  Мойка.ру  {
  usecase "Управлять своим профилем" as UC1
  usecase "Управлять списком своих авто" as UC2
  usecase "Выбрать город" as UC3
  usecase "Выбрать мойку" as UC4
  usecase "Выбрать дату + время" as UC5
  usecase "Выбрать услугу" as UC6
  usecase "Выбрать способ оплаты" as UC7
  usecase "Оплачивать услуги" as UC8
  usecase "Отменять услуги" as UC9
  usecase "Обратиться в техподдержку" as UC10
}
client --> UC1
client --> UC2
client --> UC3
client --> UC4
client --> UC5
client --> UC6
client --> UC7
client --> UC8
client --> UC9
client --> UC10
UC7 <-- ps


@enduml

