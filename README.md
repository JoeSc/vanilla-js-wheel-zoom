# vanilla-js-wheel-zoom

Image resizing using mouse wheel + drag scrollable image

```
<html>
<head>
    <meta http-equiv="Content-type" content="text/html; charset=utf-8">

    <script src="wheel-zoom.js"></script>
</head>
<body>
    <div style="width:600px;height:600px">
        <img src="https://placehold.it/1200x700" />
    </div>
    
    <script>
        document.addEventListener('DOMContentLoaded', function () {
            jcWheelZoom = JcWheelZoom.create('img', {
                prepare: function (scale, correct_x, correct_y) {
                    // do smth when image prepared
                },
                rescale: function (scale, correct_x, correct_y) {
                    // do smth when image rescaled
                }
            });
        });
    </script>
</body>
</html>
```

Default params

```
var defaults = {
    dragscrollable: true,
    speed: 10
};
```
