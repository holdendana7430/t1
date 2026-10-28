代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.guannengcc.top/gtkyfsoiyx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.pengpengdd.cyou/gtzjtiishz.html

[U68] PHP：PDO 连接
来源：http://hz.jyoumei.cn/gtcneieaug.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jqgfzy.top/gtrbcqzayp.html

[U69] PHP：PDO 预处理
来源：http://hz.ivvv.top/gtfzampffc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hfpthk.cn/gtoyvijmif.html

[U70] PHP：PDO 事务
来源：http://hz.guannengcc.top/gtjkpevyqx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.feifeiyinyue.top/gtetylmbrp.html

[U71] PHP：抛出异常
来源：http://hz.ppjwa.cn/gtnsmrvvnh.html

throw new RuntimeException("失败", 500);
来源：http://hz.xuetiantiany.cn/gtmjispztn.html

[U72] PHP：写错误日志
来源：http://hz.jianghu66.top/gteoeeerkp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shzxlz.cn/gtbhjtpods.html

[U73] PHP：读取 ini 配置
来源：http://hz.bjfxy.top/gtvhacuwtr.html

parse_ini_file("config.ini", true)
来源：http://hz.pycfn.com/gtxpkyqvpb.html

[U74] PHP：读取环境变量
来源：http://hz.tian-w.cn/gtlkdgcett.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yueranfly.top/gtuxzcyibf.html

[U75] PHP：依赖注入
来源：http://hz.jqgufenzy.top/gtmxkukcdk.html

composer require psr/container
来源：http://hz.zhengqikj.top/gtaqzopokv.html

[U76] PHP：简单路由
来源：http://hz.daria6918.cn/gtbzccrxsu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gotoacloud.top/gtgnfzuxzl.html

[U77] PHP：模板渲染
来源：http://hz.haohaochexian.top/gtsqdanknm.html

composer require twig/twig
来源：http://hz.vqdsnc.cn/gtnilysagx.html

[U78] PHP：单元测试
来源：http://hz.jianghu66.top/gtcpeutohi.html

composer require --dev phpunit/phpunit
来源：http://hz.daria6918.cn/gtgmmjucgl.html

[U79] PHP：静态分析
来源：http://hz.ivvv.top/gtvetooplo.html

composer require --dev phpstan/phpstan
来源：http://hz.kuanghao11.cn/gtddrfqoiz.html

[U80] PHP：代码规范修复
来源：http://hz.mhx1999.top/gtiurpofmy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sysykeji.top/gttlenghke.html

[U81] JS：初始化项目
来源：http://hz.hnxiangtu.top/gtsncqavof.html

npm init -y;  npm i express
来源：http://hz.ehwqpu.com/gtwiouhjna.html

[U82] JS：package.json 脚本
来源：http://hz.chenlongwang.top/gtndlnozns.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jyoumei.cn/gtsequzmwa.html

[U83] JS：ES Module 导入导出
来源：http://hz.hysaishi.cn/gtxcawdbff.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.guannengcc.top/gtvqhpeuza.html

[U84] JS：CommonJS 写法
来源：http://hz.shuidangran.top/gtypimokrv.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ppjwa.cn/gtymalsygp.html

[U85] JS：可选链
来源：http://hz.smart0.xyz/gtiafwdvql.html

a?.b?.c
来源：http://hz.yanxiufei.cn/gtxoucsxny.html

[U86] JS：空值合并
来源：http://hz.tanke756.top/gtzgagrzmp.html

a ?? b
来源：http://hz.yuxming.cn/gtwslngufm.html

[U87] JS：解构默认值
来源：http://hz.jinqigufen.top/gtdqhqjrrd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hysaishi.cn/gtkvxooxgh.html

[U88] JS：对象展开合并
来源：http://hz.andypj.xyz/gtdoqcmqpy.html

{ ...a, ...b }
来源：http://hz.snrcjt.cn/gtkawwdedq.html

[U89] JS：数组去重
来源：http://hz.feifeiyinyue.top/gtxnglxycs.html

[...new Set(arr)]
来源：http://hz.yj20258.top/gtcgsfhoba.html

[U90] JS：数字数组排序
来源：http://hz.svipenyu.cn/gtnzwatmtf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtmsbgxcyn.html

[U91] JS：对象键值遍历
来源：http://hz.chenjidiqi.icu/gticvmpyhu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.chenlongwang.top/gtwteybpky.html

[U92] JS：深拷贝
来源：http://hz.birdmap.top/gtczcgqhwf.html

