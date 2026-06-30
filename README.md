# LessonManagedSystem

基于 Java Swing 的课程管理系统

## 功能特性

- **课程管理**: 添加、删除、修改课程信息
- **搜索功能**: 支持按任意字段搜索课程（课程名、编号、类别、年级、教师姓名）
- **筛选功能**: 按年级和课程类别筛选课程
- **数据持久化**: 课程数据存储在文本文件中

## 技术栈

- Java
- Swing (GUI 框架)

## 项目结构

```
src/
  |- Main.java              # 程序入口
  |- edu/
     |- neuq/
        |- Class/
        |  |- start.java    # 主控制器，处理数据加载和保存
        |  |- Lesson.java   # 课程数据模型
        |  |- Cla.java      # 单个课程实体
        |- Handler/
        |  |- MainAction.java    # 主菜单动作处理
        |  |- MainAction01.java  # 类型筛选处理
        |  |- MainAction02.java  # 年级筛选处理
        |  |- addAction.java    # 添加课程处理
        |  |- delAction.java    # 删除课程处理
        |  |- updateAction.java # 修改课程处理
        |- UI/
           |- MainMenu.java   # 主程序窗口
           |- addMenu.java    # 添加课程对话框
           |- delMenu.java    # 删除课程对话框
           |- updateMenu.java # 修改课程对话框
data/
  |- name.txt      # 课程名称
  |- ID.txt        # 课程编号
  |- type.txt      # 课程类别（必修/选修）
  |- grade.txt     # 开课年级
  |- teacher.txt   # 教师姓名
```

## 课程字段

- 课程名称
- 课程编号
- 课程类别（必修 / 选修）
- 开课年级（大一 / 大二 / 大三 / 大四）
- 教师姓名

## 运行方法

1. 确保已安装 Java
2. 编译源文件:
   ```
   javac -d out src/*.java src/edu/neuq/**/*.java
   ```
3. 运行程序:
   ```
   java -cp out Main
   ```

## 使用方法

1. 启动程序查看主课程列表
2. 点击"添加"按钮添加新课程
3. 点击"删除"按钮删除课程
4. 点击"修改"按钮编辑课程信息
5. 点击"搜索"按钮搜索特定课程
6. 使用下拉筛选框按年级或课程类型筛选
7. 点击"退出"保存并退出