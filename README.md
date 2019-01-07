# AndroidUtils
记录Android各个小工具：零散的代码文件
==========================================
【1】 获取处于焦点的控件的ID：
View rootview = DetailActivity.this.getWindow().getDecorView();
View focusView = rootview.findFocus();
Log.i("QQ","The View which obtains the focus is :"+focusView.getId());
【2】 Android下Sqlite数据导入和导出： 通过adb 找到db文件，然后输入下面的命令：
SQLITE3 STUDENT.DB < student.sql //从student.sql文件提取数据导入并创建student.db
SQLITE3 STUDENT.DB .dump > student_result.sql  //从student.db导出数据并创建student_result.sql
