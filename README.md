Cropper
=======
定制：

1. 调整gradleVersion至2.3，com.android.tools.build:gradle:1.3.0
2. 增加是否启用裁剪的选项，不启用时不显示裁剪浮层，调裁剪接口直接返回原图
3. 修改裁剪框边线颜色（减淡），并将裁剪框显示向内缩了1/2线宽，避免拖动到边缘时边框线被吃掉一半
4. 修改裁剪框四角样式，不超出图片范围
5. 降低自动吸图像边界灵敏度
6. 修改最小选取框限制为80dp，并支持使用dp单位
7. 修正几处注释警告

----
The Cropper is an image cropping tool. It provides a way to set an image in XML and programmatically, and displays a resizable crop window on top of the image. Calling the method getCroppedImage() will then return the Bitmap marked by the crop window.

Developers can customize the following attributes (both via XML and programmatically):

- appearance of guidelines in the crop window
- whether the aspect ratio is fixed or not
- aspect ratio (if the aspect ratio is fixed)
- image resource

A public method to rotate the image by a specified number of degrees is also included. This can be used to provide the user with an option to fix the image orientation should Android miscalculate the intended orientation.

Supported on API Level 7 and above.

For more information, see the linked Github Wiki page. 

https://github.com/edmodo/cropper/wiki

![ScreenShot](http://i.imgur.com/3FhsTgfl.jpg)

Installation
=======

**build.gradle**

	repositories {
		mavenCentral()
	}

	dependencies {
	  compile 'com.edmodo:cropper:1.0.1'
	}

License
=======
Copyright 2013, Edmodo, Inc. 

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this work except in compliance with the License.
You may obtain a copy of the License in the LICENSE file, or at:

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

Contributions
=======

We'd love for you to participate in the development of our project. Before we can accept your pull request, please sign our Individual Contributor License Agreement. It's a short form that covers our bases and makes sure you're eligible to contribute. Thank you!

http://goo.gl/gfj6Mb
