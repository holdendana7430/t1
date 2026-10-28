代发 wailian999

[U69] PHP：PDO 预处理
来源：http://hz.hammf.cn/gtvjvnwrbx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shanyushiyangtech.top/gtgcwtuisf.html

[U70] PHP：PDO 事务
来源：http://hz.jqgfzy.top/gtguqskxin.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.iojbl.cn/gtdgahwiyo.html

[U71] PHP：抛出异常
来源：http://hz.cdnleiting.top/gtsyilwohx.html

throw new RuntimeException("失败", 500);
来源：http://hz.xylfe.cn/gtyxtdccoi.html

[U72] PHP：写错误日志
来源：http://hz.jinghuilouyu.cn/gtqvwgurcu.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhaomingkeji.xyz/gtzxzquuqx.html

[U73] PHP：读取 ini 配置
来源：http://hz.yangfankeji.com/gtaddpakec.html

parse_ini_file("config.ini", true)
来源：http://hz.fzhhl.top/gtiamdqwxy.html

[U74] PHP：读取环境变量
来源：http://hz.smart0.xyz/gtlaeikbxq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hywenlv.cn/gtfxxqrnwj.html

[U75] PHP：依赖注入
来源：http://hz.guannengcc.top/gtmczlxkfs.html

composer require psr/container
来源：http://hz.jianghu66.top/gtqammhxyv.html

[U76] PHP：简单路由
来源：http://hz.shanyushiyangtech.top/gtnhrbxmgy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.52xcode.cn/gtrmvqabkl.html

[U77] PHP：模板渲染
来源：http://hz.snrcjt.cn/gtluotdivy.html

composer require twig/twig
来源：http://hz.chenlongwang.top/gtfzwyhyuz.html

[U78] PHP：单元测试
来源：http://hz.aizwys.cn/gtxfbhglfh.html

composer require --dev phpunit/phpunit
来源：http://hz.zhijiandao.cn/gtatgstnis.html

[U79] PHP：静态分析
来源：http://hz.hammf.cn/gtfovrlntq.html

composer require --dev phpstan/phpstan
来源：http://hz.yj202588.top/gtzvaxiydr.html

[U80] PHP：代码规范修复
来源：http://hz.snrcjt.cn/gtphkznurm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yonumen.top/gtrsoafkvy.html

[U81] JS：初始化项目
来源：http://hz.sxryk.cn/gtvurihnms.html

npm init -y;  npm i express
来源：http://hz.gogol.net.cn/gtpeioveno.html

[U82] JS：package.json 脚本
来源：http://hz.jinyuanbaomall.cn/gtsoieuehd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sufxvd.cn/gtsioulqol.html

[U83] JS：ES Module 导入导出
来源：http://hz.daxiang520.top/gtmgkexsbx.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.0kj1m.cn/gtvjrgvkkq.html

[U84] JS：CommonJS 写法
来源：http://hz.nwbrower.top/gtgkhcegsx.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.havefunace.top/gtckajkkla.html

[U85] JS：可选链
来源：http://hz.yj202588.top/gtbudrtuxd.html

a?.b?.c
来源：http://hz.gogol.net.cn/gtgvkdkobh.html

[U86] JS：空值合并
来源：http://hz.hnqzz.top/gtaavntoub.html

a ?? b
来源：http://hz.shangyingyoupin.top/gtrrxkthiq.html

[U87] JS：解构默认值
来源：http://hz.hammf.cn/gtdtdrwvke.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hywenlv.cn/gthbmaeval.html

[U88] JS：对象展开合并
来源：http://hz.yueranfly.top/gtuppecjhr.html

{ ...a, ...b }
来源：http://hz.zhongyouzk.top/gtwbiczsjc.html

[U89] JS：数组去重
来源：http://hz.zdqjudy.top/gtlrfixfgy.html

