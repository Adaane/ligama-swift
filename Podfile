# Uncomment the next line to define a global platform for your project
platform :ios, '13.0'

target 'Ligama' do
  use_frameworks!

  pod 'FirebaseCore', '10.7.0'
  pod 'FirebaseAnalytics', '10.7.0'
  pod 'FirebaseCoreInternal', '10.7.0'
  pod 'FirebaseInstallations', '10.7.0'
  pod 'GoogleUtilities', '7.11.5'
  pod 'FirebaseMessaging', '10.7.0'

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
    end
  end
end
