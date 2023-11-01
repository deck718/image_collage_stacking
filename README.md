# image_collage_stacking
这个代码库提供了一个Python工具，用于将多张图片进行拼接和层叠操作。它使用常见的图像处理库和算法，允许用户在不同的布局和风格下创建各种图片拼贴效果。
from image_collage_stacking import ImageCollage

# 创建图片拼贴对象
collage = ImageCollage()

# 添加图片
collage.add_image("image1.jpg")
collage.add_image("image2.jpg")
collage.add_image("image3.jpg")

# 设置布局方式
collage.set_layout("grid", rows=2, columns=2)

# 设置边框和间距
collage.set_border_size(10)
collage.set_padding(5)

# 生成拼贴图片
result_image = collage.generate_collage()

# 保存拼贴图片
result_image.save("collage.jpg")