structuredClone(obj)
来源：http://hz.xinyue.icu/gtlnqqplah.html

[U93] JS：模板字符串
来源：http://hz.yuxming.cn/gtsdwxmygu.html

`共 ${n} 条`
来源：http://hz.pycfn.com/gtstvquduu.html

[U94] JS：箭头函数
来源：http://hz.zdqjudy.top/gtvkedcpsu.html

const double = x => x * 2;
来源：http://hz.wangdashe.top/gtkrvcwtxb.html

[U95] JS：Promise 包装
来源：http://hz.hnqzz.top/gtbenkeczp.html

new Promise((resolve, reject) => {})
来源：http://hz.wangshuangyany.cn/gtvrpdddhv.html

[U96] JS：async/await 与异常
来源：http://hz.jinghuilouyu.cn/gtaaeoknri.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtfssqttcg.html

[U97] JS：并发请求
来源：http://hz.birdmap.top/gtuxzirige.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtyssmfwrq.html

[U98] JS：fetch 带 JSON
来源：http://hz.ivvv.top/gtufzfgwwa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hfpthk.cn/gtlffuugmp.html

[U99] JS：事件监听
来源：http://hz.c1oappe.top/gtpnscpqhn.html

el.addEventListener("click", e => {})
来源：http://hz.yongpay.top/gtdgyvsvcr.html

[U100] JS：DOM 查询
来源：http://hz.ehwqpu.com/gtjthuembo.html

document.querySelector(".item")
来源：http://hz.shzxlz.cn/gtpkxfiwgw.html

[U101] JS：classList 操作
来源：http://hz.kuanghao11.cn/gtnunjsckk.html

el.classList.toggle("active")
来源：http://hz.sxryk.cn/gtnycoktzb.html

[U102] JS：本地存储
来源：http://hz.shanyushiyangkeji.top/gtpbvkgjvg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.snrcjt.cn/gtdeapcngp.html

[U103] JS：定时器
来源：http://hz.hfpthk.cn/gtfsyjbqaa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shzxlz.cn/gtprmfntpp.html

[U104] JS：防抖
来源：http://hz.shuidangran.top/gtvfjwtttf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtfnruejgd.html

[U105] JS：节流
来源：http://hz.yvedp.cn/gtphunfbwr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.tianlin.xyz/gthsnjotwa.html

[U106] JS：日期格式化
来源：http://hz.daria6918.cn/gtmghcdnfa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.smart0.xyz/gtngyzlghd.html

[U107] JS：数字千分位
来源：http://hz.fengsongda.top/gtshpukcli.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ppjwa.cn/gtptqydogj.html

[U108] JS：随机整数
来源：http://hz.aibaodan.cn/gtvgtsiuro.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinyuanbaomall.cn/gtejaotmjl.html

[U109] JS：数组分组
来源：http://hz.gotoacloud.top/gtahrauiqh.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yueranfly.top/gtjwvsknvp.html

[U110] JS：数组分块
来源：http://hz.nwbrower.top/gthgvonmtz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.0kj1m.cn/gtbnrvaktr.html

[U111] JS：对象转 Map
来源：http://hz.redwolf501.top/gtyzpvwydz.html

new Map(Object.entries(obj))
来源：http://hz.hywenlv.cn/gtuxzfyojv.html

[U112] JS：字符串补位
来源：http://hz.jinqigufen.top/gtlrjadyqf.html

"7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtihbargok.html

[U113] JS：正则替换全部
来源：http://hz.cdnleiting.top/gtnijztall.html

s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtoejubyva.html

[U114] JS：JSON 深比较
来源：http://hz.jyoumei.cn/gtlbmwipss.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtpzjgqdna.html

[U115] JS：生成 UUID
来源：http://hz.yj20258.top/gtnwmoybti.html

crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtolobsiza.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hywenlv.cn/gtpmhlvwba.html

/** @param {string} name */ function f(name) {}
来源：http://hz.9152youxi.cn/gtnhoyntyz.html

[U117] JS：单元测试
来源：http://hz.cheryme.top/gtuqqlfipz.html

npm i -D vitest;  npx vitest
来源：http://hz.guowangkeji.top/gtwsbqttxi.html

[U118] JS：开发服务器
来源：http://hz.guannengcc.top/gtndapeory.html

npm i -D vite;  npx vite
来源：http://hz.daria6918.cn/gtkhbcmgfd.html

[U119] JS：生产构建
来源：http://hz.zycfv.cn/gtgutdjpyq.html

