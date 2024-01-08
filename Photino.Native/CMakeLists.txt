
# TODO: copy Exports.cpp to Exports.mm and remove it after building

add_library(Photino.Native SHARED 		  
    "Photino.Mac.AppDelegate.mm"
    "Photino.Mac.UiDelegate.mm"
    "Photino.Mac.UrlSchemeHandler.mm"
    "Photino.Mac.NSWindowBorderless.mm"
    "Photino.Mac.Dialog.mm"
    "Photino.Mac.mm"
    "Exports.mm")

target_link_libraries(Photino.Native "-framework Cocoa" "-framework WebKit" "-framework UserNotifications")