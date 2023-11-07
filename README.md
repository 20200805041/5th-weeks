# 5th-weeks
5th weeks

                                                                                    SORU 1
UML nedir?
Birleşik Modelleme Dili (UML), karmaşık yazılım sistemlerinin hem yapısal hem de davranışsal olarak mimarisi, tasarımı ve uygulanması için ortak, anlamsal ve sözdizimsel açıdan zengin bir görsel modelleme dili oluşturmak üzere oluşturulmuştur. UML, üretimdeki süreç akışı gibi yazılım geliştirmenin ötesinde uygulamalara sahiptir.

Diğer alanlarda kullanılan planlara benzer ve farklı diyagram türlerinden oluşur. Toplamda, UML diyagramları sistemin ve içindeki nesnelerin sınırlarını, yapısını ve davranışını tanımlar.

UML bir programlama dili değildir ancak UML diyagramlarını kullanarak çeşitli dillerde kod oluşturmak için kullanılabilecek araçlar vardır. UML'nin nesne yönelimli analiz ve tasarımla doğrudan ilişkisi vardır.

Birleşik Modelleme Dili (UML) standartlaştırılmış bir modelleme dilidir. Yazılım geliştiricilerin yeni yazılım sistemlerini ve planlarını görselleştirmesine, oluşturmasına ve belgelemesine yardımcı olur.

UML, karmaşık sistemlerin oluşturulmasında başarılı olduğu kanıtlanmış çeşitli mühendislik uygulamalarına dayalı statik yapı diyagramları oluşturmak için kullanılır. Yayınlanan standartlar neredeyse 800 sayfa uzunluğundadır.

Tarihsel olarak UML, yazılım sistemlerini modellemek için kullanılmıştır, ancak bu yalnızca yazılım geliştiricilerle sınırlı değildir. Günümüzde süreçleri ve projeleri yönetmek için UML diyagramları da kullanılmaktadır. Bu senaryoda UML diyagramları tüm iş akışlarının ve iş süreçlerinin ana hatlarını çizer.

En sık kullanılan UML diyagramı alt kategorisidir. Tüm nesne yönelimli yazılım sistemlerinin temel taşı, sınıf diyagramıdır. Kullanıcılar, bir sistemin sınıflarına ve özniteliklerine bakarak sistemin statik yapısını görselleştirebilir ve sınıflarının birbiriyle nasıl ilişkili olduğunu belirleyebilir.
                                                                                     
                                                                                    SORU 2
 Arraylist: Yeniden boyutlandırılabilir dizi. Ne kadar veriyle çalışacağınızı bilmiyorsanız, onu Arraylist'e atıp unutabilirsiniz.

Bağlantılı liste: "Düğümlerden" oluşan bir liste; her düğümde istediğiniz her şeyi saklayabilirsiniz, ancak onu bağlantılı liste yapan şey bir sonraki düğüme yönelik bir "işaretçidir". Yani 1 -> 2 -> 3 bağlantılı bir liste için, eğer 1. düğümdeyseniz işaretçi 2'yi içeren düğüme gidecektir.

HashMap: Eşsiz şey çiftlerini anahtar, değer çiftlerinde depolamak istiyorsanız. Her anahtarın benzersiz olması gerekir, ancak değer hemen hemen her şey olabilir. Örneğin, bir kelimedeki harflerin geçişlerini saymak istiyorsanız hashmap kullanabilirsiniz. Bir kelime için "merhaba" 0 -> {"h": 1, "e": 1, "l": 2", "o": 1}.

HashSet: Benzersiz şeyleri takip etmek istiyorsanız. Bir kümede bir şeyden yalnızca bir tanesi bulunabilir.  

                                                                                                                                                                                                                                                                                                              SORU 2
                                                                                    
                                                                                    
public class harfDegistirme {
    public static void main(String[] args) {
        String str = "SeLaM KıZlAr";
        String result = changeCase(str);
        System.out.println(result);
    }

    public static String changeCase(String str) {
        StringBuilder result = new StringBuilder();
        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);
            if (Character.isUpperCase(ch)) {
                result.append(Character.toLowerCase(ch));
            } else {
                result.append(Character.toUpperCase(ch));
            }
        }
        return result.toString();
    }
}                                                                                    


                                                                            SORU 3


import java.util.Scanner;

public class Squeeze {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("İki kelime giriniz: ");
        String word1 = scanner.next();
        String word2 = scanner.next();
        String result = "";
        for (int i = 0; i < word2.length(); i++) {
            char c = word2.charAt(i);
            if (word1.indexOf(c) == -1) {
                result += c;
            }
        }
        System.out.println("Sonuç: " + result);
    }
}                                                                            











