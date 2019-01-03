# Pre-work - *Name of App Here*

**tippy** is a tip calculator application for iOS.

Submitted by: **Huanjia Liang**

Time spent: **4** hours spent in total

## User Stories

The following **required** functionality is complete:

* [ X ] User can enter a bill amount, choose a tip percentage, and see the tip and total values.

The following **optional** features are implemented:
* [ ] Settings page to change the default tip percentage.
* [ ] UI animations
* [ ] Remembering the bill amount across app restarts (if <10mins)
* [ ] Using locale-specific currency and currency thousands separators.
* [ ] Making sure the keyboard is always visible and the bill amount is always the first responder. This way the user doesn't have to tap anywhere to use this app. Just launch the app and start typing.

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app functionality!

## Video Walkthrough 

Here's a walkthrough of implemented user stories:

<img src='https://github.com/lianghuanjia/tippy/blob/master/tippyCalculation.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

GIF created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

So when I was building this app, I encountered a couple of problems.

First is I linked the Bill label to the code and make it as variable billField, but the thing is I should link the bill field as billField. Then I delete the variable in the code, but I didn't delete the connection to the Bill label, therefore I can run the simulator because there is an error. After that, I google online and figured out that in terms of deleting a thing in the code that is connected to the main.storyboard, I should right click the thing in the main story board and delete their connection.

Another problem is the number in my Tip and Total initially they only should around 4 digits. If I have more digits they will just show the first 4 and the rest will be substituted as ellipsis. Then I extend the label's length, and in their text field, I set the alignment as right, then the number will stick to the right side and extend to left if there are more digits,  and all the digits will show. 

Finally is the keyboard. Somehow when I was testing my app, the digit keyboard only appears once. After that, if I click my bill field, the keyboard doesn't show up, and I can only use my computer's keyboard to enter the number. To fix this problem, I ran over the part of setting the keyboard, and finally it works well.

## License

Copyright [2019] [Huanjia Liang]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
