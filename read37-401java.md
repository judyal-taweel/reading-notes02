## What is Amazon S3?

Amazon Simple Storage Service (Amazon S3) is storage for the Internet. It is designed to make web-scale computing easier.

This guide describes how you send requests to create buckets, store and retrieve your objects, and manage permissions on your resources. The guide also describes access control and the authentication process. Access control defines who can access objects and buckets within Amazon S3, and the type of access (for example, READ and WRITE). The authentication process verifies the identity of a user who is trying to access Amazon Web Services (AWS).

### Advantages of using Amazon S3

- Creating buckets – Create and name a bucket that stores data. Buckets are the fundamental containers in Amazon S3 for data storage.

- Storing data – Store an infinite amount of data in a bucket. Upload as many objects as you like into an Amazon S3 bucket. Each object can contain up to 5 TB of data. Each object is stored and retrieved using a unique developer-assigned key.

- Downloading data – Download your data or enable others to do so. Download your data anytime you like, or allow others to do the same.

- Permissions – Grant or deny access to others who want to upload or download data into your Amazon S3 bucket. Grant upload and download permissions to three types of users. Authentication mechanisms can help keep data secure from unauthorized access.

- Standard interfaces – Use standards-based REST and SOAP interfaces designed to work with any internet-development toolkit.

## Buckets serve several purposes:

- They organize the Amazon S3 namespace at the highest level.

- They identify the account responsible for storage and data transfer charges.

- They play a role in access control.

- They serve as the unit of aggregation for usage reporting.

## Bucket configurations have an eventual consistency model. Specifically:

- If you delete a bucket and immediately list all buckets, the deleted bucket might still appear in the list.

- If you enable versioning on a bucket for the first time, it might take a short amount of time for the change to be fully propagated. We recommend that you wait for 15 minutes after enabling versioning before issuing write operations (PUT or DELETE) on objects in the bucket.

### Common operations

- Create a bucket – Create and name your own bucket in which to store your objects.

- Write an object – Store data by creating or overwriting an object. When you write an object, you specify a unique key in the namespace of your bucket. This is also a good time to specify any access control you want on the object.

- Read an object – Read data back. You can download the data via HTTP.

- Delete an object – Delete some of your data.

- List keys – List the keys contained in one of your buckets. You can filter the key list based on a prefix.

## To start provisioning storage resources in the backend, go to your project directory and execute the command:

```
amplify add storage
```

```
dependencies {
    implementation 'com.amplifyframework:aws-storage-s3:1.24.0'
    implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'
}
```
```
Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.addPlugin(new AWSS3StoragePlugin());
```

```
public class MyAmplifyApp extends Application {
    @Override
    public void onCreate() {
        super.onCreate();

        try {
            // Add these lines to add the AWSCognitoAuthPlugin and AWSS3StoragePlugin plugins
            Amplify.addPlugin(new AWSCognitoAuthPlugin());
            Amplify.addPlugin(new AWSS3StoragePlugin());
            Amplify.configure(getApplicationContext());

            Log.i("MyAmplifyApp", "Initialized Amplify");
        } catch (AmplifyException error) {
            Log.e("MyAmplifyApp", "Could not initialize Amplify", error);
        }
    }
}
```