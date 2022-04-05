# WinClose
Global $aData = _WinAPI_EnumProcessWindows($H_au3, False)                 SciTE_SendConsoleMessage("> Trying normal script close by Sending WinClose to all Windows of Pid " &amp; $H_au3)                 If IsArray($aData) Then                     For $x = 1 To $aData[0][0]                         WinClose($aData[$x][0])                     Next                 EndIf
