# Power drain issues

1) Suspend command issued 100% battery life.

```
019-02-14T22:31:45.374679-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: Starting Login1 suspend job
2019-02-14T22:31:45.377825-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: Failed to start suspend job "org.freedesktop.login1.SleepVerbNotSupported" "Not enough swap space for hibernation"
2019-02-14T22:31:48.382855-06:00 rabbit-hole systemd-udevd[23557]: Process '/usr/sbin/tlp auto' failed with exit code 4.
2019-02-14T22:31:48.617201-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil:
2019-02-14T22:31:48.620631-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: Can't contact ck
2019-02-14T22:31:48.621056-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: We are now into activity  "121db2bd-7665-4c95-9b6f-f9dfe5b51310"
2019-02-14T22:31:48.621418-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: () ()
2019-02-14T22:31:48.621725-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: () ()
2019-02-14T22:31:48.621996-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: Loading profile for unplugged AC
2019-02-14T22:31:48.622266-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: Activity is not forcing a profile
2019-02-14T22:31:48.622555-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil:
2019-02-14T22:31:48.622881-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: Loading timeouts with  120000
2019-02-14T22:31:48.624117-06:00 rabbit-hole baloo_file[2169]: Power state changed
2019-02-14T22:31:48.718051-06:00 rabbit-hole plasmashell[2173]: plasma-pk-updates: Is on battery: true
2019-02-14T22:31:50.135728-06:00 rabbit-hole kernel: [128725.634663] usb 1-1: USB disconnect, device number 2
2019-02-14T22:31:50.135761-06:00 rabbit-hole kernel: [128725.634672] usb 1-1.1: USB disconnect, device number 4
2019-02-14T22:31:50.188117-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRNotify_OutputProperty (ignored)
2019-02-14T22:31:50.188541-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Output:  67
2019-02-14T22:31:50.188880-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Property:  EDID|U
2019-02-14T22:31:50.189242-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011State (newValue, Deleted):  1
2019-02-14T22:31:50.189593-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRNotify_OutputProperty (ignored)
2019-02-14T22:31:50.189964-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Output:  67
2019-02-14T22:31:50.190358-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Property:  EDID
2019-02-14T22:31:50.190742-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011State (newValue, Deleted):  1
2019-02-14T22:31:50.191109-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRNotify_OutputChange
2019-02-14T22:31:50.191587-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Output:  67
2019-02-14T22:31:50.191973-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011CRTC:  64
2019-02-14T22:31:50.192431-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Mode:  154
2019-02-14T22:31:50.192744-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Rotation:  "Rotate_0"
2019-02-14T22:31:50.193013-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Connection:  "Disconnected"
2019-02-14T22:31:50.193277-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Subpixel Order:  0
2019-02-14T22:31:50.194116-06:00 rabbit-hole kwin_x11[2166]: qt.qpa.xcb: QXcbConnection: XCB error: 3 (BadWindow), sequence: 50676, resource id: 37752565, major code: 15 (QueryTree), minor code: 0
2019-02-14T22:31:50.194431-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRScreenChangeNotify
2019-02-14T22:31:50.194718-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Window: 33554437
2019-02-14T22:31:50.203085-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Root: 433
2019-02-14T22:31:50.203486-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Rotation:  "Rotate_0"
2019-02-14T22:31:50.203830-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Size ID: 65535
2019-02-14T22:31:50.204164-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Size:  5760 2160
2019-02-14T22:31:50.204493-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011SizeMM:  1522 571
2019-02-14T22:31:50.204784-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRNotify_OutputChange
2019-02-14T22:31:50.205079-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Output:  67
2019-02-14T22:31:50.205447-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011CRTC:  64
2019-02-14T22:31:50.205825-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Mode:  154
2019-02-14T22:31:50.206166-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Rotation:  "Rotate_0"
2019-02-14T22:31:50.206469-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Connection:  "Disconnected"
2019-02-14T22:31:50.206779-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Subpixel Order:  0
2019-02-14T22:31:50.207064-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: XRandROutput 67 update
2019-02-14T22:31:50.207334-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011m_connected: 0
2019-02-14T22:31:50.207602-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011m_crtc XRandRCrtc(0x557c5df81b00)
2019-02-14T22:31:50.207957-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011CRTC: 64
2019-02-14T22:31:50.208292-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011MODE: 154
2019-02-14T22:31:50.208624-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Connection: 1
2019-02-14T22:31:50.208953-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Primary: false
2019-02-14T22:31:50.209259-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: Output 67 : connected = false , enabled = true
2019-02-14T22:31:50.209565-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: XRandROutput 67 update
2019-02-14T22:31:50.209868-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011m_connected: 1
2019-02-14T22:31:50.210178-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011m_crtc XRandRCrtc(0x557c5df81b00)
2019-02-14T22:31:50.210480-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011CRTC: 64
2019-02-14T22:31:50.210806-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011MODE: 154
2019-02-14T22:31:50.211116-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Connection: 1
2019-02-14T22:31:50.211424-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Primary: false
2019-02-14T22:31:50.211742-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: Output 67 : connected = false , enabled = true
2019-02-14T22:31:50.287353-06:00 rabbit-hole krunner[2171]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.288506-06:00 rabbit-hole kmozillahelper[3291]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.289304-06:00 rabbit-hole plasmashell[2173]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.290294-06:00 rabbit-hole baloo_file[2169]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.291192-06:00 rabbit-hole org_kde_powerdevil[2270]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.343712-06:00 rabbit-hole kernel: [128725.838963] usb 2-1: USB disconnect, device number 2
2019-02-14T22:31:50.345446-06:00 rabbit-hole kmozillahelper[3291]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.345895-06:00 rabbit-hole krunner[2171]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.346235-06:00 rabbit-hole baloo_file[2169]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.346560-06:00 rabbit-hole plasmashell[2173]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.346901-06:00 rabbit-hole org_kde_powerdevil[2270]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.351549-06:00 rabbit-hole krunner[2171]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.352026-06:00 rabbit-hole kmozillahelper[3291]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.352387-06:00 rabbit-hole org_kde_powerdevil[2270]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.352686-06:00 rabbit-hole plasmashell[2173]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.352973-06:00 rabbit-hole baloo_file[2169]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.487700-06:00 rabbit-hole kernel: [128725.984794] usb 1-1.2: USB disconnect, device number 6
2019-02-14T22:31:50.512724-06:00 rabbit-hole baloo_file[2169]: message repeated 6 times: [ UdevQt: unhandled device action "unbind"]
2019-02-14T22:31:50.525160-06:00 rabbit-hole kmozillahelper[3291]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.525640-06:00 rabbit-hole plasmashell[2173]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.525991-06:00 rabbit-hole kmozillahelper[3291]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.526304-06:00 rabbit-hole plasmashell[2173]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.526616-06:00 rabbit-hole krunner[2171]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.526928-06:00 rabbit-hole krunner[2171]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.527251-06:00 rabbit-hole kmozillahelper[3291]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.527589-06:00 rabbit-hole plasmashell[2173]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.527968-06:00 rabbit-hole plasmashell[2173]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.528329-06:00 rabbit-hole kmozillahelper[3291]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.528671-06:00 rabbit-hole krunner[2171]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.528982-06:00 rabbit-hole plasmashell[2173]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.529296-06:00 rabbit-hole kmozillahelper[3291]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.529652-06:00 rabbit-hole krunner[2171]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.529973-06:00 rabbit-hole krunner[2171]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.530287-06:00 rabbit-hole kmozillahelper[3291]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.530598-06:00 rabbit-hole plasmashell[2173]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.530909-06:00 rabbit-hole krunner[2171]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.531235-06:00 rabbit-hole org_kde_powerdevil[2270]: UdevQt: unhandled device action "unbind"
2019-02-14T22:31:50.532854-06:00 rabbit-hole org_kde_powerdevil[2270]: message repeated 5 times: [ UdevQt: unhandled device action "unbind"]
2019-02-14T22:31:50.729527-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: Emitting configChanged()
2019-02-14T22:31:50.972870-06:00 rabbit-hole kdeinit5[2131]: kscreen: Requesting missing EDID for outputs (66)
2019-02-14T22:31:50.973300-06:00 rabbit-hole org_kde_powerdevil[2270]: kscreen: Requesting missing EDID for outputs (66)
2019-02-14T22:31:51.016719-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: XRandR::setConfig
2019-02-14T22:31:51.017196-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: Requested screen size is QSize(1920, 1080)
2019-02-14T22:31:51.017555-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: Needed CRTCs:  1
2019-02-14T22:31:51.017883-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: Actions to perform:
2019-02-14T22:31:51.018243-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Primary Output: false
2019-02-14T22:31:51.018555-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Change Screen Size: true
2019-02-14T22:31:51.018871-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011#011Old: QSize(5760, 2160)
2019-02-14T22:31:51.019223-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011#011Intermediate: QSize(5760, 2160)
2019-02-14T22:31:51.019572-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011#011New: QSize(1920, 1080)
2019-02-14T22:31:51.019897-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Disable outputs: true
2019-02-14T22:31:51.020167-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011#011 (67)
2019-02-14T22:31:51.020454-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Change outputs: false
2019-02-14T22:31:51.020722-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Enable outputs: false
2019-02-14T22:31:51.021043-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: RRSetCrtcConfig (disable output)
2019-02-14T22:31:51.021317-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011CRTC: 64
2019-02-14T22:31:51.318404-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Result: 0
2019-02-14T22:31:51.318575-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: XRandROutput 67 update
2019-02-14T22:31:51.318688-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011m_connected: 1
2019-02-14T22:31:51.318792-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011m_crtc XRandRCrtc(0x557c5df81b00)
2019-02-14T22:31:51.318895-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011CRTC: 0
2019-02-14T22:31:51.318992-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011MODE: 0
2019-02-14T22:31:51.319083-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Connection: 1
2019-02-14T22:31:51.319197-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Primary: false
2019-02-14T22:31:51.319313-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: Disconnected output 67 from CRTC 64
2019-02-14T22:31:51.319429-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: RRSetScreenSize
2019-02-14T22:31:51.319552-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011DPI: 96.0841
2019-02-14T22:31:51.319709-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Size: QSize(1920, 1080)
2019-02-14T22:31:51.319810-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011SizeMM: QSize(507, 285)
2019-02-14T22:31:51.319902-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: XRandR::setConfig done!
2019-02-14T22:31:51.385909-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRNotify_CrtcChange
2019-02-14T22:31:51.386615-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011CRTC:  64
2019-02-14T22:31:51.386971-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Mode:  0
2019-02-14T22:31:51.387257-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Rotation:  "Rotate_0"
2019-02-14T22:31:51.387552-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Geometry:  0 0 0 0
2019-02-14T22:31:51.387899-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRNotify_OutputChange
2019-02-14T22:31:51.388215-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Output:  67
2019-02-14T22:31:51.388524-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011CRTC:  0
2019-02-14T22:31:51.388809-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Mode:  0
2019-02-14T22:31:51.389125-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Rotation:  "Rotate_0"
2019-02-14T22:31:51.389411-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Connection:  "Disconnected"
2019-02-14T22:31:51.389721-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Subpixel Order:  0
2019-02-14T22:31:51.390051-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRScreenChangeNotify
2019-02-14T22:31:51.390384-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Window: 33554437
2019-02-14T22:31:51.390703-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Root: 433
2019-02-14T22:31:51.391029-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Rotation:  "Rotate_0"
2019-02-14T22:31:51.391388-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Size ID: 65535
2019-02-14T22:31:51.391764-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Size:  5760 2160
2019-02-14T22:31:51.392072-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011SizeMM:  1522 571
2019-02-14T22:31:51.392364-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRNotify_CrtcChange
2019-02-14T22:31:51.392646-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011CRTC:  64
2019-02-14T22:31:51.392927-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Mode:  0
2019-02-14T22:31:51.393211-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Rotation:  "Rotate_0"
2019-02-14T22:31:51.393516-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Geometry:  0 0 0 0
2019-02-14T22:31:51.393803-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRNotify_OutputChange
2019-02-14T22:31:51.394094-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Output:  67
2019-02-14T22:31:51.394370-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011CRTC:  0
2019-02-14T22:31:51.394639-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Mode:  0
2019-02-14T22:31:51.394904-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Rotation:  "Rotate_0"
2019-02-14T22:31:51.395187-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Connection:  "Disconnected"
2019-02-14T22:31:51.395518-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Subpixel Order:  0
2019-02-14T22:31:51.395820-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: RRScreenChangeNotify
2019-02-14T22:31:51.396150-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Window: 33554437
2019-02-14T22:31:51.396462-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Root: 433
2019-02-14T22:31:51.396748-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Rotation:  "Rotate_0"
2019-02-14T22:31:51.397113-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Size ID: 0
2019-02-14T22:31:51.397469-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011Size:  1920 1080
2019-02-14T22:31:51.397867-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xcb.helper: #011SizeMM:  507 285
2019-02-14T22:31:51.398229-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: XRandROutput 67 update
2019-02-14T22:31:51.398538-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011m_connected: 1
2019-02-14T22:31:51.398910-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011m_crtc QObject(0x0)
2019-02-14T22:31:51.399252-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011CRTC: 0
2019-02-14T22:31:51.399590-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011MODE: 0
2019-02-14T22:31:51.400222-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Connection: 1
2019-02-14T22:31:51.400568-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Primary: false
2019-02-14T22:31:51.400982-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: Output 67 : connected = false , enabled = false
2019-02-14T22:31:51.411473-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: XRandROutput 67 update
2019-02-14T22:31:51.411937-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011m_connected: 1
2019-02-14T22:31:51.412259-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011m_crtc QObject(0x0)
2019-02-14T22:31:51.412538-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011CRTC: 0
2019-02-14T22:31:51.412805-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011MODE: 0
2019-02-14T22:31:51.413072-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Connection: 1
2019-02-14T22:31:51.413350-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: #011Primary: false
2019-02-14T22:31:51.413622-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: Output 67 : connected = false , enabled = false
2019-02-14T22:31:51.421610-06:00 rabbit-hole org_kde_powerdevil[2270]: kscreen: Requesting missing EDID for outputs (66)
2019-02-14T22:31:51.422067-06:00 rabbit-hole kdeinit5[2131]: kscreen: Requesting missing EDID for outputs (66)
2019-02-14T22:31:51.887387-06:00 rabbit-hole kscreen_backend_launcher[2182]: kscreen.xrandr: Emitting configChanged()
2019-02-14T22:31:52.110359-06:00 rabbit-hole kdeinit5[2131]: kscreen: Requesting missing EDID for outputs (66)
2019-02-14T22:31:52.110796-06:00 rabbit-hole org_kde_powerdevil[2270]: kscreen: Requesting missing EDID for outputs (66)
2019-02-14T22:31:55.523573-06:00 rabbit-hole systemd-logind[1318]: Lid closed.
2019-02-14T22:31:55.528449-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: Suspend session triggered with QMap(("Explicit", QVariant(bool, true))("Type", QVariant(uint, 1)))
2019-02-14T22:31:55.675262-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: Suspend session triggered with QMap(("Explicit", QVariant(bool, true))("SkipFade", QVariant(bool, true))("Type", QVariant(uint, 1)))
2019-02-14T22:31:55.678093-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: Starting Login1 suspend job
2019-02-14T22:31:55.713766-06:00 rabbit-hole org_kde_powerdevil[2270]: powerdevil: Pausing all media players before suspending
2019-02-14T22:31:55.715464-06:00 rabbit-hole kdeinit5[2131]: bluedevil: About to suspend
2019-02-14T22:31:55.717046-06:00 rabbit-hole ksmserver[2150]: lock called
2019-02-14T22:31:55.781730-06:00 rabbit-hole ksmserver[2150]: Lock window Id:  23068779
2019-02-14T22:31:55.792826-06:00 rabbit-hole ksmserver[2150]: CreateNotify: 23068779
2019-02-14T22:31:55.991421-06:00 rabbit-hole ksmserver[2150]: CreateNotify: 92274692
2019-02-14T22:31:56.026132-06:00 rabbit-hole kscreenlocker_greet[23756]: Qt: Session management error: networkIdsList argument is NULL
2019-02-14T22:31:56.086031-06:00 rabbit-hole ksmserver[2150]: CreateNotify: 92274696
2019-02-14T22:31:56.095412-06:00 rabbit-hole ksmserver[2150]: CreateNotify: 92274704
2019-02-14T22:31:56.113074-06:00 rabbit-hole ksmserver[2150]: CreateNotify: 92274709
2019-02-14T22:31:56.268089-06:00 rabbit-hole ksmserver[2150]: CreateNotify: 92274711
2019-02-14T22:31:56.268286-06:00 rabbit-hole ksmserver[2150]: CreateNotify: 92274713
2019-02-14T22:31:56.269908-06:00 rabbit-hole ksmserver[2150]: MapNotify: 92274711
2019-02-14T22:31:56.286639-06:00 rabbit-hole ksmserver[2150]: CreateNotify: 92274715
2019-02-14T22:31:56.727913-06:00 rabbit-hole kscreenlocker_greet[23756]: UdevQt: unable to create udev monitor connection
2019-02-14T22:31:56.911955-06:00 rabbit-hole ksmserver[2150]: CreateNotify: 92274724
2019-02-14T22:31:57.044382-06:00 rabbit-hole kscreenlocker_greet[23756]: Connecting to deprecated signal QDBusConnectionInterface::serviceOwnerChanged(QString,QString,QString)
2019-02-14T22:31:57.417569-06:00 rabbit-hole ksmserver[2150]: MapNotify: 23068779
2019-02-14T22:31:57.445442-06:00 rabbit-hole systemd[1]: Reached target Sleep.
2019-02-14T22:31:57.446839-06:00 rabbit-hole systemd[1]: Starting Suspend...
2019-02-14T22:31:57.462106-06:00 rabbit-hole systemd-sleep[23771]: INFO: Skip running /usr/lib/systemd/system-sleep/grub2.sleep for suspend
2019-02-14T22:31:57.462258-06:00 rabbit-hole systemd-sleep[23771]: Suspending system...
2019-02-14T22:31:57.463641-06:00 rabbit-hole kernel: [128732.961368] PM: suspend entry (s2idle)
```

