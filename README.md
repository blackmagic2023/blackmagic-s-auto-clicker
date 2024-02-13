# blackmagic-s-auto-clicker
just a simple auto-clicker for windows

# Images

![ac](https://github.com/francalzado/TFG-final/assets/149164084/18716c1c-cbaa-473d-96f1-1c13d9c9ef06)

# Making Changes

Open the AutoClicker.rar file to see the project file. Open the project in Visual Studio.

-To change the interval of the delay you must:
locate the timer named "StartDelay" and change the `interval` property according to your need's, the interval is defined in milliseconds so 5000 milliseconds would be 5 seconds.

-To change the start/stop key you must:
Double click on the Form to access the code. On line 8 `Private Const VK_F6 As Integer = &H75` you must change the `VK_F6` and `&H75` to corrospond with the key you would like to use. In addition to that change you must also locate line 39 `If struct.vkCode = VK_F6 Then` and you must change the `VK_F6` I also suggest changing the text for the button you can do this by locating lines 70 - 76 and change the 'F6' to match the key you set!
```
        If StartClcikBtn.Text = "Start (F6)" Then
            StartDelay.Start()
            StartClcikBtn.Text = "Stop (F6)"
        Else
            IntervalTimer.Stop()
            StartClcikBtn.Text = "Start (F6)"
        End If
```
