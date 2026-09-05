# NorthStarOps'a Katkı Sağlama

Bu repository kontrollü bir contribution süreci kullanır.

## Katkı Akışı

1. Yalnızca `Available` durumundaki Issue'lar claim edilebilir.

2. Bir Issue'yu claim etmek için Issue üzerine şu yorumu yaz:

   `/claim`

3. Bir contributor aynı anda yalnızca bir aktif claimed Issue üzerinde çalışabilir.

4. Bir Issue claim edildikten sonra 24 saat içinde o Issue'ya bağlı bir Draft Pull Request açılmalıdır.

5. 24 saat içinde uygun bir Draft Pull Request açılmazsa claim kaldırılabilir ve Issue tekrar `Available` durumuna döner.

6. Development, contributor'ın kendi fork'unda oluşturduğu bir branch üzerinde yapılmalıdır.

7. Branch isminde ilgili Issue numarası bulunmalıdır.

   Örnek:

   `feature/12-orders-readiness`

8. Pull Request, upstream repository'deki `main` branch'i hedeflemelidir.

9. Pull Request açıklamasında yalnızca bir Issue aşağıdaki formatla bağlanmalıdır:

   `Closes #<issue-number>`

10. Bir Issue için yalnızca tek accepted active contribution kabul edilir.

11. Review sonucunda değişiklik istenirse aynı branch ve aynı Pull Request üzerinde çalışmaya devam edilmelidir.

12. Review revision için yeni bir Pull Request açılmamalıdır.

13. Contributor upstream `main` branch'e doğrudan push yapmamalıdır.

## AI Kullanımı

Development sırasında AI araçlarının kullanımı serbesttir.

Ancak contributor aşağıdaki konulardan sorumludur:

- istenen davranışı anlamak,
- üretilen kodu doğrulamak,
- Allowed Scope sınırları içinde kalmak,
- implementation'ı test etmek,
- teknik kararlarını açıklayabilmek,
- engineering review feedback'lerine cevap vermek.

## Review

Bir Pull Request, ilgili Issue kontratına göre değerlendirilir.

Review sırasında özellikle şu alanlar dikkate alınır:

- Expected Behaviour,
- Acceptance Criteria,
- Allowed Scope,
- Do Not Change sınırları,
- testler,
- code quality,
- implementation risk.

Kodun build olması ya da AI tarafından üretilmiş olması approval için tek başına yeterli değildir.

Pull Request, merge edilmeden önce Issue kontratını ve engineering review gereksinimlerini karşılamalıdır.
