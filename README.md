# bully-algorithm
Bully algoritması, dağıtık sistemlerde lider seçimi algoritması olarak kullanılır. Dağıtık sistemlerde birden fazla düğüm (node) veya sunucu (server) arasında çalışan uygulamaların etkileşimli çalışması gerektiği durumlarda kullanılır. Örneğin, bir ağda birden fazla sunucu varsa ve bu sunucular arasında bir lider seçilmesi gerekiyorsa, Bully algoritması kullanılabilir.

Bully algoritmasının çalışma şekli şöyledir:

Başlangıçta, tüm düğümler lider adayıdır ve kendi öncelik seviyelerini (ID'lerini) bilirler.
Bir düğüm lider olma konusunda diğer düğümlerle bir yarışa girer. Yarışa başlamadan önce, lider adayı diğer düğümlere lider olmak istediğini belirtir.
Lider adayı, liderliği kazanabilmesi için öncelik seviyesi en yüksek olan düğümle bir bağlantı kurar.
Yüksek öncelikli düğüm, lider adayını tanıyarak liderliği ona devreder.
Lider adayı, liderliği aldığını diğer düğümlere bildirir ve lider olarak görevine başlar.
Bully algoritmasının çalışma zamanı analizi, n düğüm için O(n²) olur. En iyi durumda, lider seçimi tek adımda gerçekleşir ve çalışma zamanı O(1) olur. En kötü durumda, lider seçimi n adımda gerçekleşir ve çalışma zamanı O(n²) olur. Ortalama durumda, lider seçimi n/2 adımda gerçekleşir ve çalışma zamanı O(n²) / 2'dir.

Bully algoritmasının en iyi, en kötü ve ortalama sınırları, lider adaylarının öncelik seviyelerine ve lider seçimindeki yarışın karmaşıklığına bağlı olarak değişir. Bu sınırları bulmak için, lider adayları arasındaki öncelik seviyelerinin dağılımı ve lider seçimindeki yarışların sayısı gibi faktörler dikkate alınır. Bu hesaplamaları yapmak için, genellikle olası senaryoların simülasyonları kullanılır.