[...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtddvjeitj.html

[U90] JS：数字数组排序
来源：http://hz.gaohongyu789.top/gtfbbzrgiu.html

[...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtvwmtrnry.html

[U91] JS：对象键值遍历
来源：http://hz.52xcode.cn/gtryztdajr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhengqikj.top/gtflchrdgf.html

[U92] JS：深拷贝
来源：http://hz.tanke756.top/gtievwsdwf.html

structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtylqmgrjm.html

[U93] JS：模板字符串
来源：http://hz.xuetiantiany.cn/gtjdwepmzy.html

`共 ${n} 条`
来源：http://hz.yj202588.top/gtitgocgci.html

[U94] JS：箭头函数
来源：http://hz.shzxlz.cn/gtroelylwq.html

const double = x => x * 2;
来源：http://hz.sysykeji.top/gtgypjiwcm.html

[U95] JS：Promise 包装
来源：http://hz.jqgufenzy.top/gtperordgm.html

new Promise((resolve, reject) => {})
来源：http://hz.feifeiyinyue.top/gtynownagm.html

[U96] JS：async/await 与异常
来源：http://hz.jinqigfzy.top/gtrhjcnecx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.nanxuanxn.top/gtoekrvfaa.html

[U97] JS：并发请求
来源：http://hz.tanke756.top/gtzmblvhwv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtthafmyzj.html

[U98] JS：fetch 带 JSON
来源：http://hz.andypj.xyz/gtyezrkhcj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gogol.net.cn/gtzfybkiwq.html

[U99] JS：事件监听
来源：http://hz.gzhubu.top/gtnpvbqonl.html

el.addEventListener("click", e => {})
来源：http://hz.52xcode.cn/gtshskjbur.html

[U100] JS：DOM 查询
来源：http://hz.tianlin.xyz/gthlydierb.html

document.querySelector(".item")
来源：http://hz.yuanzhike.top/gtoyerutug.html

[U101] JS：classList 操作
来源：http://hz.wangshuangyany.cn/gtrywsiqbi.html

el.classList.toggle("active")
来源：http://hz.yonumen.top/gtpcsydbvp.html

[U102] JS：本地存储
来源：http://hz.chenjidiqi.icu/gtchnisphj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hnxiangtu.top/gtsasqgldh.html

[U103] JS：定时器
来源：http://hz.hfpthk.cn/gtswjvhneb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ywan-chungtsiang.top/gtsmphxqpi.html

[U104] JS：防抖
来源：http://hz.tianlin.xyz/gtvahjtomu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gththsacgd.html

[U105] JS：节流
来源：http://hz.yueranfly.top/gteghqbvbg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hfpthk.cn/gtqxibmyjq.html

[U106] JS：日期格式化
来源：http://hz.snrcjt.cn/gtzusdwwqm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.bjfxy.top/gtqkcuqzbp.html

[U107] JS：数字千分位
来源：http://hz.xuetiantiany.cn/gtxpezqnor.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hammf.cn/gtnpdqsfeb.html

[U108] JS：随机整数
来源：http://hz.316326.xyz/gtodlaozdt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sysykeji.top/gtqjdzzwoi.html

[U109] JS：数组分组
来源：http://hz.c1oappe.top/gtbfiyxovz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cucudq.cn/gtncvebyql.html

[U110] JS：数组分块
来源：http://hz.ydzc1.top/gtjgbahyak.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinqigufen.top/gtrkeigvxi.html

[U111] JS：对象转 Map
来源：http://hz.chenlongwang.top/gtkkttisqc.html

new Map(Object.entries(obj))
来源：http://hz.meibo888.top/gtxrpyxgyt.html

[U112] JS：字符串补位
来源：http://hz.sufxvd.cn/gtbwntbiyr.html

"7".padStart(3, "0")
来源：http://hz.meibo888.top/gtgfhrfblr.html

[U113] JS：正则替换全部
来源：http://hz.yuxming.cn/gtwbutyrxe.html

s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtdfjqerxo.html

[U114] JS：JSON 深比较
来源：http://hz.chenjidiqi.icu/gtwolxetza.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnxiangtu.top/gtkdhewyfo.html

[U115] JS：生成 UUID
来源：http://hz.guannengcc.top/gtgkemxpho.html

crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtmtowdusx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xuanzx.com/gtomsgwgfz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.kuanghao11.cn/gtvrjufsvu.html

[U117] JS：单元测试
来源：http://hz.hongshengwenyu.top/gtdcrdbmkv.html

npm i -D vitest;  npx vitest
来源：http://hz.xingfuxueyuan.xyz/gtjekzmwzd.html

[U118] JS：开发服务器
来源：http://hz.jinqigufen.top/gtjmmyzqbl.html

npm i -D vite;  npx vite
来源：http://hz.c1oappe.top/gtzlnkmdvb.html

[U119] JS：生产构建
来源：http://hz.jianghu66.top/gtdoploqqa.html

npx vite build
来源：http://hz.ppjwa.cn/gtwkwsmflr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jiagoushi.top/gtodtfpofv.html

import.meta.env.VITE_API_URL
来源：http://hz.birdmap.top/gtznvdlvmm.html

================================================================================
来源：http://hz.chenzaomai.com/gtxcmdmugv.html

统计汇总
来源：http://hz.zhiwuduotai.top/gthmabfhnd.html

================================================================================
来源：http://hz.nanxinkj.top/gtmmrganto.html

按语言统计（条）：
来源：http://hz.fzhhl.top/gtsajhxkfm.html

Python ......... 252
来源：http://hz.ywan-chungtsiang.top/gthsyrgbwu.html

PHP ............ 252
来源：http://hz.shanyushiyangtech.top/gtsosljqzz.html

JavaScript ..... 252
来源：http://hz.nwbrower.top/gtumiorpai.html

TypeScript ..... 212
来源：http://hz.cdnleiting.top/gtygaoxcto.html

Java ........... 212
来源：http://hz.jiagoushi.top/gtbppwdzdt.html

Go ............. 212
来源：http://hz.pycfn.com/gtbwnqzvfr.html

Ruby ........... 212
来源：http://hz.gogol.net.cn/gtdbavywcg.html

C# ............. 212
来源：http://hz.yongpay.top/gtgpgwpvpf.html

C .............. 30
来源：http://hz.tian-w.cn/gtpsbskyvd.html

C++ ............ 30
来源：http://hz.jinqigfzy.top/gtdpelskpt.html

SQL ............ 90
来源：http://hz.ywan-chungtsiang.top/gtmbbbdphw.html

Bash ........... 80
来源：http://hz.shanyushiyangkeji.top/gtkzpspaqh.html

Kotlin ......... 15
来源：http://hz.yonumen.top/gtztixojnf.html

Swift .......... 15
来源：http://hz.yj202588.top/gtgcgzhbnp.html

Lua ............ 10
来源：http://hz.yueranfly.top/gtfthjfkbt.html

Perl ........... 10
来源：http://hz.sufxvd.cn/gtjcsbdoch.html

Scala .......... 10
来源：http://hz.vqdsnc.cn/gtguouuzpz.html

------------------------------------
来源：http://hz.cashguo.top/gtaaqnjebj.html

合计 ........... 2106 条
来源：http://hz.tanke756.top/gtttdelpyb.html

按章节统计：
来源：http://hz.jqgufenzy.top/gtyjlyfgyp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.feifeiyinyue.top/gthznbyxdw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.snrcjt.cn/gtbrlgfpli.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtzurbtzrr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jlsjyb.cn/gtmzednpqi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenjidiqi.icu/gtoksbcgbd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jqgufenzy.top/gtnbdmdzro.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtknbmyfoh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.wangshuangyany.cn/gtqagenswz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gtvqyjjnpf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yueranfly.top/gtnkdpishl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtmumrqrkp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtaomglidh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtmjyefibp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zycfv.cn/gtnkwwrdew.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yj20258.top/gtxtgqgxxv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtrpuojitc.html

Q SQL 专题                              90
来源：http://hz.cheryme.top/gtliaeiaou.html

R Bash 专题                             80
来源：http://hz.feifeiyinyue.top/gtsfmgfiue.html

S C / C++ 专题                          60
来源：http://hz.jlsjyb.cn/gthrshbztl.html

T 其他语言补充                          60
来源：http://hz.9152youxi.cn/gtchrxkcer.html

U 高频实用片段                         120
来源：http://hz.52xcode.cn/gtxnffmgpy.html

------------------------------------
来源：http://hz.fzhhl.top/gtqoetebhs.html

合计                                  2106 条
来源：http://hz.fzhhl.top/gtyogueqxi.html

--------------------------------------------------------------------------------
来源：http://hz.c1oappe.top/gtppagjlwu.html

使用提醒
来源：http://hz.hnqzz.top/gtztbtzzmi.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtnmzgoizd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinqigufen.top/gtgyzkpmds.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinqigufen.top/gtanlljemf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhiwuduotai.top/gtlkegfkrl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.havefunace.top/gttkesuefv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.guowangkeji.top/gtuoeadcob.html

—— 文件结束 ——
来源：http://hz.gogol.net.cn/gtckidgriw.html

================================================================================
来源：http://hz.zhixingplan.top/gtcfvhqefh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yonumen.top/gtjemmquvz.html

Common Programming Examples Cheat Book
来源：http://hz.jinyuanbaomall.cn/gtovongvdb.html

================================================================================
来源：http://hz.ivvv.top/gtnuojcsfr.html

【收录内容】
来源：http://hz.ppjwa.cn/gtpeultgcz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hfpthk.cn/gtpxfreydg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.birdmap.top/gtufsjtqla.html

SQL · Bash · C · C++
来源：http://hz.sysykeji.top/gtaclgelsf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.bjfxy.top/gtiferdvzp.html

【使用说明】
来源：http://hz.ehwqpu.com/gtumpnxrbh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hysaishi.cn/gtqdzvwzyj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cucudq.cn/gtpokestum.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yueranfly.top/gtxaornzhg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.pycfn.com/gtlygytynm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.havefunace.top/gtutbcpsmw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.quarkkingdee.top/gtsazacmxd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xuanzx.com/gtijjpqwni.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ywan-chungtsiang.top/gtuqlrfujr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hongshengwenyu.top/gttanglccz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.mhx1999.top/gtlmtfmpvd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.havefunace.top/gtdmpvcwzn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.birdmap.top/gtjvwtfadp.html

【文件统计】
来源：http://hz.yj20258.top/gtfhqumcrb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shuidangran.top/gtvrpvkugj.html

--------------------------------------------------------------------------------
来源：http://hz.xylfe.cn/gtfniwqdad.html

目  录
来源：http://hz.ywan-chungtsiang.top/gtsxffavoi.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gtqtjpwnhv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ppjwa.cn/gtqcrqabet.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jianghu66.top/gtrhnjqmjg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jqgfzy.top/gtncztstgv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.snrcjt.cn/gtgkxckdps.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhijiandao.cn/gtlawhincz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.pengpengdd.cyou/gtjtxaqhfj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtxzsvvyic.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.havefunace.top/gtgnogoylj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtuejnlddj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ybcxt.top/gtsfyodsqo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhijiandao.cn/gtffmbmvwm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gtbkkdjwne.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xylfe.cn/gtnkmvtdkd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zdqjudy.top/gtriusmnzx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj202588.top/gtvlshgnxk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtcurdralv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jinqigufen.top/gtbxihdwis.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sweek.top/gttnlavmye.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.sweek.top/gtxmfikhrh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gtzslfecte.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.quarkkingdee.top/gtzaaakyyk.html

================================================================================
来源：http://hz.meibo888.top/gtnqtlolnb.html

A. 基础语法与类型
来源：http://hz.ywan-chungtsiang.top/gtiivlrkrw.html

================================================================================
来源：http://hz.yvedp.cn/gtlkbseerf.html

[A01] Hello World
来源：http://hz.zhaomingkeji.xyz/gtgbzxewhz.html

Py:   print("Hello, World!")
来源：http://hz.tian-w.cn/gtqywrkwrd.html

PHP:  echo "Hello, World!";
来源：http://hz.shzxlz.cn/gtumonqolu.html

JS:   console.log("Hello, World!");
来源：http://hz.0kj1m.cn/gtynoyqrvl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj202588.top/gtntmbjhoa.html

Java: System.out.println("Hello, World!");
来源：http://hz.fengsongda.top/gtcysiihck.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sweek.top/gtyxjhaxqn.html

Ruby: puts "Hello, World!"
来源：http://hz.dashuyun.cn/gtiaiqfxjj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.redwolf501.top/gtdjchbhkz.html

[A02] 变量声明与赋值
来源：http://hz.smart0.xyz/gtktrtimsj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.aizwys.cn/gtkvpjekot.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.dashuyun.cn/gtczvijskd.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ywan-chungtsiang.top/gtevchmxbo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xingfuxueyuan.xyz/gtuvbxvxhp.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xingfuxueyuan.xyz/gtmbfxhcuq.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhixingplan.top/gtiohcybnu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.chenlongwang.top/gtjtxnnoyn.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.andypj.xyz/gtlwyglyep.html

[A03] 常量定义
来源：http://hz.ivvv.top/gttnjpvaym.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.nanxuanxn.top/gtkomoqqjf.html

PHP:  const PI = 3.14159;
来源：http://hz.52xcode.cn/gtcdymrmyz.html

JS:   const PI = 3.14159;
来源：http://hz.haohaochexian.top/gtqsylfvbg.html

TS:   const PI: number = 3.14159;
来源：http://hz.jqgufenzy.top/gtnbtmyibb.html

Java: static final double PI = 3.14159;
来源：http://hz.iojbl.cn/gtvwwiabbc.html

Go:   const PI = 3.14159
来源：http://hz.jinqigufen.top/gtjrcapvfd.html

Ruby: PI = 3.14159
来源：http://hz.jyoumei.cn/gtceknbqvk.html

C#:   const double PI = 3.14159;
来源：http://hz.cashguo.top/gtvhvwfeld.html

[A04] 判断变量类型
来源：http://hz.andypj.xyz/gtkuaopckl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.pengpengdd.cyou/gtygcvdaqs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.dianchejie.cn/gtdgoocfvb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.redwolf501.top/gtwzbtycwj.html

TS:   typeof x; x instanceof Date
来源：http://hz.mhx1999.top/gtdibdhkus.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.svipenyu.cn/gtvkrruymq.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.nanxuanxn.top/gtaiisucrk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.ybcxt.top/gtwjuykdkl.html

C#:   x.GetType().Name; x is int
来源：http://hz.birdmap.top/gtqihebzwu.html

[A05] 整数除法与取模
来源：http://hz.yangfankeji.com/gtchyakwqm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shanyushiyangtech.top/gtysqoruau.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yj202588.top/gtivjmzvts.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.meibo888.top/gtmusghytk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtefezbpsm.html

Java: 7 / 2; 7 % 2
来源：http://hz.snrcjt.cn/gtbgawqmor.html

Go:   7 / 2; 7 % 2
来源：http://hz.cucudq.cn/gtilihtqgv.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtgttzljto.html

C#:   7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtszqicbql.html

[A06] 字符串转数字
来源：http://hz.jqgufenzy.top/gtnuflyrji.html

Py:   int("42"); float("3.14")
来源：http://hz.ybcxt.top/gtczozaezk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ydzc1.top/gtuxeoffsw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.gzhubu.top/gtaqdlhxhf.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hongshengwenyu.top/gtautedygg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.tian-w.cn/gtmfgbiwyl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jiagoushi.top/gtxwwpqsty.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.cashguo.top/gtmcqnfali.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yj20258.top/gtszvqegpq.html

[A07] 数字转字符串
来源：http://hz.jianghu66.top/gtpmlhsmyh.html

Py:   str(42)
来源：http://hz.gzhubu.top/gtroplihgj.html

PHP:  (string) 42; strval(42)
来源：http://hz.guannengcc.top/gtcfswqlvb.html

JS:   String(42); (42).toString()
来源：http://hz.ywan-chungtsiang.top/gtbsbqjkxi.html

TS:   String(42)
来源：http://hz.yvedp.cn/gtztsbimoa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hnxiangtu.top/gtvtsrvgof.html

Go:   strconv.Itoa(42)
来源：http://hz.wangdashe.top/gtcqobsjlh.html

Ruby: 42.to_s
来源：http://hz.xuetiantiany.cn/gtuljmsxcj.html

C#:   42.ToString()
来源：http://hz.zhijiandao.cn/gtojndcwkb.html

[A08] 取整与四舍五入
来源：http://hz.jyoumei.cn/gtkpwqqgnk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.shangyingyoupin.top/gtydpwdxpd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.fengsongda.top/gtrxifslhx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.sxryk.cn/gtukgusnwc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ivvv.top/gtfrfpdurw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.redwolf501.top/gtunwuslvu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.gaohongyu789.top/gtatamkkzv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.c1oappe.top/gtevidcsjd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hongshengwenyu.top/gtskhumhlu.html

[A09] 绝对值与最大最小值
来源：http://hz.iojbl.cn/gttppyjirk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.sxryk.cn/gtvtxqrnoh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhiwuduotai.top/gtaojvxmwe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.iojbl.cn/gtpxoatfdu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yj20258888.top/gtwhlicygk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.ppjwa.cn/gtnmhxvoza.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.nanxinkj.top/gtdzeepcfe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.tanke756.top/gtykdjyzwl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.chenlongwang.top/gtsnasytco.html

[A10] 生成随机数
来源：http://hz.nwbrower.top/gtvkuplgvm.html

Py:   import random; random.randint(1, 100)
来源：http://hz.c1oappe.top/gtpawkobbg.html

PHP:  random_int(1, 100);
来源：http://hz.yuxming.cn/gtoamvuxsl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.smart0.xyz/gtxvvlkwbv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.birdmap.top/gtblwmdbad.html

Java: new Random().nextInt(100) + 1
来源：http://hz.shanyushiyangtech.top/gtuebcudqs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.shanyushiyangtech.top/gtexgczeis.html

Ruby: rand(1..100)
来源：http://hz.kuanghao11.cn/gtpqvgmqdw.html


<!-- 参考信息 -->