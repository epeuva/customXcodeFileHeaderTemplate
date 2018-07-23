
# Custom Xcode file header template

## Introduction

Custom Xcode 9+ file header template in order to be able to personalize the full username (author) on file creation.

Based on: <https://oleb.net/blog/2017/07/xcode-9-text-macros/#text-macros-reference>

You can also search "Customize text macros" in Xcode Help section for more official info.

## Instructions

 1. Download __IDETemplateMacros.plist__ file (or create a new one, see the link above)

 2. Copy the __IDETemplateMacros.plist__ on one of the following locations:

      * Project user data: _\<ProjectName\>.xcodeproj/xcuserdata/[username].xcuserdatad/IDETemplateMacros.plist._
      * Project shared data: _\<ProjectName\>.xcodeproj/xcshareddata/IDETemplateMacros.plist_
      * Workspace user data: _\<WorkspaceName\>.xcworkspace/xcuserdata/[username].xcuserdatad/IDETemplateMacros.plist._
      * Workspace shared data: _\<WorkspaceName\>.xcworkspace/xcshareddata/IDETemplateMacros.plist._
      * User Xcode data: _~/Library/Developer/Xcode/UserData/IDETemplateMacros.plist._

 3. Edit _CUSTOMFULLUSERNAME_ variable

 4. Restart Xcode and create a new file with the new header

For this example, the file has been copied to User Xcode data. _~/Library/Developer/Xcode/UserData/IDETemplateMacros.plist._

## Example

The following template, when _CUSTOMFULLUSERNAME_ = _"epeuva"_

```text

//  ___FILENAME___
//  ___PRODUCTNAME___
//
//  Created by ___CUSTOMFULLUSERNAME___ on ___DATE___
//  ___COPYRIGHT___
//
```

generates:

```text
//
//  ViewController.h
//  exampleProject
//
//  Created by epeuva on 23/07/2018.
//  Copyright © 2018 epeuva. All rights reserved.
//
```