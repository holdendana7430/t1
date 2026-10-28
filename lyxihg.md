代发 wailian999

[U69] PHP：PDO 预处理
来源：http://hz.gotoacloud.top/gtdtwfvgim.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sufxvd.cn/gtseofiipo.html

[U70] PHP：PDO 事务
来源：http://hz.feifeiyinyue.top/gteisrvlcs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ydzc1.top/gtkzpvvack.html

[U71] PHP：抛出异常
来源：http://hz.redwolf501.top/gtirtyztwt.html

throw new RuntimeException("失败", 500);
来源：http://hz.tianlin.xyz/gtbbhtebrg.html

[U72] PHP：写错误日志
来源：http://hz.mhx1999.top/gtlnoocayp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.redwolf501.top/gtrjkzvytt.html

[U73] PHP：读取 ini 配置
来源：http://hz.birdmap.top/gtupbxfuqs.html

parse_ini_file("config.ini", true)
来源：http://hz.jinghuilouyu.cn/gtpbxnmaff.html

[U74] PHP：读取环境变量
来源：http://hz.pengpengdd.cyou/gtrtbxluul.html

getenv("APP_ENV") ?: "production"
来源：http://hz.feifeiyinyue.top/gtonlhrcaq.html

[U75] PHP：依赖注入
来源：http://hz.nanxuanxn.top/gtikznmssr.html

composer require psr/container
来源：http://hz.quarkkingdee.top/gtswkipnxh.html

[U76] PHP：简单路由
来源：http://hz.chenlongwang.top/gtgchsszbp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shanyushiyangkeji.top/gtjhbsjceb.html

[U77] PHP：模板渲染
来源：http://hz.jiagoushi.top/gtpwnknwsn.html

composer require twig/twig
来源：http://hz.meibo888.top/gthnolhshv.html

[U78] PHP：单元测试
来源：http://hz.guannengcc.top/gtsohozkpq.html

composer require --dev phpunit/phpunit
来源：http://hz.shanyushiyangtech.top/gtfzwkfoen.html

[U79] PHP：静态分析
来源：http://hz.feifeiyinyue.top/gtjvbkozpo.html

composer require --dev phpstan/phpstan
来源：http://hz.shangyingyoupin.top/gtjmszquaj.html

[U80] PHP：代码规范修复
来源：http://hz.guowangkeji.top/gtaccqpvti.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jiagoushi.top/gtaucpdjjr.html

[U81] JS：初始化项目
来源：http://hz.gotoacloud.top/gtmmnpontp.html

npm init -y;  npm i express
来源：http://hz.havefunace.top/gtpzeuqepr.html

[U82] JS：package.json 脚本
来源：http://hz.ppjwa.cn/gtlzxwujyo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xylfe.cn/gtbodqmdhh.html

[U83] JS：ES Module 导入导出
来源：http://hz.0kj1m.cn/gtsclneawl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.c1oappe.top/gtraypvmyt.html

[U84] JS：CommonJS 写法
来源：http://hz.hnqzz.top/gtslmxwjbt.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.feifeiyinyue.top/gthfmenebf.html

[U85] JS：可选链
来源：http://hz.guannengcc.top/gtmybbtizx.html

a?.b?.c
来源：http://hz.nanxinkj.top/gtlfyktupb.html

[U86] JS：空值合并
来源：http://hz.hfpthk.cn/gtuzfnugce.html

a ?? b
来源：http://hz.tianlin.xyz/gtutdvthyp.html

[U87] JS：解构默认值
来源：http://hz.jinqigfzy.top/gtwtqqxeau.html

const { a = 1, b = 2 } = obj;
来源：http://hz.smart0.xyz/gtnzevcbyb.html

[U88] JS：对象展开合并
来源：http://hz.chenjidiqi.icu/gtstmbjfvp.html

{ ...a, ...b }
来源：http://hz.cqqwz.cn/gtqixtlgkf.html

[U89] JS：数组去重
来源：http://hz.yanxiufei.cn/gtlnosckuw.html

