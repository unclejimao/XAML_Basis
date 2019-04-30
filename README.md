# XAML_Basis
XAML basic note
# XAML 要点
新建的WPF项目中MainWindow.xaml源码：

	<Window x:Class="XAML_Learning.MainWindow"
			xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
			xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
			xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
			xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
			xmlns:local="clr-namespace:XAML_Learning"
			mc:Ignorable="d"
			Title="MainWindow" Height="450" Width="800">
		<Grid>
        
		</Grid>
	</Window>

其中包含两个元素

- <Window>元素
- <Grid>元素

其中<Window>元素是一个顶级元素，在.xaml文件中，只能有一个顶级元素，通常用下面元素作为顶级元素：

- <Page>元素：<Page>元素与<Window>元素类似，可以用于导航应用程序
- <Application>元素

顶级元素开始标签<Window>声明时包含以下属性：

- 类名：

	x:Class="XAML_Learning.MainWindow"

- 名称空间：

	xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
	xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
	xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
	xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
	xmlns:local="clr-namespace:XAML_Learning"

- Title：标题属性
- Height：高度属性
- Width：宽度属性

## 元素属性的设置方法
1. 直接在元素开始标签中设置

	<Grid Name="grid_1">
	</Grid>

2. 在元素体中以显式方式设置

	<Grid>
		<Grid.Name>grid_1</Grid.Name>
	</Grid>