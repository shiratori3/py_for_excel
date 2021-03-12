# 自用的xlwings脚本

## 当前脚本实现功能

- 合并工作表
- 批量转换为csv文件
- 数值清洗
- 变更正负号

### 功能介绍

- 合并工作表

> 当前支持：
>
> 1. 合并当前工作簿的所有工作表
> 2. 合并当前工作簿的文件路径下指定格式（支持csv、xls、xlsx）的所有文件内的首个或多个工作表至当前工作表或对应工作表（以文件名命名或以工作表命名）

    # 现有宏名称及对应功能
    merge_current_sheet # 合并当前工作簿的所有工作表至当前工作表
    merge_csv_to_same_sheet # 合并当前路径下的所有csv文件的首个工作表至当前工作表
    merge_xlsx_to_same_sheet # 合并当前路径下的所有xlsx文件的首个工作表至当前工作表
    merge_csv_to_diff_sheets # 合并当前路径下的所有csv文件的首个工作表至以文件名命名的工作表
    merge_xls_to_diff_sheets # 合并当前路径下的所有xls文件的首个工作表至以文件名命名的工作表
    merge_xlsx_to_diff_sheets # 合并当前路径下的所有xlsx文件的首个工作表至以文件名命名的工作表

- 批量转换为csv文件

> 当前支持：
>
> 1. 将当前工作簿的文件路径下对应格式的文件均转换成对应名称的csv文件

    # 现有宏名称及对应功能
    from_xlsx_to_csv # 当前路径下的xlsx文件批量转成csv
    from_xls_to_csv # 当前路径下的xls文件批量转成csv

- 数值清洗

> 当前支持：
>
> 1. 将当前工作表中，选中区域中含数字[0-9]的单元格清洗成纯数值，其余单元格不做变换。

    # 现有宏名称及对应功能
    num_with_2_dec # 清洗为2位小数的数值
    num_with_4_dec # 清洗为4位小数的数值
    num_with_0_dec # 清洗为0位小数的数值

- 变更正负号

> 当前支持：
>
> 1. 将当前工作表中，选中区域中为数值格式的单元格的数值乘以-1，实现变更正负的功能。

    # 现有宏名称及对应功能
    num_change_minus # 变更选中区域的数值的正负号
