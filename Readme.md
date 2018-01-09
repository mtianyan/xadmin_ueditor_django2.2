# xadmin_django2.0.1

[![Build Status](https://travis-ci.org/mtianyan/hexoBlog-Github.svg?branch=master)](https://travis-ci.org/mtianyan/hexoBlog-Github)

基于原版 for Django 2.0版本分支修改部分bug：

- 只修改bug, 以及必要改动。个人项目自用, 亲测Python3.5+django2.0.1运行正常

## bug汇总(也可通过commit记录查看已修复bug):

- IndexError(已解决)

```
list index out of range
```

>解决方案基于: https://github.com/sshwsfc/xadmin/issues/499

- 导出csv中文乱码(已解决)

>解决方案: 修改xadmin/plugins/export.py(大约221行)get_response中charset改为gbk

```
content_type="%s; charset=gbk" % self.export_mimes[file_type])
```


