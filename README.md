#Verve Ad Library SDK

##Overview

* __samples__ - This is the directory containing sample code for the Android AdSDK.

The Verve Ad SDK requires a run-time of Android 2.3 or later (set minSdkVersion to at least 9). </br>

###Project Setup
#### 1. Obtain Partner (Ad) Keyword
Obtain a partner (ad) keyword from your Verve Mobile Account Manager to allow you to retrieve Vere Ads. A temporary partner (ad) keyword of “adsdkexample” has been included in the samples for your convenience. This keyword will allow you to see ads filled 100% of the time (banner and interstitial) and can be used for testing.
#### 2. Add Verve Ad SDK To Project
Add the Verve Ad SDK (Verve_AdSDK_1.3.17.jar file) to your Android project.
#### 3. Configure Dependencies for IDE
#####3.1 Eclipse
1. Add the Android Support Library (android-support-v4.jar file) to your Eclipse project. See the instructions for how to download and add the Support Library without resources to your project: <https://developer.android.com/tools/support-library/setup.html>
2. Add and reference the Google Play services library project in your Eclipse workspace. See the instructions for how to set up the Google Play services SDK: <https://developer.android.com/google/play-services/setup.html>

#####3.2 Android Studio
1. Open your module's build.gradle file and add the following dependencies:

			compile 'com.android.support:appcompat-v7:21.+'




		<application>
		


		</application>

		<application>
			<receiver android:name="com.vervewireless.advert.LocalNotificationReceiver">



            	@Override
            	public void onAdLoaded(AdResponse response) {
                	Log.d("Test", "AdView loaded");
            	}

            	@Override
            	public void onAdError(AdError e) {
                	Log.e("Test", "AdView error:" + e);
            		}

            	@Override
            	public void onNoAdReturned(AdResponse response) {
                	Log.d("Test", "AdView no ad");
            	}

            	@Override
            	public void onAdPageFinished() {
               		Log.d("Test", "AdView page finished loading");
            	}
        	});
        

            	@Override
            	public void onAdLoaded(AdResponse response) {
                	Log.d("Test", "AdView loaded");
            	}

            	@Override
            	public void onAdError(AdError e) {
                	Log.e("Test", "AdView error:" + e);
            	}

            	@Override
            	public void onNoAdReturned(AdResponse response) {
                	Log.d("Test", "AdView no ad");
            	}

            	@Override
            	public void onAdPageFinished() {
                	Log.d("Test", "AdView page finished loading");
            	}
        	});
        



	adRequest.setCategory(Category.HOME_PAGE);




            @Override
           	public void onAdLoaded(AdResponse response) {
               	Log.d("Test", "AdView loaded");
           	}

           	@Override
           	public void onAdError(AdError e) {
               	Log.e("Test", "AdView error:" + e);
          	}

           	@Override
            public void onNoAdReturned(AdResponse response) {
               	Log.d("Test", "AdView no ad");
           	}

            @Override
           	public void onAdPageFinished() {
             	Log.d("Test", "AdView page finished loading");
            }
        });


            @Override
            public boolean onAdClicked(Ad ad, Uri uri) {
                Log.d("Test", "AdView link clicked - uri: " + uri.toString());

				/*
                 * If you want to handle clicks on ad
				 * and override the default behavior,
				 * return true, otherwise return false.
				 */
                return false;
            }
        });
























		<application>
			


		/** The listener to be notified about activity lifecycle. */
	
			RelativeLayout.LayoutParams params = new RelativeLayout.LayoutParams(LayoutParams.MATCH_PARENT, LayoutParams.WRAP_CONTENT);
			params.addRule(RelativeLayout.ALIGN_PARENT_BOTTOM);

				@Override
				public void onAdLoaded() {
					Log.d(InterstitialSample.LOG_TAG, "onAdLoaded");
					interstitialAd.show();
				}
		
				/** Called when an ad failed to load. */
				@Override
				public void onAdFailedToLoad(int errorCode) {
					Log.d(InterstitialSample.LOG_TAG, "onAdFailedToLoad");
				}
		
				/**
		 		 * Called when an Activity is created in front of the app (e.g. an interstitial is shown, or an
		 		 * ad is clicked and launches a new Activity).
		 		 */
				@Override
				public void onAdOpened() {
					Log.d(InterstitialSample.LOG_TAG, "onAdOpened");
				}
		
				/** Called when an ad is closed and about to return to the application. */
				@Override
				public void onAdClosed() {
					Log.d(InterstitialSample.LOG_TAG, "onAdClosed");
				}
		
				/**
		 		 * Called when an ad is clicked and going to start a new Activity that will leave the
		 		 * application (e.g. breaking out to the Browser or Maps application).
		 		 */
				@Override
				public void onAdLeftApplication() {
					Log.d(InterstitialSample.LOG_TAG, "onAdLeftApplication");
				}















		
		dependencies {
			compile 'com.android.support:support-annotations:22.0.0'
			compile 'com.mopub.volley:mopub-volley:1.1.0'
			compile (name:'mopub-sdk-3.8.0', ext:'aar')
		}


				dirs 'libs'
			jcenter()
		}

The contents of these identical files should be included in your Proguard config when using the MoPub SDK in a Proguarded project.
https://github.com/mopub/mopub-android-sdk/blob/master/mopub-sample/proguard.cfg__

				/** Called when an ad failed to load. */
				@Override
				public void onInterstitialFailed(MoPubInterstitial interstitial, MoPubErrorCode errorCode) {
					Log.d(InterstitialSample.LOG_TAG, "onInterstitialFailed");
				}

				/**
		 		 * Called when an Activity is created in front of the app (an interstitial is shown).
		 		 */
				@Override
				public void onInterstitialShown(MoPubInterstitial interstitial) {
					Log.d(InterstitialSample.LOG_TAG, "onInterstitialShown");
				}

				/**
		 		 * Called when an ad is clicked and going to start a new Activity that will leave the
		 		 * application (e.g. breaking out to the Browser or Maps application).
		 		 */
				@Override
				public void onInterstitialClicked(MoPubInterstitial interstitial) {
					Log.d(InterstitialSample.LOG_TAG, "onInterstitialClicked");
				}

				/** Called when an ad is closed and about to return to the application. */
				@Override
				public void onInterstitialDismissed(MoPubInterstitial interstitial) {
					Log.d(InterstitialSample.LOG_TAG, "onInterstitialDismissed");
				}



























<link rel="stylesheet" href="http://yandex.st/highlightjs/7.3/styles/github.min.css">
<script>
  hljs.initHighlightingOnLoad();
</script>