<img width="1120" alt="image" src="https://github.com/user-attachments/assets/899d322f-7f25-4999-8694-ee498daef335">

# rsse
阿里云盘、夸克云盘等云盘搜索引擎

# 如何使用？
```
模糊查询:
    完美世界
精准:
    +"完美世界"
找"完美世界"的第 166 集：
    +"完美世界" +name:"166"
专业搜索 精准搜索、匹配的 2024-06-06 更新的 "完美世界" 第 166 集，且高清 大于 1Gib(1073741824) 的视频资源:
    +type:file +category:video +mime_type:video +size:>1073741824 +"video_media_metadata.width":>1024 +created_at:>="2024-06-06" +tags:"完美世界" +name:"166"

排除，例如搜索今天更新，排除"完美世界"：
    +created_at:>="2024-06-06" -:"完美世界"

匹配视频：
    +category:video +mime_type:vide
匹配视频宽度：
    +"video_media_metadata.width":>1024
匹配文件大小（字节）：
    +size:>1073741824

搜索大于1GiB的文件:
    +size:>1073741824

搜索大于 50 GiB 的文件:
    +size:>=53687091200

禁止：
    1、禁止查询超过 7 天数据，避免命中太多导致服务器压力
    2、禁止没有输入关键词，也没有限定7天内的查询

```
