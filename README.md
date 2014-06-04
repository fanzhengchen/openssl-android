OpenSSL FIPS library for Android  
================================  
Ubuntu11.10(64bit)上で以下の環境をAndroid用にビルドした結果。  

+ openssl-1.0.1g
+ openssl-fips-2.0.5

ビルド準備
-----------------
### NDK  
$HOMEにandroid-ndk-r9d-linux-x86\_64.tar.bz2を解凍。  

### ビルド対象  
$HOMEにこのリポジトリをクローンする。  

### setenv-android.sh  
以下のように変更。  

+ \_ANDROID\_NDK="android-ndk-r9d"  
+ \_ANDROID\_EABI="arm-linux-androideabi-4.6"  
+ \_ANDROID\_API="android-17"  

ビルド方法  
----------
『OpenSSL FIPS Library and Android Guide.pdf』を参照。 
ドキュメント内のコマンドはandroid-14を前提にしているのでandroid-17に置き換える。  


ビルド結果 
----------
install/に設定。  

	cp -rf /usr/local/ssl install/


参考  
----  
http://wiki.openssl.org/index.php/FIPS_Library_and_Android

