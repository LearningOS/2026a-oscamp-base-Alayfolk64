# 学员领取与提交指南

## 1. 绑定账号并领取仓库

加入 [OpenCamp 秋冬季训练营](https://opencamp.cn/os2edu/camp/2026fall)，并绑定自己实际使用的 GitHub 账号。

点击[领取作业仓库](https://github.com/LearningOS/2026a-enroll/issues/new?template=base.yml)，点击 **Create** 提交申请。系统自动读取申请人账号；等待机器人回复，打开回复里的邀请链接并接受邀请。

## 2. 克隆作业仓库

```sh
git clone https://github.com/LearningOS/2026a-oscamp-base-你的GitHub登录名.git
```

把占位文字替换为自己的登录名；该命令下载已分配的作业仓库。

```sh
cd 2026a-oscamp-base-你的GitHub登录名
```

进入本地仓库。保持在默认的 `main` 分支完成实验。

## 3. 提交实验

使用自己已经登录的 Git 客户端提交并 push 到 `main`。命令行示例：

```sh
git add 你修改的实验文件
git commit -m "Complete an exercise"
git push origin main
```

依次暂存指定实验文件、记录提交、推送到分配仓库的 `main`。Git 的 push 仍需使用自己的 GitHub 账号授权。可以直接用已登录的 GitHub Desktop 或编辑器完成相同步骤。

## 4. 查看评测与成绩

每次 push 自动触发配置检查和正式评测。打开 Actions，查看各练习原始日志与分数。只有自己账号触发的运行会上传自己的成绩；维护者代推只测试。

总分 100，上传本次完整评测的实际得分。未完成的模板出现测试失败属于预期。环境安装失败或运行被取消时不会上传不完整结果。

上传成功日志为 `OpenCamp accepted the score (result=1).`。若接口拒绝，先确认自己加入秋冬季训练营、绑定同一个 GitHub 账号，再把脱敏错误交给维护者。修复后可在 GitHub Actions 重跑工作流。