2) Powering on Battery 75%.

```
2019-02-15T08:49:00.909322-06:00 rabbit-hole kernel: [128732.961370] PM: Syncing filesystems ... done.
2019-02-15T08:49:00.909434-06:00 rabbit-hole kernel: [128733.016659] Freezing user space processes ... (elapsed 0.002 seconds) done.
2019-02-15T08:49:00.909437-06:00 rabbit-hole kernel: [128733.018884] OOM killer disabled.
2019-02-15T08:49:00.909438-06:00 rabbit-hole kernel: [128733.018885] Freezing remaining freezable tasks ... (elapsed 0.001 seconds) done.
2019-02-15T08:49:00.909439-06:00 rabbit-hole kernel: [128733.020411] printk: Suspending console(s) (use no_console_suspend to debug)
2019-02-15T08:49:00.909440-06:00 rabbit-hole kernel: [128733.021522] wlp2s0: deauthenticating from 7a:8a:20:2e:5f:31 by local choice (Reason: 3=DEAUTH_LEAVING)
2019-02-15T08:49:00.909443-06:00 rabbit-hole kernel: [165755.347691] ath10k_pci 0000:02:00.0: unsupported HTC service id: 1536
2019-02-15T08:49:00.909444-06:00 rabbit-hole kernel: [165755.358962] nvme nvme0: Shutdown timeout set to 8 seconds
2019-02-15T08:49:00.909445-06:00 rabbit-hole kernel: [165755.363111] ath10k_pci 0000:02:00.0: Unknown eventid: 118809
2019-02-15T08:49:00.909446-06:00 rabbit-hole kernel: [165755.448096] WARNING: CPU: 1 PID: 23798 at drivers/net/wireless/ath/ath10k/mac.c:5650 ath10k_bss_info_changed+0xeec/0x1000 [ath10k_core]
2019-02-15T08:49:00.909448-06:00 rabbit-hole kernel: [165755.448100] Modules linked in: uinput ccm cmac fuse rfcomm af_packet xt_tcpudp ip6t_rpfilter ip6t_REJECT nf_reject_ipv6 ipt_REJECT nf_reject_ipv4 xt_conntrack ebtable_nat ip6table_nat nf_nat_ipv6 ip6table_mangle ip6table_raw ip6table_security iptable_nat nf_nat_ipv4 hid_logitech_hidpp nf_nat iptable_mangle iptable_raw iptable_security nf_conntrack nf_defrag_ipv6 nf_defrag_ipv4 ip_set nfnetlink ebtable_filter ebtables ip6table_filter ip6_tables iptable_filter ip_tables x_tables bpfilter bnep btusb uvcvideo btrtl btbcm videobuf2_vmalloc btintel videobuf2_memops videobuf2_v4l2 bluetooth videodev videobuf2_common ecdh_generic cdc_acm arc4 hid_multitouch snd_hda_codec_hdmi msr iTCO_wdt iTCO_vendor_support intel_rapl x86_pkg_temp_thermal intel_powerclamp mei_wdt coretemp kvm_intel kvm irqbypass dell_laptop snd_hda_codec_realtek snd_hda_codec_generic snd_soc_skl snd_soc_hdac_hda snd_hda_ext_core snd_soc_skl_ipc snd_soc_sst_ipc snd_soc_sst_dsp snd_soc_acpi_intel_match snd_soc_acpi snd_soc_core
2019-02-15T08:49:00.909450-06:00 rabbit-hole kernel: [165755.448162]  crct10dif_pclmul ath10k_pci snd_compress crc32_pclmul snd_pcm_dmaengine ath10k_core snd_hda_intel ghash_clmulni_intel snd_hda_codec dell_wmi ath dell_smbios snd_hda_core dcdbas mac80211 snd_hwdep snd_pcm aesni_intel aes_x86_64 crypto_simd cryptd glue_helper idma64 snd_timer cfg80211 snd soundcore mei_me ucsi_acpi i2c_i801 wmi_bmof intel_wmi_thunderbolt rtsx_pci_ms typec_ucsi pcspkr intel_lpss_pci dell_wmi_descriptor joydev processor_thermal_device rfkill memstick mei intel_lpss intel_pch_thermal typec intel_soc_dts_iosf thermal battery pinctrl_sunrisepoint int3403_thermal pinctrl_intel intel_hid int3400_thermal acpi_thermal_rel int340x_thermal_zone sparse_keymap button acpi_pad ac pcc_cpufreq hid_logitech_dj hid_generic usbhid btrfs libcrc32c xor i915 rtsx_pci_sdmmc mmc_core raid6_pq i2c_algo_bit drm_kms_helper xhci_pci syscopyarea xhci_hcd sysfillrect sysimgblt fb_sys_fops crc32c_intel serio_raw drm usbcore rtsx_pci wmi i2c_hid video sg dm_multipath dm_mod scsi_dh_rdac
2019-02-15T08:49:00.909453-06:00 rabbit-hole kernel: [165755.448237]  scsi_dh_emc scsi_dh_alua
2019-02-15T08:49:00.909455-06:00 rabbit-hole kernel: [165755.448248] CPU: 1 PID: 23798 Comm: kworker/u16:33 Tainted: G        W         4.20.6-1-default #1 openSUSE Tumbleweed (unreleased)
2019-02-15T08:49:00.909456-06:00 rabbit-hole kernel: [165755.448250] Hardware name: Dell Inc. XPS 13 9370/0F6P3V, BIOS 1.4.0 05/25/2018
2019-02-15T08:49:00.909458-06:00 rabbit-hole kernel: [165755.448258] Workqueue: events_unbound async_run_entry_fn
2019-02-15T08:49:00.909460-06:00 rabbit-hole kernel: [165755.448272] RIP: 0010:ath10k_bss_info_changed+0xeec/0x1000 [ath10k_core]
2019-02-15T08:49:00.909462-06:00 rabbit-hole kernel: [165755.448276] Code: ff ff b8 40 00 00 00 e9 ed f4 ff ff 8b b5 70 01 00 00 89 f2 89 c1 48 c7 c6 b0 c7 c6 c0 4c 89 c7 e8 19 32 00 00 e9 0d fe ff ff <0f> 0b e9 c9 f2 ff ff 89 c2 48 c7 c6 20 c7 c6 c0 4c 89 cf 89 04 24
2019-02-15T08:49:00.909464-06:00 rabbit-hole kernel: [165755.448279] RSP: 0000:ffffa587843d7cc8 EFLAGS: 00010282
2019-02-15T08:49:00.909465-06:00 rabbit-hole kernel: [165755.448283] RAX: 00000000fffffffe RBX: ffff8cd9db171580 RCX: 0000000000000000
2019-02-15T08:49:00.909466-06:00 rabbit-hole kernel: [165755.448286] RDX: 0000000000000001 RSI: ffffa587843d7ce8 RDI: ffff8cd9ce5cd3a0
2019-02-15T08:49:00.909468-06:00 rabbit-hole kernel: [165755.448288] RBP: ffff8cd9ce5cd3a0 R08: 0000000000200000 R09: 0000000000000000
2019-02-15T08:49:00.909470-06:00 rabbit-hole kernel: [165755.448291] R10: 000000000000001f R11: ffff8cd9cfc98900 R12: 00000000020674ff
2019-02-15T08:49:00.909471-06:00 rabbit-hole kernel: [165755.448293] R13: ffff8cd9ce5cd3a8 R14: ffff8cd9db172558 R15: ffff8cd9db171580
2019-02-15T08:49:00.909472-06:00 rabbit-hole kernel: [165755.448297] FS:  0000000000000000(0000) GS:ffff8cd9de840000(0000) knlGS:0000000000000000
2019-02-15T08:49:00.909473-06:00 rabbit-hole kernel: [165755.448300] CS:  0010 DS: 0000 ES: 0000 CR0: 0000000080050033
2019-02-15T08:49:00.909474-06:00 rabbit-hole kernel: [165755.448303] CR2: 00007fd85664b030 CR3: 000000002620a006 CR4: 00000000003606e0
2019-02-15T08:49:00.909476-06:00 rabbit-hole kernel: [165755.448305] Call Trace:
2019-02-15T08:49:00.909478-06:00 rabbit-hole kernel: [165755.448324]  ? ath10k_conf_tx+0x6a/0x480 [ath10k_core]
2019-02-15T08:49:00.909480-06:00 rabbit-hole kernel: [165755.448365]  ieee80211_bss_info_change_notify+0xa8/0x1c0 [mac80211]
2019-02-15T08:49:00.909482-06:00 rabbit-hole kernel: [165755.448406]  ieee80211_reconfig+0x639/0x1120 [mac80211]
2019-02-15T08:49:00.909483-06:00 rabbit-hole kernel: [165755.448445]  wiphy_resume+0x7f/0x150 [cfg80211]
2019-02-15T08:49:00.909483-06:00 rabbit-hole kernel: [165755.448470]  ? addresses_show+0xa0/0xa0 [cfg80211]
2019-02-15T08:49:00.909485-06:00 rabbit-hole kernel: [165755.448477]  dpm_run_callback+0x59/0x180
2019-02-15T08:49:00.909487-06:00 rabbit-hole kernel: [165755.448484]  device_resume+0xbb/0x210
2019-02-15T08:49:00.909489-06:00 rabbit-hole kernel: [165755.448490]  ? dpm_show_time+0xd0/0xd0
2019-02-15T08:49:00.909490-06:00 rabbit-hole kernel: [165755.448495]  async_resume+0x19/0x30
2019-02-15T08:49:00.909492-06:00 rabbit-hole kernel: [165755.448500]  async_run_entry_fn+0x37/0x140
2019-02-15T08:49:00.909494-06:00 rabbit-hole kernel: [165755.448509]  process_one_work+0x1fd/0x420
2019-02-15T08:49:00.909496-06:00 rabbit-hole kernel: [165755.448517]  worker_thread+0x2d/0x3d0
2019-02-15T08:49:00.909497-06:00 rabbit-hole kernel: [165755.448525]  ? rescuer_thread+0x340/0x340
2019-02-15T08:49:00.909499-06:00 rabbit-hole kernel: [165755.448529]  kthread+0x116/0x130
2019-02-15T08:49:00.909501-06:00 rabbit-hole kernel: [165755.448535]  ? kthread_create_worker_on_cpu+0x40/0x40
2019-02-15T08:49:00.909503-06:00 rabbit-hole kernel: [165755.448542]  ret_from_fork+0x24/0x50
2019-02-15T08:49:00.909504-06:00 rabbit-hole kernel: [165755.448553] ---[ end trace 50dfa477b058b7ee ]---
2019-02-15T08:49:00.909505-06:00 rabbit-hole kernel: [165755.448592] WARNING: CPU: 1 PID: 23798 at drivers/net/wireless/ath/ath10k/mac.c:5688 ath10k_bss_info_changed+0xe47/0x1000 [ath10k_core]
2019-02-15T08:49:00.909506-06:00 rabbit-hole kernel: [165755.448594] Modules linked in: uinput ccm cmac fuse rfcomm af_packet xt_tcpudp ip6t_rpfilter ip6t_REJECT nf_reject_ipv6 ipt_REJECT nf_reject_ipv4 xt_conntrack ebtable_nat ip6table_nat nf_nat_ipv6 ip6table_mangle ip6table_raw ip6table_security iptable_nat nf_nat_ipv4 hid_logitech_hidpp nf_nat iptable_mangle iptable_raw iptable_security nf_conntrack nf_defrag_ipv6 nf_defrag_ipv4 ip_set nfnetlink ebtable_filter ebtables ip6table_filter ip6_tables iptable_filter ip_tables x_tables bpfilter bnep btusb uvcvideo btrtl btbcm videobuf2_vmalloc btintel videobuf2_memops videobuf2_v4l2 bluetooth videodev videobuf2_common ecdh_generic cdc_acm arc4 hid_multitouch snd_hda_codec_hdmi msr iTCO_wdt iTCO_vendor_support intel_rapl x86_pkg_temp_thermal intel_powerclamp mei_wdt coretemp kvm_intel kvm irqbypass dell_laptop snd_hda_codec_realtek snd_hda_codec_generic snd_soc_skl snd_soc_hdac_hda snd_hda_ext_core snd_soc_skl_ipc snd_soc_sst_ipc snd_soc_sst_dsp snd_soc_acpi_intel_match snd_soc_acpi snd_soc_core
2019-02-15T08:49:00.909509-06:00 rabbit-hole kernel: [165755.448648]  crct10dif_pclmul ath10k_pci snd_compress crc32_pclmul snd_pcm_dmaengine ath10k_core snd_hda_intel ghash_clmulni_intel snd_hda_codec dell_wmi ath dell_smbios snd_hda_core dcdbas mac80211 snd_hwdep snd_pcm aesni_intel aes_x86_64 crypto_simd cryptd glue_helper idma64 snd_timer cfg80211 snd soundcore mei_me ucsi_acpi i2c_i801 wmi_bmof intel_wmi_thunderbolt rtsx_pci_ms typec_ucsi pcspkr intel_lpss_pci dell_wmi_descriptor joydev processor_thermal_device rfkill memstick mei intel_lpss intel_pch_thermal typec intel_soc_dts_iosf thermal battery pinctrl_sunrisepoint int3403_thermal pinctrl_intel intel_hid int3400_thermal acpi_thermal_rel int340x_thermal_zone sparse_keymap button acpi_pad ac pcc_cpufreq hid_logitech_dj hid_generic usbhid btrfs libcrc32c xor i915 rtsx_pci_sdmmc mmc_core raid6_pq i2c_algo_bit drm_kms_helper xhci_pci syscopyarea xhci_hcd sysfillrect sysimgblt fb_sys_fops crc32c_intel serio_raw drm usbcore rtsx_pci wmi i2c_hid video sg dm_multipath dm_mod scsi_dh_rdac
2019-02-15T08:49:00.909511-06:00 rabbit-hole kernel: [165755.448708]  scsi_dh_emc scsi_dh_alua
2019-02-15T08:49:00.909512-06:00 rabbit-hole kernel: [165755.448715] CPU: 1 PID: 23798 Comm: kworker/u16:33 Tainted: G        W         4.20.6-1-default #1 openSUSE Tumbleweed (unreleased)
2019-02-15T08:49:00.909514-06:00 rabbit-hole kernel: [165755.448717] Hardware name: Dell Inc. XPS 13 9370/0F6P3V, BIOS 1.4.0 05/25/2018
2019-02-15T08:49:00.909516-06:00 rabbit-hole kernel: [165755.448721] Workqueue: events_unbound async_run_entry_fn
2019-02-15T08:49:00.909518-06:00 rabbit-hole kernel: [165755.448734] RIP: 0010:ath10k_bss_info_changed+0xe47/0x1000 [ath10k_core]
2019-02-15T08:49:00.909520-06:00 rabbit-hole kernel: [165755.448738] Code: 00 00 e8 6c 56 c3 d9 e9 0c fc ff ff 8b b5 70 01 00 00 89 f2 89 c1 48 c7 c6 33 09 c7 c0 4c 89 ff e8 be 32 00 00 e9 2a fe ff ff <0f> 0b 4c 89 f7 e8 0f 25 c4 d9 e9 2a f4 ff ff 49 8b 91 98 03 00 00
2019-02-15T08:49:00.909521-06:00 rabbit-hole kernel: [165755.448740] RSP: 0000:ffffa587843d7cc8 EFLAGS: 00010282
2019-02-15T08:49:00.909523-06:00 rabbit-hole kernel: [165755.448743] RAX: 00000000fffffffe RBX: ffff8cd9db171580 RCX: 0000000000000000
2019-02-15T08:49:00.909525-06:00 rabbit-hole kernel: [165755.448746] RDX: 0000000000000001 RSI: ffffa587843d7ce8 RDI: ffff8cd9ce5cd3a0
2019-02-15T08:49:00.909565-06:00 rabbit-hole kernel: [165755.448748] RBP: ffff8cd9ce5cd3a0 R08: 0000000000200000 R09: 0000000000000000
2019-02-15T08:49:00.909568-06:00 rabbit-hole kernel: [165755.448751] R10: 000000000000001f R11: ffff8cd9cfc98900 R12: 0000000000000020
2019-02-15T08:49:00.909569-06:00 rabbit-hole kernel: [165755.448753] R13: ffff8cd9ce5cd3a8 R14: ffff8cd9db172558 R15: ffff8cd9db171580
2019-02-15T08:49:00.909570-06:00 rabbit-hole kernel: [165755.448757] FS:  0000000000000000(0000) GS:ffff8cd9de840000(0000) knlGS:0000000000000000
2019-02-15T08:49:00.909571-06:00 rabbit-hole kernel: [165755.448759] CS:  0010 DS: 0000 ES: 0000 CR0: 0000000080050033
2019-02-15T08:49:00.909573-06:00 rabbit-hole kernel: [165755.448762] CR2: 00007fd85664b030 CR3: 000000002620a006 CR4: 00000000003606e0
2019-02-15T08:49:00.909575-06:00 rabbit-hole kernel: [165755.448764] Call Trace:
2019-02-15T08:49:00.909576-06:00 rabbit-hole kernel: [165755.448777]  ? ath10k_conf_tx+0x6a/0x480 [ath10k_core]
2019-02-15T08:49:00.909578-06:00 rabbit-hole kernel: [165755.448809]  ieee80211_bss_info_change_notify+0xa8/0x1c0 [mac80211]
2019-02-15T08:49:00.909579-06:00 rabbit-hole kernel: [165755.448847]  ieee80211_reconfig+0x639/0x1120 [mac80211]
2019-02-15T08:49:00.909580-06:00 rabbit-hole kernel: [165755.448878]  wiphy_resume+0x7f/0x150 [cfg80211]
2019-02-15T08:49:00.909582-06:00 rabbit-hole kernel: [165755.448902]  ? addresses_show+0xa0/0xa0 [cfg80211]
2019-02-15T08:49:00.909584-06:00 rabbit-hole kernel: [165755.448907]  dpm_run_callback+0x59/0x180
2019-02-15T08:49:00.909586-06:00 rabbit-hole kernel: [165755.448913]  device_resume+0xbb/0x210
2019-02-15T08:49:00.909587-06:00 rabbit-hole kernel: [165755.448919]  ? dpm_show_time+0xd0/0xd0
2019-02-15T08:49:00.909588-06:00 rabbit-hole kernel: [165755.448924]  async_resume+0x19/0x30
2019-02-15T08:49:00.909590-06:00 rabbit-hole kernel: [165755.448929]  async_run_entry_fn+0x37/0x140
2019-02-15T08:49:00.909592-06:00 rabbit-hole kernel: [165755.448936]  process_one_work+0x1fd/0x420
2019-02-15T08:49:00.909594-06:00 rabbit-hole kernel: [165755.448944]  worker_thread+0x2d/0x3d0
2019-02-15T08:49:00.909595-06:00 rabbit-hole kernel: [165755.448951]  ? rescuer_thread+0x340/0x340
2019-02-15T08:49:00.909597-06:00 rabbit-hole kernel: [165755.448956]  kthread+0x116/0x130
2019-02-15T08:49:00.909599-06:00 rabbit-hole kernel: [165755.448961]  ? kthread_create_worker_on_cpu+0x40/0x40
2019-02-15T08:49:00.909600-06:00 rabbit-hole kernel: [165755.448966]  ret_from_fork+0x24/0x50
2019-02-15T08:49:00.909601-06:00 rabbit-hole kernel: [165755.448976] ---[ end trace 50dfa477b058b7ef ]---
2019-02-15T08:49:00.909602-06:00 rabbit-hole kernel: [165755.454206] OOM killer enabled.
2019-02-15T08:49:00.916488-06:00 rabbit-hole systemd-logind[1318]: Lid opened.
2019-02-15T08:49:00.927873-06:00 rabbit-hole kernel: [165755.454207] Restarting tasks ... done.
2019-02-15T08:49:00.952222-06:00 rabbit-hole systemd[1]: Starting Check if mainboard battery is Ok...
2019-02-15T08:49:00.960649-06:00 rabbit-hole systemd[1]: Started Timeline of Snapper Snapshots.
2019-02-15T08:49:00.972970-06:00 rabbit-hole systemd[1]: Started Check if mainboard battery is Ok.
2019-02-15T08:49:00.975720-06:00 rabbit-hole dbus-daemon[1269]: [system] Activating service name='org.opensuse.Snapper' requested by ':1.444' (uid=0 pid=23874 comm="/usr/lib/snapper/systemd-helper --timeline ") (using servicehelper)
2019-02-15T08:49:01.007731-06:00 rabbit-hole dbus-daemon[1269]: [system] Successfully activated service 'org.opensuse.Snapper'
2019-02-15T08:49:01.013805-06:00 rabbit-hole kscreenlocker_greet[23756]: qt.virtualkeyboard.hunspell: Hunspell dictionary is missing for "en_GB" . Search paths ("/usr/share/qt5/qtvirtualkeyboard/hunspell", "/usr/share/hunspell", "/usr/share/myspell/dicts")
2019-02-15T08:49:01.061301-06:00 rabbit-hole systemd-sleep[23771]: System resumed.
2019-02-15T08:49:01.063871-06:00 rabbit-hole kernel: [165755.605865] PM: suspend exit
2019-02-15T08:49:01.073697-06:00 rabbit-hole systemd-sleep[23771]: INFO: Skip running /usr/lib/systemd/system-sleep/grub2.sleep for suspend
2019-02-15T08:49:01.077038-06:00 rabbit-hole systemd[1]: Started Suspend.
2019-02-15T08:49:01.077331-06:00 rabbit-hole systemd[1]: sleep.target: Unit not needed anymore. Stopping.
2019-02-15T08:49:01.077990-06:00 rabbit-hole systemd[1]: Stopped target Sleep.
2019-02-15T08:49:01.078229-06:00 rabbit-hole systemd[1]: Reached target Suspend.
2019-02-15T08:49:01.078461-06:00 rabbit-hole systemd[1]: suspend.target: Unit not needed anymore. Stopping.
2019-02-15T08:49:01.078670-06:00 rabbit-hole systemd[1]: Stopped target Suspend.$
2019-02-15T08:49:01.080024-06:00 rabbit-hole systemd-logind[1318]: Operation 'sleep' finished.
2019-02-15T08:49:01.087489-06:00 rabbit-hole kdeinit5[2131]: bluedevil: About to resume
```

3) JournalCTL - I seem to be missing a day here

```
Feb 13 10:46:27 rabbit-hole kernel: check: Scanning 1 areas for low memory corruption
...skipping...
Feb 15 09:27:07 rabbit-hole plasmashell[2173]: qt.qpa.xcb: QXcbConnection: XCB error: 2

```