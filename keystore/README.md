# Android release signing

Store the private release key `mediasteru-release.jks` in this folder, but do
not commit it. Back up the key and `companion-android/keystore.properties` in a
secure location; losing either prevents signing compatible Android updates.

Create `companion-android/keystore.properties` locally with:

```properties
storeFile=../keystore/mediasteru-release.jks
storePassword=<store password>
keyAlias=companion
keyPassword=<key password>
```

The `.jks` and properties file are ignored by Git. Keep their backups separate
from this repository.
