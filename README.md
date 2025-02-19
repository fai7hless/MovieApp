Frontend
1. Node.js + npm - https://nodejs.org/en/download/package-manager
2. Android Studio/SDK - https://developer.android.com/studio
 - Set ANDROID_HOME path - https://www.ibm.com/docs/en/devops-test-ui/11.0.1?topic=prwut-setting-changing-android-home-path-in-windows-operating-systems
3. Open MovieApp folder and run "npm install" in a terminal
4. Chnage the ip address to your ipv4 address for the back end inside usePushNotifications.tsx, movie-list.tsx and [id].tsx
5. Add the api credentials for the Facebook SDK inside of app.json
6. Set up an emulator through Android studio or use a physical device connected with a usb cable
4. Use "npx expo start" for development build
or "npx expo start --no-dev --minify" for production build

Backend
1. Download PHP - https://windows.php.net/download#php-8.3 
- set enivronment variable Path to PHP installation directory
2. Download Composer - https://getcomposer.org/download/
3. Download MySQL installer - https://dev.mysql.com/downloads/
4. Edit php.in located in your PHP directory and enable extensions - fileinfo,mysqli,pdo_mysql (depending on database)
5. Open MovieApi folder and run these commands
5. composer install
6. cp .env.example .env
- input MySQL details in .env
8. php artisan key:generate
9. php artisan migrate
10. php artisan serve --host=0.0.0.0 --port=8000

How to send push notification
1. Open the Expo Push Notification Tool - https://expo.dev/notifications
2. Get the Expo Push Token from the database (should look something like this "ExponentPushToken[xxxxxxxxxxxxxx]")
3. Enter a recipient(Push token), title and message
4. (Optional) Enter a data payload if you want the notification to redirect to a specific movies' details page. The format is {"movieId": "2","screen": "MovieDetails"} change only the movieId

Demonstration of push notification: https://www.youtube.com/watch?v=EZ8jcsdjS9U

![Screenshot_1](https://github.com/user-attachments/assets/ef2a2969-69cf-4324-8b6f-8464ff2ee91b)
![Screenshot_2](https://github.com/user-attachments/assets/5a0fe1a1-7ccd-4edf-9291-f886b962e8b7)
![Screenshot_3](https://github.com/user-attachments/assets/2e87a3df-7120-4bce-8a45-cef911a29951)
![Screenshot_4](https://github.com/user-attachments/assets/f612f4d5-779e-4940-8980-d92cf4c9bff6)



