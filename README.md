1. Setup Skeleton
2. Link up files and test them
3. Add dummy data to controller
4. ng-repeat dummy data in the three categories
5. Style
6. Add filter to each employee list
7. Add All Employee filter




## Dummy Data: 

$scope.terminatedEmployees = [{"id":1,"first_name":"Gay","last_name":"Smees","email":"gsmees0@ed.gov","job_title":"Technical Writer","picture":"https://robohash.org/aspernaturquisin.bmp?size=100x100&set=set1","department":"Human Resources","ssn":"151-41-9431"},
{"id":2,"first_name":"Clevie","last_name":"Extall","email":"cextall1@angelfire.com","job_title":"Safety Technician II","picture":"https://robohash.org/utquosat.png?size=100x100&set=set1","department":"Support","ssn":"311-42-4618"},
{"id":3,"first_name":"Fernanda","last_name":"Bonifazio","email":"fbonifazio2@wikipedia.org","job_title":"Sales Representative","picture":"https://robohash.org/totamvelab.png?size=100x100&set=set1","department":"Accounting","ssn":"457-76-0362"},
{"id":4,"first_name":"Gabriel","last_name":"Couroy","email":"gcouroy3@eepurl.com","job_title":"Web Developer I","picture":"https://robohash.org/doloresnobisrem.jpg?size=100x100&set=set1","department":"Support","ssn":"431-28-1152"},
{"id":5,"first_name":"Merlina","last_name":"Gurnee","email":"mgurnee4@usa.gov","job_title":"Administrative Assistant IV","picture":"https://robohash.org/dolorremet.png?size=100x100&set=set1","department":"Legal","ssn":"724-90-4588"}, {"id":6,"first_name":"Neely","last_name":"Moorhouse","email":"nmoorhouse5@alibaba.com","job_title":"Assistant Professor","picture":"https://robohash.org/iddolorumnulla.png?size=100x100&set=set1","department":"Research and Development","ssn":"768-88-1190"},
{"id":7,"first_name":"Lauritz","last_name":"Beaudry","email":"lbeaudry6@mashable.com","job_title":"Account Representative III","picture":"https://robohash.org/etautemet.png?size=100x100&set=set1","department":"Support","ssn":"578-91-6931"},
{"id":8,"first_name":"Codie","last_name":"Maudlin","email":"cmaudlin7@scribd.com","job_title":"Sales Associate","picture":"https://robohash.org/aliquamvoluptatererum.png?size=100x100&set=set1","department":"Human Resources","ssn":"452-67-6610"},
{"id":9,"first_name":"Ray","last_name":"Son","email":"rson8@studiopress.com","job_title":"Electrical Engineer","picture":"https://robohash.org/adipisciveritatisex.jpg?size=100x100&set=set1","department":"Research and Development","ssn":"327-36-4774"},
{"id":10,"first_name":"Hanny","last_name":"Shemelt","email":"hshemelt9@parallels.com","job_title":"Recruiting Manager","picture":"https://robohash.org/officiisvoluptatemneque.bmp?size=100x100&set=set1","department":"Product Management","ssn":"182-50-8400"},
{"id":11,"first_name":"Dario","last_name":"Lebreton","email":"dlebretona@goo.gl","job_title":"Assistant Media Planner","picture":"https://robohash.org/estdoloremdolores.png?size=100x100&set=set1","department":"Accounting","ssn":"764-54-6945"}]


$scope.newEmployees = [{"id":48,"first_name":"Pris","last_name":"Spittle","email":"pspittle1b@tuttocitta.it","job_title":"Quality Control Specialist","picture":"https://robohash.org/delectusetaccusamus.bmp?size=100x100&set=set1","department":"Support","ssn":"508-47-5413"},
{"id":49,"first_name":"Hillard","last_name":"Kitchenman","email":"hkitchenman1c@usgs.gov","job_title":"Design Engineer","picture":"https://robohash.org/optioiureaccusantium.jpg?size=100x100&set=set1","department":"Services","ssn":"878-58-8484"},
{"id":50,"first_name":"Violet","last_name":"Shaxby","email":"vshaxby1d@fastcompany.com","job_title":"General Manager","picture":"https://robohash.org/undeeligendifugiat.bmp?size=100x100&set=set1","department":"Accounting","ssn":"254-99-8362"},{"id":42,"first_name":"Lanita","last_name":"Aronow","email":"laronow15@networksolutions.com","job_title":"VP Product Management","picture":"https://robohash.org/atquerepellendusratione.bmp?size=100x100&set=set1","department":"Sales","ssn":"466-64-9707"},
{"id":43,"first_name":"Barty","last_name":"Catteroll","email":"bcatteroll16@ucoz.com","job_title":"Senior Sales Associate","picture":"https://robohash.org/nesciuntmodiea.jpg?size=100x100&set=set1","department":"Human Resources","ssn":"561-85-4464"},
{"id":44,"first_name":"Joanie","last_name":"Greenan","email":"jgreenan17@oaic.gov.au","job_title":"Help Desk Operator","picture":"https://robohash.org/eaqueconsequaturaliquid.bmp?size=100x100&set=set1","department":"Product Management","ssn":"469-99-4889"},
{"id":45,"first_name":"Kaleb","last_name":"Hurling","email":"khurling18@photobucket.com","job_title":"Accounting Assistant III","picture":"https://robohash.org/inpraesentiumdeserunt.png?size=100x100&set=set1","department":"Research and Development","ssn":"716-28-5916"},
{"id":46,"first_name":"Cristin","last_name":"Heighton","email":"cheighton19@cpanel.net","job_title":"Chief Design Engineer","picture":"https://robohash.org/recusandaeoccaecaticonsequatur.jpg?size=100x100&set=set1","department":"Accounting","ssn":"870-97-0227"},
{"id":47,"first_name":"Marketa","last_name":"Tuxell","email":"mtuxell1a@topsy.com","job_title":"Administrative Assistant IV","picture":"https://robohash.org/optioperferendisrerum.png?size=100x100&set=set1","department":"Services","ssn":"727-43-2415"}]

