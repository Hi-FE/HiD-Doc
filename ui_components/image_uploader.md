## image-uploader

<img src="http://77fkpo.com5.z0.glb.clouddn.com/8b4d7e9c48a732d4429b53bf6e4b2039.png" width="400"></img>

image-uploader是一种图片上传的组件，它的内容由一个当前图片、一个进度条、一个标题（包含最小尺寸）和一个遮罩组成。

``` html
  <image-uploader name="banner_m" title="Banner for Mobile"
                  min_width="828" min_height="621"
                  image_url="{{ promotion.mobile_image }}"
                  change-image-url="{{ setPromotionImageForMobile }}"></image-uploader>
```

  - **name** `string` 上传组件所需ID，必须且唯一。
  - **title** `string` 所上传图片说明，必须。
  - **min_width** `number` 图片要求最小宽度，必须。
  - **min_height** `number` 图片要求最小高度，必须。
  - **image_url** `string` 图片URL，必须。
  - **change-image-url** `function` 更新当前展示图片，必须。

> 目前只限制图片最小尺寸。<br>
> 目前限制图片大小不可以超过1M。<br>
> 目前限制可上传文件格式为jpg,gif,png。