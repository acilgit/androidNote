# androidNote
我的安卓笔记
android notes
终于有时间可以开始写下日常的笔记了

2016-04-24
 -- keyword --
（1）使用transient关键字时，保存实例序列化后再取回时，实例并不会再被创建一次，而是直接读取到原来状态，而transient的字段将会返回null。

 -- AS --
（1）AS2.0开始Debug时不再需要每次都重Build项目，但有小数情况在崩溃后要重装App时，可能再Build的时候会出现无法删除Buil目录的问题，这时候最好退出AS然后删除项目下的Build目录即可。如果觉得麻烦，要以下载LockHunter，并在项目中的build.gradle文件中添加Clear项目的操作：
task clean(type: Delete) {
    delete rootProject.buildDir
}

 -- Manifest -- 
（1）如无需要，不要添加硬件加速功能，这会使很多控件会出现显示问题，但如要使用，请在不需要加速的地方上添加独立关闭加速。

