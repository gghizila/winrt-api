---
-api-id: T:Windows.UI.Core.CharacterReceivedEventArgs
-api-type: winrt class
---

<!-- Class syntax.
public class CharacterReceivedEventArgs : Windows.UI.Core.ICharacterReceivedEventArgs, Windows.UI.Core.ICoreWindowEventArgs
-->

# Windows.UI.Core.CharacterReceivedEventArgs

## -description
Provides the arguments returned by the event raised when a character is received by the input queue.

## -remarks


> **Windows 10**
> Apps do not receive this event when an [](http://msdn.microsoft.com/library/5fcc73e6-f499-47e6-8e81-0014ca4d241c) is enabled. The Input Method Editor (IME) handles all keyboard input and sets [Handled](acceleratorkeyeventargs_handled.md) to **true**.



> **Windows Phone**
> This API is supported in native apps only.

This object is returned by a delegate registered for the following event:
+ [CoreWindow.CharacterReceived](corewindow_characterreceived.md)




```cpp

// returning character received events data through CharacterReceivedEventArgs

void MyCoreWindowEvents::SetWindow( // implementation called by CoreApplication::Run(), provided for context
    _In_ CoreWindow^ window
    )
{
   
    // ...
    window->CharacterReceived +=
        ref new TypedEventHandler<CoreWindow^, CharacterReceivedEventArgs^>(this, &CoreWindowEvents::OnCharacterReceived);

    // ...
   
}

```



> [!NOTE]
> : This class is not agile, which means that you need to consider its threading model and marshaling behavior. For more info, see [Threading and Marshaling (C++/CX)](http://go.microsoft.com/fwlink/p/?linkid=258275).

## -examples

## -see-also
[CharacterReceived](corewindow_characterreceived.md)