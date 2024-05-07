#### This is the sample project to create a CICD pipeline using the GitHub Actions workflow to build & distribute MAUI Android & iOS builds to Google Play Store & Apple App Store.



# iOS 📱

### Command to copy base64

`base64 -i Certificates.p12 | pbcopy`

### Details to create the iOS required api keys to publish the ipa on Test Flight(App Store) can be found on:
https://docs.codemagic.io/yaml-publishing/app-store-connect/

### A visual representation can be found on: 
https://youtu.be/JfVu126Dfyc?feature=shared

(video is old and can be considered just for an refrence, refer documentatioon for updated directions)

# Android 📱

On https://console.cloud.google.com/ create a new project & download the json. The same json will be used for Secrets.SERVICE_ACCOUNT_JSON. It will create a new user.

After the user is created, the same user needs to granted with the access for the specific App on Google Console.
    
    • In Google Play Console go to "Settings" / "Developer Account" / "API Access".
    • You should see your Service Account there. Click on "Grant Access"
    • When you are cool with the permissions, press "Invite User"
    • The Service account should instantly accept the invite and things should work after that.
