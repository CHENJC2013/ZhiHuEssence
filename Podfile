source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'
use_frameworks!

target 'ZhiHuEssence' do
    pod 'CocoaLumberjack/Swift'
    pod 'AlamofireObjectMapper'
    pod 'SwifterSwift', '~> 3.2.0'
    #pod 'RestKit', :head, :subspecs => ['Core', 'CocoaLumberjack'] #http://stackoverflow.com/questions/31923006/restkit-and-cocoalumberjack-integrated-as-frameworks-in-xcode7
#    pod 'Reachability'
#    pod 'RealReachability'
    pod 'PKHUD', '~> 5.0'
    pod 'Kingfisher'
    pod 'IQKeyboardManagerSwift'
    pod 'Colours/Swift'
    #pod 'iRate'
#    pod 'Harpy'
    pod 'SAMKeychain'
    pod 'DZNEmptyDataSet'
    pod 'Masonry'
#    pod 'FBMemoryProfiler'

    
#    pod 'FCUUID'

    # Swift Pods
#    pod 'Hero', '~> 0.3.6'
#    pod 'PageMenu'  #因为要使用OC版本，改为直接添加文件至Vendor
#    pod 'Charts'    #Drag the Charts.xcodeproj to your project,否则会报Error ITMS-90086、90087、90209、90125、90203的问题
end



#解决上传报错Error ITMS-90635的问题
#http://www.jianshu.com/p/34616dd42da4、http://blog.csdn.net/lovehalok/article/details/51594473、http://www.jianshu.com/p/176ea563f051
post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['ENABLE_BITCODE'] = 'NO'
            #config.build_settings['SWIFT_VERSION'] = '3.0'  ##http://stackoverflow.com/questions/38446097/xcode-8-beta-3-use-legacy-swift-issue
        end
    end
end
