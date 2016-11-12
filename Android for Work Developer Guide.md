
    [Managed profile compatibility](https://developer.android.com/work/guide.html#managed-profiles)—Modify your Android app so it functions best on an Android device with a work profile.
    [Managed configurations—Modify](https://developer.android.com/work/guide.html#managed-configurations) your app to allow IT administrators the option to specify custom settings for your apps.
    [Corporate-owned, single-use (COSU)](https://developer.android.com/work/guide.html#cosu)—Optimize your app so that it can be deployed on an Android device as a **kiosk**.
    [Single Sign-On (SSO)](https://developer.android.com/work/guide.html#sso)—Simplify the sign-on process for users signing in to different apps on their Android device running Android for Work.

[AOSP中managed-profile的解釋](https://source.android.com/devices/tech/admin/managed-profiles.html)

A managed profile or work profile is an Android user with additional special properties around management and visual aesthetic.

The primary goal of a managed profile is to create a segregated and secure space for managed data (such as corporate data) to reside. The administrator of the profile has full control over scope, ingress, and egress of data as well as its lifetime. These policies offer great powers and therefore fall upon the managed profile instead of the device administrator.

    Creation. Managed profiles can be created by any application in the primary user. The user is notified of managed profile behaviors and policy enforcement before creation.
    Management. Management is performed by applications that programmatically invoke APIs in the DevicePolicyManager class to restrict use. Such applications are referred to as profile owners and are defined at initial profile setup. Policies unique to managed profile involve app restrictions, updatability, and intent behaviors.
    Visual treatment. Applications, notifications, and widgets from the managed profile are always badged and typically made available inline with user interface (UI) elements from the primary user.
