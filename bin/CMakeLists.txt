cmake_minimum_required(VERSION 3.0)

set(OPALKELLYFRONTPANAL_SRC       )
set(OPALKELLYFRONTPANAL_HEADERS   )
set(OPALKELLYFRONTPANAL_LIBS      )
set(OPALKELLYFRONTPANAL_BINS
        fpoip-passwd
        fpoip-server
        AsyncTriggerEx
        BusEventsEx
        CustomImageEx
        ExtendedShutterEx
        FlyCap2.glade
        FlyCap2_arm
        FlyCapture2GUI_GTK.glade
        FlyCapture2Test
        GigEGrabEx
        GrabCallbackEx
        HighDynamicRangeEx
        ImageEventEx
        MultipleCameraEx
        )



install (FILES ${OPALKELLYFRONTPANAL_SRC}  DESTINATION include )
install (FILES  ${OPALKELLYFRONTPANAL_HEADERS}  DESTINATION include )
install (FILES ${OPALKELLYFRONTPANAL_LIBS}  DESTINATION lib )
install (FILES ${OPALKELLYFRONTPANAL_BINS}  DESTINATION bin )

add_subdirectory(C)
