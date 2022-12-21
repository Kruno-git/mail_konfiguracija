
Prođite kuharicu svakako prije no što kopirate fajlove iz repositorija na svoj mail server, na taj način ćete izbjeći pogreške.
Fajlovi koji se nalaze u repou su konfigurirani za postavke koje su vam potrebne. Jedino što treba promijeniti su stavke koje su ili unutar <> ili na kojima piše npr: KERBEROS.REALM.OVDJE ili neka.domena.ovdje. Pratite statuse journal ili logove kako biste otkrili jeste lli u određenim konfiguracijskim datotekama pogriješili.

Obratite pozornost na MX recorde na ds1 i ns1, DNS mora biti pravilno konfiguriran kako bi mail mogao raditi, isto tako, apsolutno je potrebno napraviti Mail grupu (imenujte ju npr Mail_users jer je "Mail" u sustavu grupa rezervirana riječ) na ds1 serveru i u nju staviti sve korisnike koji su predviđeni za korištenje maila.

Ovaj mail server konfiguriran je isključivo za Informacijski sustav koji se sastoji od Linux mašina, drugim riječima morati ćete promjeniti postavke logina ako nemate AD server, a planirate da ovaj mail server koriste windows računala (login preko password) Ukoliko imate linux based sustav, ovo će ići kao podmazano Thunderbird, novi account, naziv, bez passworda, upišete hostname mail servera i automatski će se pokazati sigurni portovi za imap i smtp.

Što se tice konfiguracijskih fajlova ovdje, korisite ih tako sto cete promijeniti podatke relevantne za uspostavljanje vaseg informacijskog sustava.
U svrhu ocuvanja mentalnog zdravlja, originalni config ostavite sa ekstenzijom .bak .old ili kako hocete, za svaki slucaj, ako se nesto obatali.

Obratite pozornost na kuharice koje ce takodjer biti implementirane u svaki od repoa.
Napravite si sliku informacijskog sustava, tako da uvijek znate gdje ste i sto radite.
