default_platform(:ios)
platform :ios do
#       desc ???Install pod dependencies???
#       lane :install_pods do
#          cocoapods(
#              podfile: "/Users/ec2-user/.jenkins/workspace/SampleProject",
#              use_bundle_exec: false)


#       desc "Incrementing Build Number"
#       lane :increment_build do
#            current_build_number = latest_testflight_build_number(version: "1.0")
#            increment_build_number(
#            build_number: current_build_number + 1
#            )
       end

#      lane :build_ipa do
#          gym(
#             scheme: "MyNotes",
#             output_directory: "/Users/ec2-user/.jenkins/workspace/SampleProject",
#             output_name: "MyNotes",
#             export_method: "app-store",
#             export_options: {
#               signingCertificates:"iPhone Distribution: NETSOL Technologies Limited",
#               provisioningProfiles:{
#                  "xyz.weom.explore" => "WEOM_Distribution_Profile"
#                              }
#              },
#            include_bitcode: false,
#            clean: true
#               )
#      end
#end
# default_platform(:ios)

# platform :ios do
#   desc "Description of what the lane does"
 lane :custom_lane do |options|
   #   sh "pwd" # => "[root]/fastlane"
  #    puts Dir.pwd # => "[root]/fastlane"
           xcodebuild(
                   project:"MyNotes.xcodeproj",
                   scheme: "MyNotes",
                   configuration: "Debug",
                   clean: options[:clean] || false,
                   build: true,
                   destination: "generic/platform=iOS",
                   output_directory: "/Users/ec2-user/.jenkins/workspace/SampleProject", # Destination directory. Defaults to current directory.
                   output_name: "MyNotes.ipa",
                   build_settings: {
                    "CODE_SIGNING_REQUIRED" => "NO",
                    "CODE_SIGN_IDENTITY" => ""
                 }
              )
   end
# end


# default_platform(:ios)

# platform :ios do
#   desc "Description of what the lane does"
#   lane :custom_lane do
#     # add actions here: https://docs.fastlane.tools/actions
#      gym(
#         # Specify the project or workspace file name
#         project: "MyNotes.xcodeproj",
#         # Set the scheme to build
#         scheme: "MyNotes",
#         # Set the output directory for the build
#         output_directory: "./builds",
#         # Set the name for the output .ipa file
#         output_name: "MyNotes.ipa"
#        )
#          puts("hi zain")
#   end
# end
# Fastfile

# default_platform(:ios)

# # Define lane for creating a build
# lane :build do
#   # Use gym action to create a build
#   gym(
#     # Specify the project or workspace file name
#     project: "MyNotes.xcodeproj",
#     # Set the scheme to build
#     scheme: "MyNotes",
#     # Set the output directory for the build
#     output_directory: "./builds",
#     # Set the name for the output .ipa file
#     output_name: "MyNotes.ipa"
#   )
# end
