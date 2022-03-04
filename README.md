
## LoadingDrawable: Android cool animation collection
[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-LoadingDrawable-brightgreen.svg?style=flat)](http://android-arsenal.com/details/1/3450)

 LoadingDrawable is some android animations implement of drawable: a library can be used in the pull-down to refresh, the placeholders of image loading and the time-consuming tasks. 
 
The following content show a brief overview of LoadingDrawable

* It extends `Drawable` and implement the interface `Animatable`
* it uses strategy mode
* It can be used as the background of View or content of `ImageView`
* It's constructor must be passed a `LoadingRenderer`
* It interact with `LoadingRenderer` by the callback `Callback`
* `LoadingRenderer` is used for measuring and drawing the `LoadingDrawable`. note:
`LoadingRenderer` is the core
* `LoadingRenderer` only can be created by their `Builder`. 
 
Learn more about LoadingDrawable on the [Wiki Home](https://github.com/dinuscxj/LoadingDrawable/wiki).

![](https://raw.githubusercontent.com/dinuscxj/LoadingDrawable/master/Preview/ShapeChangeDrawable.gif)
![](https://raw.githubusercontent.com/dinuscxj/LoadingDrawable/master/Preview/GoodsDrawable.gif)
![](https://raw.githubusercontent.com/dinuscxj/LoadingDrawable/master/Preview/AnimalDrawable.gif)
![](https://raw.githubusercontent.com/dinuscxj/LoadingDrawable/master/Preview/SceneryDrawable.gif)
![](https://raw.githubusercontent.com/dinuscxj/LoadingDrawable/master/Preview/CircleJumpDrawable.gif)
![](https://raw.githubusercontent.com/dinuscxj/LoadingDrawable/master/Preview/CircleRotateDrawable.gif)

## LoadingRenderer Style

#### ShapeChange
 * CircleBroodLoadingRenderer
 * CoolWaitLoadingRenderer

#### Goods
 * BalloonLoadingRenderer
 * WaterBottleLoadingRenderer

#### Animal
 * FishLoadingRenderer
 * GhostsEyeLoadingEyeRenderer

#### Scenery
 * ElectricFanLoadingRenderer
 * DayNightLoadingRenderer

#### Circle Jump
 * CollisionLoadingRenderer
 * SwapLoadingRenderer
 * GuardLoadingRenderer
 * DanceLoadingRenderer

#### Circle Rotate
 * WhorlLoadingRenderer
 * MaterialLoadingRenderer
 * GearLoadingRenderer
 * LevelLoadingRenderer

## Usage
 Define the `LoadingView` in XML and specify the `LoadingRenderer` style:
 ```xml
 <app.dinus.com.loadingdrawable.LoadingView
    android:id="@+id/level_view"
    android:layout_width="0dp"
    android:layout_height="match_parent"
    android:layout_weight="1"
    android:background="#fff1c02e"
    app:loading_renderer="LevelLoadingRenderer"/>
  ```
 Or specify the `LoadingRenderer` style in Java
 ```java
 ***LoadingRenderer.Builder builder = new ***LoadingRenderer.Builder(context);
 LoadingView.setLoadingRenderer(builder.build());
 ```
 
## TODO
 When I feel less bugs enough, I will add a gradle dependency. So I hope you will make more Suggestions or Issues.

## Misc
 If you like LoadingDrawable or use it, could you please:

 * star this repo
 * send me some feedback. Thanks!


## License
    Copyright 2015-2019 dinus

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
