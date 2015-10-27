# Uncomment this line to define a global platform for your project
platform :ios, '8.0'
use_frameworks!

target 'MaxBoxDemo' do
    
    pod 'Mapbox-iOS-SDK'
    
    # disable bitcode in every sub-target
    post_install do |installer|
        installer.pods_project.targets.each do |target|
            target.build_configurations.each do |config|
                config.build_settings['ENABLE_BITCODE'] = 'NO'
            end
        end
    end

end

