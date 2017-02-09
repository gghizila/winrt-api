---
-api-id: T:Windows.UI.Xaml.Media.Animation.AddDeleteThemeTransition
-api-type: winrt class
---

<!-- Class syntax.
public class AddDeleteThemeTransition : Windows.UI.Xaml.Media.Animation.Transition, Windows.UI.Xaml.Media.Animation.IAddDeleteThemeTransition
-->

# Windows.UI.Xaml.Media.Animation.AddDeleteThemeTransition

## -description
Provides the animated transition behavior for when controls add or delete children of a panel. For example, if you have a collection of photos displayed in a [Grid](../windows.ui.xaml.controls/grid.md), you can associate this animation to the [Grid](../windows.ui.xaml.controls/grid.md) so that when photos are added or deleted, the photos will animate in and out of view.

## -xaml-syntax
```xaml
<AddDeleteThemeTransition .../>
```


## -remarks

## -examples
The following example shows how to use the [AddDeleteThemeTransition](adddeletethemetransition.md) to animate rectangles as they are added and deleted from a panel. Notice how the other child elements of the panel re-flow when one of them is removed.


<!--  
      <p xml:space="preserve">
            <TRANSLATE_MANUALLY>
              <externalLink xmlns="http://ddue.schemas.microsoft.com/authoring/2003/5">
                <linkText>Run this sample</linkText>
                <linkUri>http://go.microsoft.com/fwlink/p/?linkid=139798&amp;sref=BackEase_scale</linkUri>
              </externalLink>
            </TRANSLATE_MANUALLY>
          </p>-->



[!code-xml[AddDeleteThemeTransition](../windows.ui.xaml.media.animation/code/AddDeleteThemeTransition/csharp/BlankPage.xaml#SnippetAddDeleteThemeTransition)]

[!code-cs[AddDeleteThemeTransition_code](../windows.ui.xaml.media.animation/code/AddDeleteThemeTransition/csharp/BlankPage.xaml.cs#SnippetAddDeleteThemeTransition_code)]

## -see-also
[Transition](transition.md), [Animating list additions and deletions](http://msdn.microsoft.com/library/3317d9c5-9936-42ec-bdeb-4df538374232), [Guidelines and checklist for add and delete animations](http://msdn.microsoft.com/library/a85006ae-4992-457a-b514-500b8bef5dc8)