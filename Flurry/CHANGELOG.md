## Changelog
 * 12.5.0.0
    * This version of the adapter has been certified with Flurry 12.5.0 and MoPub SDK 5.13.1.
    * This version of the adapter will only support native ad format.
    * Deprecate Flurry interstitial adapter support.
    Note: We are [deprecating Flurry mediation support](https://developers.mopub.com/publishers/mediation/networks/yahooflurry/) for interstitial ad format. Publishers mediating Flurry via supported connection should migrate from Flurry connection to
    [Verizon Media Connection](https://developers.mopub.com/publishers/mediation/networks/verizon/) for interstitial format.

 * 12.0.3.1
    * Log Flurry ad space name in ad lifecycle events.
    * Map additional error codes for failure cases.

 * 12.0.3.0
    * This version of the adapters has been certified with Flurry 12.0.3.

 * 11.7.1.1
    * Add support for AndroidX. This is the minimum version compatible with MoPub 5.9.0.

 * 11.7.1.0
    * This version of adapters has been certified with Flurry 11.7.1.

 * 11.6.0.2
    * Add a call to `setTargeting()` for Flurry native ads. Currently supported is the ability to enable test mode via `localExtras`.

 * 11.6.0.1
    * Allow `null` FlurryAgentListener in FlurryAgentWrapper to start Flurry agent.

 * 11.6.0.0
    * This version of adapters has been certified with Flurry 11.6.0.
    
 * 11.5.0.1
    * Flurry Adapter will now be released as an Android Archive (AAR) file that includes manifest file for [Flurry manifest changes](https://developer.yahoo.com/flurry/docs/integrateflurry/android-manual/#configure-the-androidmanifest-and-proguard-files).

  * 11.5.0.0
    * This version of the adapters has been certified with Flurry 11.5.0.

  * 11.4.0.1
    * **Note**: This version is only compatible with the 5.5.0+ release of the MoPub SDK.
    * Add the `FlurryAdapterConfiguration` class to: 
         * pre-initialize the Flurry SDK during MoPub SDK initialization process
         * store adapter and SDK versions for logging purpose
    * Streamline adapter logs via `MoPubLog` to make debugging more efficient. For more details, check the [Android Initialization guide](https://developers.mopub.com/docs/android/initialization/) and [Writing Custom Events guide](https://developers.mopub.com/docs/android/custom-events/).

  * 11.4.0.0
    * This version of the adapters has been certified with Flurry 11.4.0.
    
  * 10.1.0.2
    * Expose the native ad's advertiser name asset for publishers to show as required by Flurry (https://developer.yahoo.com/flurry/docs/publisher/gettingstarted/nativeadguidelines/).

  * 10.1.0.1
    * Align MoPub's interstitial impression tracking to that of Flurry. 
        * `setAutomaticImpressionAndClickTracking` is set to `false`, and Flurry's `onRendered` callback is leveraged to fire MoPub impressions. This change requires MoPub 5.3.0 or higher.

  * 10.1.0.0
    * This version of the adapters has been certified with Flurry 10.1.0.

  * 9.0.0.0
    * This version of the adapters has been certified with Flurry 9.0.0.

  * 8.2.0.1
    * Fix an NPE in FlurryNativeAdRenderer's StaticNativeViewHolder.

  * 8.2.0.0
    * This version of the adapters has been certified with Flurry 8.2.0.

  * Initial Commit
  	* Adapters moved from [mopub-android-sdk](https://github.com/mopub/mopub-android-sdk) to [mopub-android-mediation](https://github.com/mopub/mopub-android-mediation/)
