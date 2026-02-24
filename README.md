# OnePlus_Action
**```Build Kernel For OnePlus```**
>更高效 更全面 更快速 更稳定

[![Build](https://img.shields.io/badge/GitHub%20Actions-Build-181717?logo=github&logoColor=white&style=flat-square)](https://github.com/Kdufse/OnePlus_Action/actions/workflows/Build%20Kernel%20OnePlus.yml) [![OnePlus Kernel Manifest](https://img.shields.io/badge/OnePlus%20Kernel%20Manifest-EB0029?logo=oneplus&logoColor=white&style=flat-square)](https://github.com/OnePlusOSS/kernel_manifest) [![Coolapk](https://img.shields.io/badge/Follow-Coolapk-3DDC84?style=flat-square&logo=android&logoColor=white)](http://www.coolapk.com/u/30424290)

------
# Fork本项目
> 打开项目的右上角的Fork按键，随后取消勾选"Copy the `main` branch only"，Fork成功后会跳转到Fork后的仓库界面，打开Settings，找到Default branch，将其修改为"sample"，然后你就可以自行创作了。

------

# 公告
 
------
> [!NOTE]
>配置文件中最后的一个``_？``后缀是你正在使用系统版本的代号。而无后缀的大部分是出厂``Android``版本。**``Android16``起从``_b``开始重新计算。** 判断具体的适用安卓版本请手动打开清单,手动改成其他代号,前提是它们确实存在。
> <details>
> <summary><strong>点击查看详细的版本代号</strong></summary>
>
>>`_？ Android19 (？)`
>
>>`_？ Android18 (？)`
>
>>`_c Android17 (Cinnamon Bun)`<strong>
>
>>`_b Android16 (Baklava)`
>
>>`_v Android15 (Vanilla Ice Cream)`
>
>>`_u Android14 (Upside Down Cake)`
>
>>`_t Android13 (Tiramisu)`
>
>>`_s Android12 (Snow Cone)`</strong>
>
> </details>
 
------
> [!IMPORTANT]
>关于运行时间的数据参考
>
>|| 平均耗时|最大耗时|
>|------------------|----------------------|------------|
>| `极速构建所有机型` | `1st:19min ~ 35min 2nd:9min ~ 19min` | `42min`|
>| `内核版本5.10-5.15使用官方脚本构建` | `29min ~ 35min`| `45min`    |
>| `内核版本6.1-6.12使用官方脚本构建` | `59min ~ 1h12min`| `1h28min` |
>
> >使用ccache第一次可能会减速、仅极速构建生效
>
> >repo工具版本差异可能会影响耗时
>
>也就是说,如果你运行的时长超过了对应机型的最高时间,请暂停重新运行并查看step,看看有没有占用时间过长的步骤,特别注意Initialize Repo and Sync这一步,受到上游REPO工具链的影响会经常出问题.这一步超过15min可以重新尝试一次,如果依旧失败请等待修复
 
------
 