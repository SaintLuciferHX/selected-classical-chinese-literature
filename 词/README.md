# 说明
此文件夹存放体裁为词（广义）的json文件。

# 数据形式
文件名为ci.json，只记录词名，词牌名，内容，作者名和词的哈希值（用于检测是否重复，哈希函数输入为词牌名+词名+作者+词前两句，不包括标点。例如《虞美人》的输入为"虞美人李煜春花秋月何时了往事知多少"）。文件格式如下：

```text
[
    {
        "title": "虞美人",
        "author": "李李煜白",
        "paragraphs": [
            "春花秋月何时了，往事知多少。",
            "小楼昨夜又东风，故国不堪回首月明中。",
            "雕阑玉砌应犹在，只是朱颜改。",
            "问君能有几多愁，恰是一江春水向东流。"
        ],
        "hash": "1236f1243ec2c55cffa49bb2d73bb486"
    }
]
```
注意，如果既有词名又有词牌名，标题应用·符号隔开，词牌名在前，词名在后。

# 编辑方法
你可以直接编辑此文件夹下的json文件，但请一定按照格式来写。

你也可以使用此文件加下的py脚本来编辑。使用方法很简单，我相信如果你能打开github看到这个一定会使用它。实在不会就给此邮箱发邮件linfyedu@gmail.com。