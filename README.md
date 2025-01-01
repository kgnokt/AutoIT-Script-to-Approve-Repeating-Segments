Global $toggle = False

HotKeySet("*", "ToggleScript")

Func ToggleScript()
    $toggle = Not $toggle
    While $toggle
        Send("^{ENTER}")    ; Sends Ctrl+Enter simultaneously
        Sleep(1700)          ; Adjust this delay as needed
        Send("{DOWN}")      ; Press Down Arrow
        Sleep(1700)          ; Adjust this delay as needed
		Send("^{ENTER}")    ; Sends Ctrl+Enter simultaneously
        Sleep(1700)          ; Adjust this delay as needed
    WEnd
EndFunc

; Keep script running
While 1
    Sleep(1700)
WEnd
