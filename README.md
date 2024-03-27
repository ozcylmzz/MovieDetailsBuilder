# MovieDetailsBuilder
## The project code is private and prepared for job interviews. Please contact yilmaz.ozcn@gmail.com for the project code.

![launchScreenGif](https://github.com/ozcylmzz/OMDBMovieList/assets/34898893/2cda88dc-e0ec-44e0-8268-80c9ec176d8c)
![movieSearchGif](https://github.com/ozcylmzz/OMDBMovieList/assets/34898893/7e0e8e01-791c-43cc-b9e9-10e82c067bfe)
![movieDetailsGif](https://github.com/ozcylmzz/OMDBMovieList/assets/34898893/77305b59-509a-425f-a716-4593861d668b)

## **Kullanılan Kütüphaneler**
### **Alamofire:** HTTP isteklerini yapmak için kullanılmıştır.
### **PopupDialog:** Kullanıcıya bildirimler göstermek için kullanılmıştır.
### **Reachability:** İnternet bağlantısını kontrol etmek için kullanılmıştır.
### **Firebase Analytics & Remote Config:** Firebase Analytics ile kullanıcı etkileşimlerini takip etmek ve Firebase Remote Config ile dinamik olarak uygulama yapılandırmasını güncellemek için kullanılmıştır.

## **Mimariler**
### **MVVM & VIPER:** Proje, MVVM (Model-View-ViewModel) ve VIPER (View-Interactor-Presenter-Entity-Router) mimarilerini bir araya getirir. MVVM ve VIPER klasörleri içinde, bu mimarilere uygun olarak düzenlenmiş classları bulabilirsiniz. Servis yönetimi, view ve extension classları bu iki mimari için ortaklanmıştır.

## **Özellikler**
### **AppDelegate Konfigürasyonları:** Uygulama başlangıcında mimari yapıyı oluşturmak için gerekli ayarlar AppDelegate üzerinde yapılmıştır.
### **LaunchScreen Animasyonu:** Default LaunchScreen yerine bir storyboard kullanılarak, Lottie Animations kütüphanesi ile animasyon eklenmiştir.
### **Firebase Remote Config:** Uygulama başlangıcında Remote Config üzerinden alınan metin, belirli bir süre sonra ana ekrana geçilmeden önce gösterilmektedir.
### **Ana Ekran:** MainViewController açıldığında, öncelikle Empty View görüntülenir. Kullanıcı, IMDB API ile film aramaları yapabilir ve sonuçlar listelenir. Detay ekranı, ilgili film seçildiğinde yüklenir.
### **Kullanıcı Etkileşimleri:** Kullanıcının yaptığı işlemler Firebase Log Event yapısı ile Firebase'e kaydedilir.
### **İnternet Bağlantısı Kontrolü:** Reachability kullanılarak, internet bağlantısının olmadığı durumlarda kullanıcıya uygun bir bildirim gösterilir.
### **API İstekleri:** Generic yapı ve Alamofire kullanılarak API istekleri yapılır. MVVM ve VIPER mimarileri için uygun hale getirilmiş OMDBService class'ı bulunmaktadır.
### **Önbellek Yönetimi:** Cache Manager yapısı eklenmiş, aynı verinin tekrar çekilmesinin önüne geçilmiştir.
### **Görsel İndirme:** URLSession kullanılarak, ilgili film posterleri indirilir.
### **Modelleme:** Kullanılmayan değişkenler için entity oluşturma planı yapılmış, ancak kısıtlı zaman sebebiyle modeller kullanılmıştır.

__________

## **Used Libraries**
### **Alamofire:** Used for making HTTP requests.
### **PopupDialog:** Used to show notifications to the user.
### **Reachability:** Used to check internet connectivity.
### **Firebase Analytics & Remote Config:** Used for tracking user interactions with Firebase Analytics and dynamically updating app configurations with Firebase Remote Config.

## **Architectures**
### **MVVM & VIPER:** The project combines MVVM (Model-View-ViewModel) and VIPER (View-Interactor-Presenter-Entity-Router) architectures. Inside the MVVM and VIPER folders, you can find classes organized according to these architectures. Service management, view, and extension classes are shared between these two architectures.

## **Features**
### **AppDelegate Configurations:** Necessary settings to build the architectural structure are done in the AppDelegate.
### **LaunchScreen Animation:** Instead of the default LaunchScreen, an animation is added using a storyboard and the Lottie Animations library.
### **Firebase Remote Config:** Text fetched from Remote Config at app startup is displayed for a certain period before transitioning to the main screen.
### **Main Screen:** Upon opening the MainViewController, an Empty View is initially displayed. Users can perform movie searches using the IMDB API, and the results are listed. The detail screen loads when a specific movie is selected.
### **User Interactions:** User actions are logged to Firebase using the Firebase Log Event structure.
### **Internet Connection Control:** Reachability is used to show appropriate notifications to the user when there is no internet connection.
### **API Requests:** API requests are made using a generic structure and Alamofire. There is an OMDBService class tailored for MVVM and VIPER architectures.
### **Cache Management:** Cache Manager structure is implemented to prevent redundant data fetching.
### **Image Downloading:** Movie posters are downloaded using URLSession.
### **Modeling:** Plans were made to create entities for unused variables, but models were used due to limited time.