npx vite build
来源：http://hz.nwbrower.top/gtwsylvpec.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenzaomai.com/gtrhwkjzrg.html

import.meta.env.VITE_API_URL
来源：http://hz.zdqjudy.top/gtdfzpoffx.html

================================================================================
来源：http://hz.gotoacloud.top/gtpathctcp.html

统计汇总
来源：http://hz.nwbrower.top/gtspuwlqmn.html

================================================================================
来源：http://hz.nanxinkj.top/gtkhdnitmn.html

按语言统计（条）：
来源：http://hz.zhixingplan.top/gtzzirtunb.html

Python ......... 252
来源：http://hz.yj20258888.top/gthfuzjwlv.html

PHP ............ 252
来源：http://hz.tian-w.cn/gtpddlydkk.html

JavaScript ..... 252
来源：http://hz.sufxvd.cn/gtrwfeaoio.html

TypeScript ..... 212
来源：http://hz.ehwqpu.com/gtzczxzkms.html

Java ........... 212
来源：http://hz.ybcxt.top/gttdvxxddu.html

Go ............. 212
来源：http://hz.cashguo.top/gttrgywici.html

Ruby ........... 212
来源：http://hz.ydjk.org.cn/gtznhowbvn.html

C# ............. 212
来源：http://hz.fengsongda.top/gtaozlgqtq.html

C .............. 30
来源：http://hz.sysykeji.top/gtpxurvjgt.html

C++ ............ 30
来源：http://hz.yj20258.top/gtxrktpntm.html

SQL ............ 90
来源：http://hz.yonumen.top/gtdyticnhn.html

Bash ........... 80
来源：http://hz.ydzc1.top/gtmtbvxpls.html

Kotlin ......... 15
来源：http://hz.hfpthk.cn/gtjlqyecrv.html

Swift .......... 15
来源：http://hz.jinqigfzy.top/gtpknmgjxh.html

Lua ............ 10
来源：http://hz.jyoumei.cn/gtgrsqdsln.html

Perl ........... 10
来源：http://hz.xziqi.cn/gttvwnuogb.html

Scala .......... 10
来源：http://hz.zhengqikj.top/gtsptfqnjj.html

------------------------------------
来源：http://hz.bjfxy.top/gtuxiuhmgt.html

合计 ........... 2106 条
来源：http://hz.feifeiyinyue.top/gtmjuffpev.html

按章节统计：
来源：http://hz.andypj.xyz/gtocyqkhvk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.iojbl.cn/gtvwgxxnzi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.feifeiyinyue.top/gtgfsnbdyu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtobbfvofm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yueranfly.top/gteqgfqgxy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xinyue.icu/gtdtbpfogd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sysykeji.top/gtldjxldfb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtnmqgakbt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.aizwys.cn/gtzrofzufi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtlumurrqr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.mhx1999.top/gtqiwuaobn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtwkoowezw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gtjiaaoyar.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtwvluqoyz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhaomingkeji.xyz/gtqialwsrj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.fengsongda.top/gtweccyrvi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtteyxzicg.html

Q SQL 专题                              90
来源：http://hz.yj20258.top/gtudvmykpj.html

R Bash 专题                             80
来源：http://hz.yvedp.cn/gttrhmtqqr.html

S C / C++ 专题                          60
来源：http://hz.hnqzz.top/gtpfbyaesn.html

T 其他语言补充                          60
来源：http://hz.haohaochexian.top/gtlsduexqk.html

U 高频实用片段                         120
来源：http://hz.zdqjudy.top/gtohgtzoyx.html

------------------------------------
来源：http://hz.quarkkingdee.top/gtouiluuqw.html

合计                                  2106 条
来源：http://hz.jiagoushi.top/gtfkzzjrmm.html

--------------------------------------------------------------------------------
来源：http://hz.vqdsnc.cn/gtgrlybuum.html

使用提醒
来源：http://hz.zhaomingkeji.xyz/gtairmbuwj.html

--------------------------------------------------------------------------------
来源：http://hz.dashuyun.cn/gtuediccib.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.haohaochexian.top/gtkdkbacpl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.52xcode.cn/gtupcgnmjx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.tanke756.top/gtqcfwqlvn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.daria6918.cn/gtzexcdzpg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yangfankeji.com/gtsdojuebt.html

—— 文件结束 ——
来源：http://hz.yuanzhike.top/gtofstoqfr.html

================================================================================
来源：http://hz.gotoacloud.top/gtysoxmmqp.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.gogol.net.cn/gtamxbbaia.html

