source 'https://github.com/CocoaPods/Specs.git'
platform :ios, ‘9.0’

target 'RadishMeeting' do

    pod 'yoga', :path => '../node_modules/react-native/ReactCommon/yoga'
    pod 'DoubleConversion', :podspec => '../node_modules/react-native/third-party-podspecs/DoubleConversion.podspec'
    pod 'glog', :podspec => '../node_modules/react-native/third-party-podspecs/GLog.podspec'
    pod 'Folly', :podspec => '../node_modules/react-native/third-party-podspecs/Folly.podspec'
    pod 'React', :path => '../node_modules/react-native', :subspecs => [
    'Core',
#    'DevSupport',
    'CxxBridge',
    'RCTImage'
    ]
    
    pod 'AFNetworking', '~> 3.0'
    pod 'Masonry'

  pod 'react-native-contacts', :path => '../node_modules/react-native-contacts'
  pod 'react-native-camera', path: '../node_modules/react-native-camera'#调用相机
  pod 'RNImageCropPicker', :path => '../node_modules/react-native-image-crop-picker' #相册选择
  pod 'rn-fetch-blob', :path => '../node_modules/rn-fetch-blob'
  pod 'RNFS', :path => '../node_modules/react-native-fs'
  pod 'RNViewShot', :path => '../node_modules/react-native-view-shot'
  pod 'BVLinearGradient', :path => '../node_modules/react-native-linear-gradient'

  pod 'CodePush', :path => '../node_modules/react-native-code-push'

  pod 'RNDeviceInfo', :path => '../node_modules/react-native-device-info'

  pod 'react-native-netinfo', :path => '../node_modules/@react-native-community/netinfo'

  pod 'RNI18n', :path => '../node_modules/react-native-i18n'

  pod 'RCTSystemSetting', :path => '../node_modules/react-native-system-setting'

  pod 'RNSVG', :path => '../node_modules/react-native-svg'

  pod 'boost-for-react-native', :git => 'https://gitee.com/damon-s/boost-for-react-native.git’

  
  pod 'UMCPush' #友盟推送
  pod 'UMCCommon' #友盟基础库
  pod 'UMCSecurityPlugins' #友盟基础库
  pod 'Bugly' #Bugly
  pod 'FSScrollContentView'
  pod 'SDWebImage'
  pod 'SDWebImage/GIF'
  #卓朗弹框
  pod 'RNTroilaAlert', :path => '../node_modules/react-native-troila-alert/ios/RNTroilaAlert.podspec'
  pod 'RealReachability'
  #SocketRocket
  pod 'SocketRocket’
  pod 'GoogleWebRTC'
  pod 'MJExtension'
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        if target.name == "React"
            target.remove_from_project
        end
    end
end