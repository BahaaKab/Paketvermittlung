# Aufgabe
Um Nachrichten in einem paketvermittelten Rechnernetz (z. B. dem Internet) von einem Sender End-System zu einem Empfänger End-System übertragen zu können, müssen längere Nachrichten in einzelne Datenpakete aufgeteilt werden. Die Datenpakete können anschließend entweder verbindungsorientiert oder verbindungslos vom Sender End-System zum Empfänger End-System übertragen werden.
Ein Datenpaket soll in dieser Aufgabe aus den folgenden Feldern bestehen:<br />
• Version: 4 oder 6 <br />
• Absender: je nach Version IPv4- oder IPv6-Adresse <br />
• Empfänger: je nach Version IPv4- oder IPv6-Adresse <br />
• Paketlaufnummer: Integer > 0 <br />
• Datenteil-Länge: Integer > 0 <br />
• Datenteil: String aus Buchstaben, Zahlen, Sonderzeichen <br />
Ihre Aufgabe besteht nun darin ein Java-Programm zu entwickeln, dass vom Benutzer die Version, den Absender, den Empfänger und eine mehrzeilige Nachricht der Länge N, die mit Zeilenumbruch.Zeilenumbruch (bzw. <CR><LF>.<CR><LF>) abgeschlossen wird, bekommt und die Nachricht in Datenpakete mit Datenteil-Länge P verpackt. Dabei darf jedes Paket ausschließlich ganze Wörter enthalten, eine Trennung in der Wortmitte ist also ausgeschlossen.
Weitere Vorgaben: <br />
• Die maximale Datenteil-Länge P soll als Kommandozeilenargument übergeben werden. <br />
• Die Nachricht enthält keine Leerzeichen am Zeilenanfang und am Zeilenende. <br />
• Keine Anfangs- und Endleerzeichen im Datenteil. <br />
• Leerzeichen haben die Länge 1. <br />
• Zeilenumbrüche sollen mit \n kodiert werden und haben demzufolge die Länge 2. Eine Trennung von \n ist nicht erlaubt. <br />
• Wenn die Nachricht vom Benutzer ein Wort mit Länge W > P enthält, so gibt dass Java-Programm einen entsprechenden Fehler aus. 
**Beispielhafte** Fehlermeldung: Die Nachricht kann nicht versendet werden, da sie ein Wort mit Länge W > P enthält. Dabei W und P mit den eigentlichen Werten ersetzen.
• Wörter mit Bindestrich (z. B. Peer-To-Peer-Modell) oder Schrägstrich (z. B. TCP/IP) dürfen beliebig am Bindestrich/Schrägstrich getrennt und in mehrere Datenpakete aufgeteilt werden. <br />
• Es sind nur Datenpakete mit Version 4 oder 6 erlaubt. Die Eingaben für Absender und Empfänger müssen jedoch nicht auf Korrektheit geprüft werden.
