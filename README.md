# Karabiner 配置

## 主要功能

### 全局

- 按下 escape 键将 normal_mode 变量设置为 1，并且将输入法切换到系统自带的英文输入法
- 将右 command 键映射为右 control
- 单独按下右 shift 键切换输入法

### 在非终端 APP 中

- 按 caps_lock 键切换鼠须管与系统自带的英文输入法

### 在终端 APP 中

- 按 asiocASIOC 会设置 normal_mode 变量为 0
- 在 normal_mode 为 1，英文输入法状态时按下 caps_lock 设置 normal_mode 为 0，并输出 a 进入 Vim 的插入模式，然后切换输入法为鼠须管
- 在 normal_mode 为 0，鼠须管输入法状态时按下 caps_lock 设置 normal_mode 为 1，并输出 escape 跳出 vim 插入模式，然后切换输入法为系统自带的英文输入法
- 在 normal_mode 为 0，系统自带的英文输入法状态时按下 caps_lock 设置 normal_mode 为 1，并输出 escape 跳出 vim 插入模式
- 连续按下 jk 映射为 escape 键，然后再切换输入法为系统自带的英文输入法

## 说明

本配置主要是为了实现在 Vim 中快速实现中英文输入法的切换。karabiner 中有选择输入法的功能，但是似乎目前的系统有 bug，切换非系统自带的输入法会导致输入法切换失败。希望苹果能够早日修复这个 bug。