$scope.employees = [
{"id":12,"first_name":"Layne","last_name":"Yosselevitch","email":"lyosselevitchb@constantcontact.com","job_title":"Staff Scientist","picture":"https://robohash.org/eumsedsapiente.bmp?size=100x100&set=set1","department":"Business Development","ssn":"612-96-2131"},
{"id":13,"first_name":"Rachele","last_name":"Merrall","email":"rmerrallc@time.com","job_title":"Mechanical Systems Engineer","picture":"https://robohash.org/quiesseaccusantium.jpg?size=100x100&set=set1","department":"Sales","ssn":"134-51-8419"},
{"id":14,"first_name":"Gabbie","last_name":"Abbot","email":"gabbotd@admin.ch","job_title":"Help Desk Operator","picture":"https://robohash.org/eumeostempore.png?size=100x100&set=set1","department":"Engineering","ssn":"797-18-8714"},
{"id":15,"first_name":"Deanne","last_name":"MacCahee","email":"dmaccaheee@reuters.com","job_title":"Paralegal","picture":"https://robohash.org/etquaeincidunt.png?size=100x100&set=set1","department":"Product Management","ssn":"671-89-9688"},
{"id":16,"first_name":"Suzette","last_name":"Pea","email":"speaf@wikimedia.org","job_title":"VP Quality Control","picture":"https://robohash.org/officiarerumdolorem.png?size=100x100&set=set1","department":"Training","ssn":"100-86-1794"},
{"id":17,"first_name":"Priscella","last_name":"Izat","email":"pizatg@opera.com","job_title":"Design Engineer","picture":"https://robohash.org/nostrumporrodolor.bmp?size=100x100&set=set1","department":"Engineering","ssn":"887-20-8837"},
{"id":18,"first_name":"Nina","last_name":"Breston","email":"nbrestonh@noaa.gov","job_title":"Computer Systems Analyst III","picture":"https://robohash.org/etnonat.png?size=100x100&set=set1","department":"Legal","ssn":"155-59-5791"},
{"id":19,"first_name":"Milton","last_name":"Kayser","email":"mkayseri@ovh.net","job_title":"Senior Developer","picture":"https://robohash.org/perspiciatisutut.png?size=100x100&set=set1","department":"Product Management","ssn":"379-15-7382"},
{"id":20,"first_name":"Wallis","last_name":"Imbrey","email":"wimbreyj@ucoz.com","job_title":"Payment Adjustment Coordinator","picture":"https://robohash.org/ipsamquamaut.jpg?size=100x100&set=set1","department":"Research and Development","ssn":"640-45-6076"},
{"id":21,"first_name":"Kassi","last_name":"Abbie","email":"kabbiek@rakuten.co.jp","job_title":"Research Associate","picture":"https://robohash.org/etaspernaturnesciunt.jpg?size=100x100&set=set1","department":"Legal","ssn":"206-90-1346"},
{"id":22,"first_name":"Glen","last_name":"Bunclark","email":"gbunclarkl@nydailynews.com","job_title":"Financial Analyst","picture":"https://robohash.org/remitaquerecusandae.jpg?size=100x100&set=set1","department":"Support","ssn":"718-43-8577"},
{"id":23,"first_name":"Dorris","last_name":"Linnett","email":"dlinnettm@ning.com","job_title":"Recruiting Manager","picture":"https://robohash.org/veroomnisimpedit.png?size=100x100&set=set1","department":"Engineering","ssn":"846-63-4095"},
{"id":24,"first_name":"Fielding","last_name":"Cypler","email":"fcyplern@nydailynews.com","job_title":"VP Accounting","picture":"https://robohash.org/nequerepellendusrerum.jpg?size=100x100&set=set1","department":"Business Development","ssn":"639-21-9631"},
{"id":25,"first_name":"Ardyth","last_name":"Pilbury","email":"apilburyo@tamu.edu","job_title":"Software Test Engineer IV","picture":"https://robohash.org/quoveleius.bmp?size=100x100&set=set1","department":"Support","ssn":"319-94-2360"},
{"id":26,"first_name":"Trixie","last_name":"Ferry","email":"tferryp@google.nl","job_title":"Software Test Engineer I","picture":"https://robohash.org/molestiaeetmolestiae.jpg?size=100x100&set=set1","department":"Sales","ssn":"641-21-6205"},
{"id":27,"first_name":"Vernor","last_name":"Marrian","email":"vmarrianq@stumbleupon.com","job_title":"Media Manager IV","picture":"https://robohash.org/sedestblanditiis.png?size=100x100&set=set1","department":"Business Development","ssn":"349-99-4904"},
{"id":28,"first_name":"Aluin","last_name":"Pengilley","email":"apengilleyr@i2i.jp","job_title":"Web Designer I","picture":"https://robohash.org/etquisconsectetur.bmp?size=100x100&set=set1","department":"Accounting","ssn":"847-20-1861"},
{"id":29,"first_name":"Josefa","last_name":"Peerless","email":"jpeerlesss@shinystat.com","job_title":"Food Chemist","picture":"https://robohash.org/aliquamporrolaborum.png?size=100x100&set=set1","department":"Sales","ssn":"120-17-0629"},
{"id":30,"first_name":"Woody","last_name":"Woodcraft","email":"wwoodcraftt@imageshack.us","job_title":"Social Worker","picture":"https://robohash.org/facilisexpeditaeius.png?size=100x100&set=set1","department":"Support","ssn":"693-43-1745"},
{"id":31,"first_name":"Elisabet","last_name":"Kinnock","email":"ekinnocku@un.org","job_title":"Compensation Analyst","picture":"https://robohash.org/autrepellenduserror.png?size=100x100&set=set1","department":"Sales","ssn":"521-07-2514"},
{"id":32,"first_name":"Jasmin","last_name":"Aleshkov","email":"jaleshkovv@umich.edu","job_title":"Environmental Tech","picture":"https://robohash.org/eiusharummollitia.bmp?size=100x100&set=set1","department":"Accounting","ssn":"617-99-6321"},
{"id":33,"first_name":"Lizzie","last_name":"Kraut","email":"lkrautw@icq.com","job_title":"Geologist I","picture":"https://robohash.org/quoetfacilis.bmp?size=100x100&set=set1","department":"Human Resources","ssn":"124-01-8178"},
{"id":34,"first_name":"Zea","last_name":"Jarville","email":"zjarvillex@themeforest.net","job_title":"Financial Analyst","picture":"https://robohash.org/itaqueexcepturiqui.jpg?size=100x100&set=set1","department":"Business Development","ssn":"532-42-0083"},
{"id":35,"first_name":"Ethyl","last_name":"Bande","email":"ebandey@mashable.com","job_title":"Internal Auditor","picture":"https://robohash.org/culpaexpeditaitaque.jpg?size=100x100&set=set1","department":"Support","ssn":"277-52-5062"},
{"id":36,"first_name":"Elnora","last_name":"Welton","email":"eweltonz@harvard.edu","job_title":"General Manager","picture":"https://robohash.org/omnisquialaudantium.jpg?size=100x100&set=set1","department":"Product Management","ssn":"828-94-7188"},
{"id":37,"first_name":"Seka","last_name":"Jannex","email":"sjannex10@flickr.com","job_title":"Nurse Practicioner","picture":"https://robohash.org/quiareiciendisofficiis.bmp?size=100x100&set=set1","department":"Marketing","ssn":"632-36-7163"},
{"id":38,"first_name":"Shepperd","last_name":"Filpi","email":"sfilpi11@tripadvisor.com","job_title":"Executive Secretary","picture":"https://robohash.org/sintaliasenim.bmp?size=100x100&set=set1","department":"Services","ssn":"172-38-7909"},
{"id":39,"first_name":"Rosella","last_name":"Sealeaf","email":"rsealeaf12@smh.com.au","job_title":"Human Resources Assistant IV","picture":"https://robohash.org/molestiaenonsapiente.bmp?size=100x100&set=set1","department":"Research and Development","ssn":"874-40-7505"},
{"id":40,"first_name":"Nap","last_name":"Sends","email":"nsends13@go.com","job_title":"Teacher","picture":"https://robohash.org/omnisconsequaturlaudantium.bmp?size=100x100&set=set1","department":"Research and Development","ssn":"599-20-9294"},
{"id":41,"first_name":"Sallyann","last_name":"Schirach","email":"sschirach14@infoseek.co.jp","job_title":"Computer Systems Analyst I","picture":"https://robohash.org/doloremrerumvel.bmp?size=100x100&set=set1","department":"Research and Development","ssn":"164-74-9208"}]