Common Programming Examples Cheat Book
来源：http://hz.snrcjt.cn/gtkifoyvkp.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzpmejgtq.html

【收录内容】
来源：http://hz.cdnleiting.top/gtpnvqjuqh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jlsjyb.cn/gtawoktusa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.haohaochexian.top/gtrlafkeqf.html

SQL · Bash · C · C++
来源：http://hz.zycfv.cn/gtzecxtozt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydjk.org.cn/gtquwfwnhm.html

【使用说明】
来源：http://hz.snrcjt.cn/gtdacrlkbk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.chenlongwang.top/gtsrqmjunr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.tianlin.xyz/gthuyjodag.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.iojbl.cn/gtwfujoqor.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.mhx1999.top/gtnghbzkyo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jiagoushi.top/gtylctqesr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jlsjyb.cn/gtsczvchva.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yangfankeji.com/gtkxltdsva.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.vqdsnc.cn/gtxaabkpaz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.daxiang520.top/gtpcnygdmq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhixingplan.top/gthkkuhztp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yuxming.cn/gtiiwcflew.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.52xcode.cn/gtdccuncfa.html

【文件统计】
来源：http://hz.ybcxt.top/gtfwgotkao.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.tian-w.cn/gtqttprxyf.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gtqkcpyidi.html

目  录
来源：http://hz.xylfe.cn/gtgdhdncji.html

--------------------------------------------------------------------------------
来源：http://hz.aibaodan.cn/gtyiqpoxnl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xziqi.cn/gtfkxgjfui.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jiagoushi.top/gtdzfeznrk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.tian-w.cn/gttdeuvgrb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.dianchejie.cn/gtrgkeamhi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.daria6918.cn/gtbebctoyh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yanxiufei.cn/gtlnblbrrr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gaohongyu789.top/gtebghqjhx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ybcxt.top/gtqspxlrtx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtiftsbzhc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.iojbl.cn/gtqlltwpcz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yanxiufei.cn/gtpigsyhyg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.sweek.top/gtrozfwlsr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtdiquxmrk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.316326.xyz/gtogstcqxb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jyoumei.cn/gtviigejxo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtoiyctupb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.dianchejie.cn/gtswtinoax.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.cucudq.cn/gtpelcwbae.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinqigufen.top/gtimlbwigs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.smart0.xyz/gtvvpipcad.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangdashe.top/gtwmegvgiv.html

================================================================================
来源：http://hz.redwolf501.top/gtjlglxqug.html

A. 基础语法与类型
来源：http://hz.zhaomingkeji.xyz/gtuppczfps.html

================================================================================
来源：http://hz.ydzc1.top/gtlzytvtcg.html

[A01] Hello World
来源：http://hz.jqgfzy.top/gtqoswjrtx.html

Py:   print("Hello, World!")
来源：http://hz.jyoumei.cn/gtupjrkzdy.html

PHP:  echo "Hello, World!";
来源：http://hz.fzhhl.top/gtokxtgfmv.html

JS:   console.log("Hello, World!");
来源：http://hz.quarkkingdee.top/gtmqlpnuov.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yongpay.top/gtfxioafnw.html

Java: System.out.println("Hello, World!");
来源：http://hz.wangdashe.top/gtnukrogpe.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.daria6918.cn/gtganiohxp.html

Ruby: puts "Hello, World!"
来源：http://hz.cashguo.top/gtqluqnmiu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.sufxvd.cn/gtobdcnmyg.html

[A02] 变量声明与赋值
来源：http://hz.ybcxt.top/gtuikvhygm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.guowangkeji.top/gtljbikruz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhengqikj.top/gtjrypedts.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jiagoushi.top/gtiicwrvwf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhengqikj.top/gtubotcktk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yj202588.top/gtydujvsbl.html

Go:   name := "Alex"; age := 20
来源：http://hz.daxiang520.top/gtsaxkdfde.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinqigufen.top/gtyyexylyc.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.pycfn.com/gtvggmdblq.html

[A03] 常量定义
来源：http://hz.sufxvd.cn/gtwgckexvb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hywenlv.cn/gtqwdkvmym.html

PHP:  const PI = 3.14159;
来源：http://hz.nanxinkj.top/gtbevltydi.html

JS:   const PI = 3.14159;
来源：http://hz.tianlin.xyz/gtqddnwacd.html

TS:   const PI: number = 3.14159;
来源：http://hz.cdnleiting.top/gtxlosnmip.html

