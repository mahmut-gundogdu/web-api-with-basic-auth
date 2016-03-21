# Asp.net Web Api 2 Basic Auth Örneği
Asp.net web api 2 ile basic auth örneği. 
burada asıl sorunu çözen iki kod mevcut 
1. HttpModule.cs dosyası içindeki   public class BasicAuthHttpModule : IHttpModule bizim oturum açmamızı sağlayan kod parçası.
kullanıcı doğrulamayı da burada yapıyoruz.örnek olduğu için db vs bağlanmıyor
2.     BasicAuthHttpModule modulunun web config üzerinden sisteme tanıtılması.
>     <modules>
>       <add name="BasicAuthHttpModule"
>          type="BasicAuth.BasicAuthHttpModule, BasicAuth"/>
>      </modules>

basic auth ile güven sıkıntınız veya soru işaretlerini varsa bu yazıyı bir okuyun. 
https://www.rdegges.com/2015/why-i-love-basic-auth/
