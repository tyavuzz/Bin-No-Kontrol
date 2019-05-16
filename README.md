# Bin No Kontrol


banka ve Kredi kartlarının ilk 6 hanesi banka ve kartı tanımlayan bin numarasıdır. 

MSSQl fonksiyonunun yaptığı iş ise kendisine yollanan 6 haneli bin numarasının ilgili banka adı ve kart özelliklerini geri yollamaktır. 

DECLARE @cardnum VARCHAR (16)
SET @cardnum='444678**********'
SELECT dbo.BANKAADI(LEFT(@cardnum,6))

şeklinde veri yollanırsa fonksiyondan dönecek veri aşağıdaki gibi olacaktır. 

T.C. ZİRAAT BANKASI A.Ş. VISA PLATINUM

