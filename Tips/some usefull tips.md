# Pytorch编程技巧

#### 比较两个tensor是否完全相同
直接使用a == b返回的是一个a.shape的矩阵，如果只想返回一个最终是否相同的结果，可以使用：
```python 
torch.all(torch.eq(a, b))
```
