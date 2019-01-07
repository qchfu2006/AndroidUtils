# AndroidUtils
记录Android各个小工具：零散的代码文件
==========================================
【1】 获取处于焦点的控件的ID：
View rootview = DetailActivity.this.getWindow().getDecorView();
View focusView = rootview.findFocus();
Log.i("QQ","The View which obtains the focus is :"+focusView.getId());
