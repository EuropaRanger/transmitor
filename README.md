# transmitor
qt.qpa.plugin: Could not find the Qt platform plugin "qt5ct" in ""
This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.

Available platform plugins are: eglfs, linuxfb, minimal, minimalegl, offscreen, vnc, xcb.

*** Aborted at 1747908970 (unix time) try "date -d @1747908970" if you are using GNU date ***
PC: @     0x7fa1c829500b gsignal
*** SIGABRT (@0x3ea00002b9d) received by PID 11165 (TID 0x7fa1c3abd900) from PID 11165; stack trace: ***
    @     0x7fa1c9ed4631 (unknown)
    @     0x7fa1c9417420 (unknown)
    @     0x7fa1c829500b gsignal
    @     0x7fa1c8274859 abort
    @     0x7fa1c88aaaad QMessageLogger::fatal()
    @     0x7fa1c8e8c7ae QGuiApplicationPrivate::createPlatformIntegration()
    @     0x7fa1c8e8d708 QGuiApplicationPrivate::createEventDispatcher()
    @     0x7fa1c8ab1f55 QCoreApplicationPrivate::init()
    @     0x7fa1c8e8f543 QGuiApplicationPrivate::init()
    @     0x7fa1c95993bd QApplicationPrivate::init()
    @     0x55f4d27d9dcc RunGraphicalUserInterface()
    @     0x55f4d27c4eaf main
    @     0x7fa1c8276083 __libc_start_main
    @     0x55f4d27c8f6e _start
已放弃 (核心已转储)

