

Наша команда в течении 6 лет разрабатывает облачную медицинскую информационную систему
для соединенных штатов.

Сегодня я хотел рассказать о молодом, но многообещающем стандарте fhir.

Но вначале немного предистории.

Мы все с вами понимаем, что данные которые собирает и хранит система не принадлежат самой 
системе, а в рамках парадигмы patient-centric медицины, являются собственностью самого пациента.
Поэтому практически не избежно наши системы должны будут отдавать эти данные (другим системам или пациенту)
и принимать их. Важным аспектом передачи медицинской информации является то, что принимающая сторона
должна правильно их интерпретировать, те понять. Для этого наши системы должны говорить на одном общепонятном
языке.

Именно этими проблемами занимается международная организация HL7, которая разрабатывает стандарты для обмена
данными.


Исторически первым организацией HL7 был разработан стандарт обмена сообщениями - HL7 v2.
Это простой и практичный стандарт, который получил широкое распространение. Сейчас значительная 
часть систем, таких как лабораторные приборы и системы, фармакологические, административные и т.д, 
умеет говорить на языке HL7 v2.


Однако этот стандарт обладает рядом серьезных недостатков:

* в основе стандарта лежит жесткая и неявная модель сообщений и сегментов
* в стандарте предусмотрен лишь наивный способ расширения в виде сегментов общего назначения и каждая реализация использует их по разному
* с другой стороны стандарт не предусматривает штатного способа наложения более жестких ограничений на содержимое сообщений, что достаточно часто необходимо.

Из нашего опыта: мы много интегрировались с различными лабораторными, фармацевтическими и другими системами
и можем подтвердить, что эти проблемы реальны. 

Реализовав одну интеграцию, нам практически с нуля приходилось настраивать следующую. Постоянную и жгучую боль
вызывала агрегация данных из разных источников.

По этим причинам организация HL7 решила отправить стандарт версии 2 на поддержку и принятся за разработку стандарта нового поколеления, который как не удивительно был назван HL7 v3. Это было более 10 лет назад. Стандарт был призван учесть недостатки предыдущей версии. Для его разработки был даже стандартизован сам процесс разработки. Сам стандарт
из себя представляет целый пакет самостоятельных стандартов и рекомендаций, таких как референсная информационная модель, модели различных предметных областей, модели сообщений для этих предметных областей. 

Но к сожалению следует констатировать, что за эти 10 лет стандарт не достиг поставленной перед ним цели и не достиг планируемого распространения. Он оказался сложным и медленным в разработке. Можно сказать, что перемудрили.
Самой важной ошибкой было то, что стандарт практически не учитывал его реализуемость.

С этим столкнулись и мы, учавствовуюя в программе Abama Care и сертифицирую нашу систему. Одним из тербований сертификации была реализация импорта и экспорта саммари медицинской истории в формате CCD, который основан на стандартах HL7 v3 и стандарте CDA (архитектура клинических документов).  

