# Soil-type-Code-conversion-FAO90-HWSD
# Runtime environment: Arcmap
# 编写背景
- HWSD数据集中的土壤类型栅格仅对土壤类型赋予代码，但是当需要制图输出的时候，需要将土壤类型代码转换为土壤类型名称，如果图斑数很多，类别数很多的时候，人工手动去赋值费时费力，通过编写本脚本代码，可以实现批量自动化赋值，将土壤类型代码转换为土壤类型名称，省时省力。这个代码是仅针对HWSD数据集，其采用FAO-90编码土壤分类系统，关于该数据集和分类系统说明请到相应官网或者其他数据网站下载。
# 操作步骤

1、在属性表中选择需要重新赋值的字段，右键打开字段计算器（Field Calculator），注意该字段类型必须是string类型。
![image](https://user-images.githubusercontent.com/44941550/167160345-0dee195b-4482-4a14-8253-6901cac50af0.png)

2、勾选Show Codeblock后填入本程序的源代码（代码当中gridcode字段代表土壤类型代码），将转换源代码填入Pre-Logic Script Code，然后在“typename=”下面填入u

![image](https://user-images.githubusercontent.com/44941550/167160386-194be3c4-13fc-4c55-b6ae-d9bf0dc07286.png)

3、这里填入的u是跟代码里面的Dim u对应的，如果代码第一条的u变成其它字符，相应的下面填入的字符也要跟着变，而typename是赋值土壤名称的字段名称，也就是刚才点击右键打开字段计算器的字段的名称。

然后点击ok就开始计算了

![image](https://user-images.githubusercontent.com/44941550/167160434-e446e5fc-689d-4171-bb0d-1367183474a2.png)

下图是重新赋值的结果

![image](https://user-images.githubusercontent.com/44941550/167160461-3adf6c18-0cd6-4b87-be48-c5445eb7b0d0.png)