Java: static final double PI = 3.14159;
来源：http://hz.c1oappe.top/gtnhptlriu.html

Go:   const PI = 3.14159
来源：http://hz.jiagoushi.top/gtrbidpltv.html

Ruby: PI = 3.14159
来源：http://hz.haohaochexian.top/gtluwqfdru.html

C#:   const double PI = 3.14159;
来源：http://hz.jqgfzy.top/gtaxtridfi.html

[A04] 判断变量类型
来源：http://hz.shzxlz.cn/gtfkzonsve.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhijiandao.cn/gtwajpjgaa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ywan-chungtsiang.top/gtraxlwvhs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hnqzz.top/gthlaibjjw.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinqigfzy.top/gtpfiqmuhq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.iojbl.cn/gtiotmmdwu.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.cdnleiting.top/gteovdfxuq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sufxvd.cn/gtwitcxefw.html

C#:   x.GetType().Name; x is int
来源：http://hz.aizwys.cn/gtnjdnreth.html

[A05] 整数除法与取模
来源：http://hz.tian-w.cn/gtdfyekiuz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jinqigufen.top/gtyvxvpffi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.cucudq.cn/gteksmztfo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhiwuduotai.top/gtarvwswvz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gtkhkdzeaq.html

Java: 7 / 2; 7 % 2
来源：http://hz.fengsongda.top/gtzqbsvpla.html

Go:   7 / 2; 7 % 2
来源：http://hz.cqqwz.cn/gtgqgtdcpk.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtvtmwmpys.html

C#:   7 / 2; 7 % 2
来源：http://hz.hongshengwenyu.top/gtkbljhdwm.html

[A06] 字符串转数字
来源：http://hz.sxryk.cn/gtfqowrpbv.html

Py:   int("42"); float("3.14")
来源：http://hz.yueranfly.top/gtpcqdxwvm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jianghu66.top/gtvuzuyosa.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.0kj1m.cn/gtzlqfmtrp.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.shangyingyoupin.top/gtlcuvndnc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zycfv.cn/gtsvqmibml.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xziqi.cn/gtytxsqpwh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.daxiang520.top/gtbuierahc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.pycfn.com/gtsxfgfsks.html

[A07] 数字转字符串
来源：http://hz.ybcxt.top/gtadyxxzjt.html

Py:   str(42)
来源：http://hz.ywan-chungtsiang.top/gtsnpwgjze.html

PHP:  (string) 42; strval(42)
来源：http://hz.ybcxt.top/gtfzlyjtkr.html

JS:   String(42); (42).toString()
来源：http://hz.hnqzz.top/gtkqyrvhml.html

TS:   String(42)
来源：http://hz.quarkkingdee.top/gtuzgpvytk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhengqikj.top/gtunmjnmff.html

Go:   strconv.Itoa(42)
来源：http://hz.pycfn.com/gtehmffbgy.html

Ruby: 42.to_s
来源：http://hz.yongpay.top/gtprfklbre.html

C#:   42.ToString()
来源：http://hz.c1oappe.top/gteqnvsxcm.html

[A08] 取整与四舍五入
来源：http://hz.xuetiantiany.cn/gtuweuiqas.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.cdnleiting.top/gtzjfgnkun.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yuxming.cn/gtyxobknsq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yj202588.top/gtolrefqgs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.gzhubu.top/gtvthnebbu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.tianlin.xyz/gtaozrqvsh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jinyuanbaomall.cn/gtjuuobpiz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.xuetiantiany.cn/gtvluwrwen.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yj20258.top/gtywxzmyfh.html

[A09] 绝对值与最大最小值
来源：http://hz.ppjwa.cn/gthcgakikp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hywenlv.cn/gtyvsvzqtc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.smart0.xyz/gtyjsspbvi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zycfv.cn/gtbzpiuzvr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.gotoacloud.top/gtoqoxsawt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.shuidangran.top/gtzxbndnmp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.gogol.net.cn/gtoejtsyvu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.nwbrower.top/gtzgtleolz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.jinqigufen.top/gtuousjire.html

[A10] 生成随机数
来源：http://hz.xziqi.cn/gtkcagyvrh.html

Py:   import random; random.randint(1, 100)
来源：http://hz.shangyingyoupin.top/gtckawoozw.html

PHP:  random_int(1, 100);
来源：http://hz.yueranfly.top/gtsotbbxkz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.0kj1m.cn/gtjhcitjsk.html


<!-- 参考信息 -->