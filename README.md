
## Reproduction Steps:

  1. Clone the repo  
  2. Move to the folder RuntimeTest/DrtTests
  3.  Run command  '.\Build.cmd'
  4.  Move to the test folder 'cd .\publish\Debug\x86\Test\'
  5.  Run the test

.\RunDrts.cmd /name=[NAME]
[NAME] :  drtwindowscroll or drtwindowfunctionality


## DrtTests
### DRT Window Scroll: 
In this DRT, we focus on validating the behavior of the ScrollViewer control within the context of a Page's style.
 The test scenario involves the following application structure:
Window -> Page -> ScrollViewer -> Rectangle (figure)
To accomplish this, we attach an event handler (OnLoaded) to the Page. When the Page is loaded, this event handler triggers multiple tests to verify the behavior of the content presenter and the visibility of the scroll bar. These tests are conducted with different content sizes, ensuring comprehensive coverage.

### DRT Window Functionality:
We aim to validate different functionalities and behaviors of the Window control and test that setting visibility is async.
In this test, we have verified the size and visibility of content in various situation where we changed the size, position and state of the window (Normal, minimized, maximized).!