[...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtactkpnaz.html

[U90] JS：数字数组排序
来源：http://hz.fzhhl.top/gtylglccmn.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xinyue.icu/gtztphvlce.html

[U91] JS：对象键值遍历
来源：http://hz.gzhubu.top/gtbwlvrjqh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinqigfzy.top/gtosbntucu.html

[U92] JS：深拷贝
来源：http://hz.iojbl.cn/gtswtwhxhv.html

structuredClone(obj)
来源：http://hz.tianlin.xyz/gtytsrjnfm.html

[U93] JS：模板字符串
来源：http://hz.mhx1999.top/gtpcfblcfu.html

`共 ${n} 条`
来源：http://hz.xinyue.icu/gtojktclsb.html

[U94] JS：箭头函数
来源：http://hz.aizwys.cn/gtljbmjbyl.html

const double = x => x * 2;
来源：http://hz.zhixingplan.top/gtvwlewewh.html

[U95] JS：Promise 包装
来源：http://hz.yueranfly.top/gtohlcrwsq.html

new Promise((resolve, reject) => {})
来源：http://hz.tian-w.cn/gtyplwnwnw.html

[U96] JS：async/await 与异常
来源：http://hz.chenjidiqi.icu/gtvchaovzd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtdmtwwppg.html

[U97] JS：并发请求
来源：http://hz.chenzaomai.com/gtnviieest.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtljvryscw.html

[U98] JS：fetch 带 JSON
来源：http://hz.dianchejie.cn/gtphlftqql.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hnxiangtu.top/gtohungurt.html

[U99] JS：事件监听
来源：http://hz.shzxlz.cn/gtirhalfdq.html

el.addEventListener("click", e => {})
来源：http://hz.guannengcc.top/gtgtigzhnn.html

[U100] JS：DOM 查询
来源：http://hz.xingfuxueyuan.xyz/gtodzemuak.html

document.querySelector(".item")
来源：http://hz.shuidangran.top/gtveqvwrcr.html

[U101] JS：classList 操作
来源：http://hz.hnxiangtu.top/gtalbrwlmk.html

el.classList.toggle("active")
来源：http://hz.zhoulong.xyz/gttumviyhs.html

[U102] JS：本地存储
来源：http://hz.zhixingplan.top/gtljfbrnki.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shzxlz.cn/gtkhceeukx.html

[U103] JS：定时器
来源：http://hz.quarkkingdee.top/gtnqegsiby.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinyuanbaomall.cn/gtwxrivxuv.html

[U104] JS：防抖
来源：http://hz.nanxuanxn.top/gtxbcehmpm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtolelrrby.html

[U105] JS：节流
来源：http://hz.chenlongwang.top/gtktutlwer.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuxming.cn/gtxwnunbwv.html

[U106] JS：日期格式化
来源：http://hz.jqgufenzy.top/gtjofoiulv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.chenjidiqi.icu/gtrjjjudxc.html

[U107] JS：数字千分位
来源：http://hz.pycfn.com/gtaxeknsqo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tianlin.xyz/gtaqkpecwi.html

[U108] JS：随机整数
来源：http://hz.ehwqpu.com/gtswkadrrl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zycfv.cn/gtefotajfd.html

[U109] JS：数组分组
来源：http://hz.meibo888.top/gtdnpkjghf.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gtjrrotuof.html

[U110] JS：数组分块
来源：http://hz.kuanghao11.cn/gttqmmymfb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhixingplan.top/gtlmyuwwdp.html

[U111] JS：对象转 Map
来源：http://hz.shzxlz.cn/gtmlvfrejh.html

new Map(Object.entries(obj))
来源：http://hz.xziqi.cn/gttbiymadj.html

[U112] JS：字符串补位
来源：http://hz.hfpthk.cn/gtjmqihftf.html

"7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtppbiptsx.html

[U113] JS：正则替换全部
来源：http://hz.cheryme.top/gtaubrezpt.html

s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtcyengnmm.html

[U114] JS：JSON 深比较
来源：http://hz.fzhhl.top/gtbbsthkfu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xziqi.cn/gtdvsgjmyl.html

[U115] JS：生成 UUID
来源：http://hz.ppjwa.cn/gtswnlmmfe.html

crypto.randomUUID()
来源：http://hz.52xcode.cn/gtugtatqgw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.nanxuanxn.top/gtugemqpsz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shzxlz.cn/gtydmjxpag.html

[U117] JS：单元测试
来源：http://hz.c1oappe.top/gtrfwviszr.html

npm i -D vitest;  npx vitest
来源：http://hz.cheryme.top/gtqiwviqpy.html

[U118] JS：开发服务器
来源：http://hz.cdnleiting.top/gtqxujoxgk.html

npm i -D vite;  npx vite
来源：http://hz.nanxinkj.top/gtkueudyrp.html

[U119] JS：生产构建
来源：http://hz.xinyue.icu/gtqwgbnuxx.html

npx vite build
来源：http://hz.zhixingplan.top/gtapdomgwz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xinyue.icu/gtkuhixcrx.html

import.meta.env.VITE_API_URL
来源：http://hz.birdmap.top/gtwhrpmlft.html

================================================================================
来源：http://hz.hnxiangtu.top/gtwvovwtdi.html

统计汇总
来源：http://hz.daxiang520.top/gtxfzuyqqe.html

================================================================================
来源：http://hz.daria6918.cn/gtlsmpckop.html

按语言统计（条）：
来源：http://hz.hysaishi.cn/gtvwmqmuek.html

Python ......... 252
来源：http://hz.hnxiangtu.top/gtrgpbpadz.html

PHP ............ 252
来源：http://hz.jqgufenzy.top/gtiqpfpitx.html

JavaScript ..... 252
来源：http://hz.xinyue.icu/gtksyrybgu.html

TypeScript ..... 212
来源：http://hz.52xcode.cn/gtngsgrjxt.html

Java ........... 212
来源：http://hz.chenzaomai.com/gtfhwlfofo.html

Go ............. 212
来源：http://hz.shuidangran.top/gtnxacxhaa.html

Ruby ........... 212
来源：http://hz.ydzc1.top/gtirehzkrf.html

C# ............. 212
来源：http://hz.shzxlz.cn/gtuizvhsna.html

C .............. 30
来源：http://hz.quarkkingdee.top/gtaianrtsy.html

C++ ............ 30
来源：http://hz.cashguo.top/gtjtwwkfnv.html

SQL ............ 90
来源：http://hz.havefunace.top/gtvsgsqlnc.html

Bash ........... 80
来源：http://hz.zdqjudy.top/gtfpwrdcax.html

Kotlin ......... 15
来源：http://hz.chenlongwang.top/gtgrdlahot.html

Swift .......... 15
来源：http://hz.shuidangran.top/gtdqajaqfb.html

Lua ............ 10
来源：http://hz.ydjk.org.cn/gtqlvlprnv.html

Perl ........... 10
来源：http://hz.hysaishi.cn/gtuhwfdcnp.html

Scala .......... 10
来源：http://hz.sufxvd.cn/gtpcrauirm.html

------------------------------------
来源：http://hz.jinqigfzy.top/gtygyxijai.html

合计 ........... 2106 条
来源：http://hz.xuanzx.com/gttftjmszn.html

按章节统计：
来源：http://hz.jlsjyb.cn/gtnbsyplyi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.316326.xyz/gtyrhzpoxn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gtyilrsuyc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhoulong.xyz/gtqtcycnpj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jinqigfzy.top/gtdzxxwlgy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhixingplan.top/gtbrbdxscw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xylfe.cn/gtuaebyoiq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtackyoapm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.meibo888.top/gtfnglsrao.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtooccieyj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shzxlz.cn/gtkyxvqwhj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtotwbqrkv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtteeyautd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtbqmildxj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shanyushiyangtech.top/gtsiobmlfo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xinyue.icu/gtwtmasjfe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gtwohhonei.html

Q SQL 专题                              90
来源：http://hz.ydjk.org.cn/gtrfpppexi.html

R Bash 专题                             80
来源：http://hz.yuxming.cn/gtgglehjii.html

S C / C++ 专题                          60
来源：http://hz.gotoacloud.top/gtvqeksnvv.html

T 其他语言补充                          60
来源：http://hz.gotoacloud.top/gtnncanwtr.html

U 高频实用片段                         120
来源：http://hz.pycfn.com/gtgyeygppb.html

------------------------------------
来源：http://hz.chenzaomai.com/gtohbjdxjn.html

合计                                  2106 条
来源：http://hz.shanyushiyangtech.top/gtkvqcyoss.html

--------------------------------------------------------------------------------
来源：http://hz.pengpengdd.cyou/gthowyaqpo.html

使用提醒
来源：http://hz.cheryme.top/gtfsccwbpz.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtxytunmbt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.bjfxy.top/gtvqysxllr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.52xcode.cn/gtlemqttkv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yonumen.top/gtzrzcpksj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.haohaochexian.top/gtwfvgjalf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xinyue.icu/gtnbbhhnsn.html

—— 文件结束 ——
来源：http://hz.cucudq.cn/gtclojoznm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtnqoenfbe.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sysykeji.top/gtbpzhlnex.html

Common Programming Examples Cheat Book
来源：http://hz.hysaishi.cn/gtavqophys.html

================================================================================
来源：http://hz.9152youxi.cn/gtkwmeottx.html

【收录内容】
来源：http://hz.andypj.xyz/gtcnmagzpo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinghuilouyu.cn/gtwhbgkokc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yuxming.cn/gthamjonwl.html

SQL · Bash · C · C++
来源：http://hz.iojbl.cn/gtivqwqqdc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cheryme.top/gtscoxbkyv.html

【使用说明】
来源：http://hz.snrcjt.cn/gtjkplxuhy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.wangdashe.top/gtzwpynujx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.aibaodan.cn/gtidbaozek.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhixingplan.top/gtodpaktkt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.birdmap.top/gtbrgnuhaw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.haohaochexian.top/gtdprgyziy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sysykeji.top/gttazftaco.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shuidangran.top/gtzegoeflx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.kuanghao11.cn/gtmimptdcz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.pengpengdd.cyou/gtbuobqpdv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.snrcjt.cn/gtkpxgnukw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hywenlv.cn/gtzpmxxvsp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shanyushiyangkeji.top/gtocprtsti.html

【文件统计】
来源：http://hz.yonumen.top/gturekniym.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jlsjyb.cn/gtiyubbwgq.html

--------------------------------------------------------------------------------
来源：http://hz.yuxming.cn/gtexkyojoj.html

目  录
来源：http://hz.nanxuanxn.top/gtsiyngott.html

--------------------------------------------------------------------------------
来源：http://hz.zycfv.cn/gtkyfbxtdz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.iojbl.cn/gtnhzmrwao.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gtreuxtzki.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jiagoushi.top/gtifoapoiv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yuanzhike.top/gtirjfwpbx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.daria6918.cn/gtjvjdiwsb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yj20258888.top/gtflujqdcd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.aibaodan.cn/gtnoernbst.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.c1oappe.top/gtzitnngpl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xylfe.cn/gtmwydbpia.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ydjk.org.cn/gtcpuigpej.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtiryrfvcw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gtrbxaxchx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtytrmsygt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.birdmap.top/gtzormxzpo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.chenjidiqi.icu/gthffxitca.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtbvclwlgp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gotoacloud.top/gtwraxeybz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.svipenyu.cn/gtmcvpvcqc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hysaishi.cn/gtvtutzfea.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gtvdpgmtas.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shzxlz.cn/gtcdzetasm.html

================================================================================
来源：http://hz.havefunace.top/gtprkvlkag.html

A. 基础语法与类型
来源：http://hz.9152youxi.cn/gterxxrmhp.html

================================================================================
来源：http://hz.cqqwz.cn/gtpgygvbda.html

[A01] Hello World
来源：http://hz.snrcjt.cn/gtmanwrtak.html

Py:   print("Hello, World!")
来源：http://hz.xziqi.cn/gtkintvweg.html

PHP:  echo "Hello, World!";
来源：http://hz.wangdashe.top/gtyxifxvmr.html

JS:   console.log("Hello, World!");
来源：http://hz.gotoacloud.top/gtxkqbbmah.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.guannengcc.top/gtvsixqblr.html

Java: System.out.println("Hello, World!");
来源：http://hz.xylfe.cn/gtkrazeyeo.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.wangshuangyany.cn/gthnwgzxbe.html

Ruby: puts "Hello, World!"
来源：http://hz.kuanghao11.cn/gtjmwckouz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.guowangkeji.top/gteuwpohvv.html

[A02] 变量声明与赋值
来源：http://hz.aizwys.cn/gtapbxqlxz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.chenjidiqi.icu/gtnwziwhkg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.cdnleiting.top/gtdtrtvprz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.52xcode.cn/gtjhfolaby.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jinghuilouyu.cn/gtcsalmcue.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hongshengwenyu.top/gtjyujocxh.html

Go:   name := "Alex"; age := 20
来源：http://hz.sweek.top/gtvkwqpmkr.html

Ruby: name = "Alex"; age = 20
来源：http://hz.gotoacloud.top/gtjvcsnytv.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gaohongyu789.top/gtdypnbxpw.html

[A03] 常量定义
来源：http://hz.sweek.top/gtkcsqasja.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhoulong.xyz/gtyocwjqjr.html

PHP:  const PI = 3.14159;
来源：http://hz.chenlongwang.top/gtshsmsblf.html

JS:   const PI = 3.14159;
来源：http://hz.birdmap.top/gtqwuolfkh.html

TS:   const PI: number = 3.14159;
来源：http://hz.shuidangran.top/gtgswozkls.html

Java: static final double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtnalrjtys.html

Go:   const PI = 3.14159
来源：http://hz.fzhhl.top/gtpbcotqnd.html

Ruby: PI = 3.14159
来源：http://hz.daria6918.cn/gtkbrifwaj.html

C#:   const double PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gthqotrgea.html

[A04] 判断变量类型
来源：http://hz.cdnleiting.top/gtjorbtvty.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.pengpengdd.cyou/gtqevmmtdz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jinghuilouyu.cn/gtylcdlbuf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhoulong.xyz/gtuqlnlria.html

TS:   typeof x; x instanceof Date
来源：http://hz.316326.xyz/gtnrjlmoru.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ppjwa.cn/gtdoiickod.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shzxlz.cn/gtohmrkrzo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zhongyouzk.top/gttevyqvgc.html

C#:   x.GetType().Name; x is int
来源：http://hz.xziqi.cn/gtantkmeqr.html

[A05] 整数除法与取模
来源：http://hz.shangyingyoupin.top/gtjiqvrynz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.c1oappe.top/gtmcyctvyk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.wangdashe.top/gthizgdojt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinqigfzy.top/gtjgtrpfjn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhengqikj.top/gtiexokgdj.html

Java: 7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtlivzjvtq.html

Go:   7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gteaparjgo.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.316326.xyz/gtipcuxakv.html

C#:   7 / 2; 7 % 2
来源：http://hz.wangdashe.top/gtfptmtamg.html

[A06] 字符串转数字
来源：http://hz.zhixingplan.top/gtuqyqbszh.html

Py:   int("42"); float("3.14")
来源：http://hz.hywenlv.cn/gtskkxtobl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.quarkkingdee.top/gtgnrmfjar.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.dianchejie.cn/gthcvhxvmq.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.fengsongda.top/gtrklqtxsn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.wangdashe.top/gttgwzuzii.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yuanzhike.top/gtmjnziong.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.nanxinkj.top/gtypshjkdu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.redwolf501.top/gtzjuyyhpp.html

[A07] 数字转字符串
来源：http://hz.shanyushiyangkeji.top/gtmemklinv.html

Py:   str(42)
来源：http://hz.sxryk.cn/gtutpoctcm.html

PHP:  (string) 42; strval(42)
来源：http://hz.xingfuxueyuan.xyz/gtvobiuiuf.html

JS:   String(42); (42).toString()
来源：http://hz.zhongyouzk.top/gtvxyicgno.html

TS:   String(42)
来源：http://hz.feifeiyinyue.top/gtlytochid.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xylfe.cn/gtrdbwdrza.html

Go:   strconv.Itoa(42)
来源：http://hz.hammf.cn/gtjnnzcrgr.html

Ruby: 42.to_s
来源：http://hz.guannengcc.top/gtgbjpwyfc.html

C#:   42.ToString()
来源：http://hz.jianghu66.top/gtsizsxeis.html

[A08] 取整与四舍五入
来源：http://hz.shzxlz.cn/gtialymlqi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.gogol.net.cn/gtjoynqhpe.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.fengsongda.top/gtcqovdjje.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zdqjudy.top/gtpugpaphv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.shanyushiyangkeji.top/gtfkjeqzdo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.sysykeji.top/gttjxemflt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yj20258.top/gtwsviyaqe.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.ivvv.top/gtxweqmydm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.smart0.xyz/gtxjliuugb.html

[A09] 绝对值与最大最小值
来源：http://hz.sysykeji.top/gteivzwfyi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yanxiufei.cn/gtobmzkzof.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.sxryk.cn/gtpivjkcwu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.tian-w.cn/gtpjpxmwfh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.bjfxy.top/gtgokstuap.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.bjfxy.top/gtiedzcgjl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zycfv.cn/gtrxbryawp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.dianchejie.cn/gtdnnzpvwp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.shangyingyoupin.top/gtuysrogdv.html

[A10] 生成随机数
来源：http://hz.xuetiantiany.cn/gtzkcuvexw.html

Py:   import random; random.randint(1, 100)
来源：http://hz.yongpay.top/gtupvpdsrg.html

PHP:  random_int(1, 100);
来源：http://hz.shuidangran.top/gtdfqxcklr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.iojbl.cn/gtugtsfzmb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhengqikj.top/gtmhakemet.html

Java: new Random().nextInt(100) + 1
来源：http://hz.birdmap.top/gthfgsnyap.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.52xcode.cn/gtncemdbon.html

Ruby: rand(1..100)
来源：http://hz.sxryk.cn/gtpwrfkcwi.html


<!-- 参考信息 -->