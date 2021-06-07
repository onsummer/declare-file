类型声明文件

# 1 查找顺序

- 若存在 `package.json` > `"types"` 字段
  - 若 `"types"` 字段指向的是 `d.ts` 文件，那默认就使用它
  - 若 `"types"` 字段指向的是 js 文件，则默认使用同级下同名的 `d.ts` 文件
- 否则，`package.json` > `"main"` 字段
  - 若 `"main"` 字段指向的是 `d.ts` 文件，那默认就使用它
  - 若 `"main"` 字段指向的是 js 文件，则默认使用同级下同名的 `d.ts` 文件
- 最后 `index.d.ts` 

