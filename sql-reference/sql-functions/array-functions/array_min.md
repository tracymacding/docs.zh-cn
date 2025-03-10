# array_min

## 功能

求取一个ARRAY中的所有数据中的最小值，返回这个结果。

## 语法

```Haskell
array_min(array(type))
```

## 示例

```plain text
mysql> select array_min([113, 11, 12]);
+------------------------+
| array_min([113,11,12]) |
+------------------------+
| 11                     |
+------------------------+

mysql> select array_min([11.33, 11.11, 12.324]);
+---------------------------------+
| array_min([11.33,11.11,12.324]) |
+---------------------------------+
| 11.11                           |
+---------------------------------+

mysql> select array_min([cast('2020-02-25 11:35:17' as datetime), cast('2019-08-25 17:07:10' as datetime), cast('2025-08-25 17:07:10' as datetime)]);
+--------------------------------------------------------------------------------------------------------------------------------------+
| array_min([CAST('2020-02-25 11:35:17' AS DATETIME),CAST('2019-08-25 17:07:10' AS DATETIME),CAST('2025-08-25 17:07:10' AS DATETIME)]) |
+--------------------------------------------------------------------------------------------------------------------------------------+
| 2019-08-25 17:07:10                                                                                                                  |
+--------------------------------------------------------------------------------------------------------------------------------------+
```
