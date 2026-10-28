代发 wailian999

[U71] PHP：抛出异常
来源：http://hz.aizwys.cn/gtgfzudzvy.html

throw new RuntimeException("失败", 500);
来源：http://hz.shangyingyoupin.top/gtodyqywsi.html

[U72] PHP：写错误日志
来源：http://hz.smart0.xyz/gthesncyxq.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhoulong.xyz/gtvwhchfar.html

[U73] PHP：读取 ini 配置
来源：http://hz.cheryme.top/gtiapmvadk.html

parse_ini_file("config.ini", true)
来源：http://hz.mhx1999.top/gtfecifife.html

[U74] PHP：读取环境变量
来源：http://hz.9152youxi.cn/gtluvenwlu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hnqzz.top/gtojixldnk.html

[U75] PHP：依赖注入
来源：http://hz.fzhhl.top/gthrlrwmfy.html

composer require psr/container
来源：http://hz.ehwqpu.com/gtgohrrweq.html

[U76] PHP：简单路由
来源：http://hz.zhoulong.xyz/gtpvksygyq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ybcxt.top/gtvfpvzsnl.html

[U77] PHP：模板渲染
来源：http://hz.ppjwa.cn/gtfzhjxynt.html

composer require twig/twig
来源：http://hz.hywenlv.cn/gtzsmvikkx.html

[U78] PHP：单元测试
来源：http://hz.xylfe.cn/gtwlappvwq.html

composer require --dev phpunit/phpunit
来源：http://hz.sxryk.cn/gtauzmjsqy.html

[U79] PHP：静态分析
来源：http://hz.hongshengwenyu.top/gtgnpvegei.html

composer require --dev phpstan/phpstan
来源：http://hz.kuanghao11.cn/gtmsunirqz.html

[U80] PHP：代码规范修复
来源：http://hz.xziqi.cn/gtkdglzkxq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.nwbrower.top/gtgxjcjqxs.html

[U81] JS：初始化项目
来源：http://hz.guannengcc.top/gtcqswccrz.html

npm init -y;  npm i express
来源：http://hz.chenjidiqi.icu/gtpdlzawte.html

[U82] JS：package.json 脚本
来源：http://hz.jqgufenzy.top/gtpkpivuwj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sysykeji.top/gtkwndqwis.html

[U83] JS：ES Module 导入导出
来源：http://hz.dianchejie.cn/gthvzjcytq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cqqwz.cn/gtudjncfor.html

[U84] JS：CommonJS 写法
来源：http://hz.cdnleiting.top/gtlefgamos.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cdnleiting.top/gthgbocace.html

[U85] JS：可选链
来源：http://hz.shanyushiyangkeji.top/gtnjwdxpah.html

a?.b?.c
来源：http://hz.havefunace.top/gtxmgydmws.html

[U86] JS：空值合并
来源：http://hz.ybcxt.top/gtpynxfrrk.html

a ?? b
来源：http://hz.wangshuangyany.cn/gtmnweyysz.html

[U87] JS：解构默认值
来源：http://hz.jyoumei.cn/gtevhdihqd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cashguo.top/gtwjffbnpm.html

[U88] JS：对象展开合并
来源：http://hz.yueranfly.top/gtobdaublf.html

{ ...a, ...b }
来源：http://hz.chenjidiqi.icu/gtxavwdytr.html

[U89] JS：数组去重
来源：http://hz.redwolf501.top/gtsqqsaahd.html

[...new Set(arr)]
来源：http://hz.sxryk.cn/gtwvmkmopp.html

[U90] JS：数字数组排序
来源：http://hz.yueranfly.top/gtaofgwcqg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtdivoyrfj.html

[U91] JS：对象键值遍历
来源：http://hz.ppjwa.cn/gtasvbfecw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.smart0.xyz/gthhvpijcz.html

[U92] JS：深拷贝
来源：http://hz.jqgufenzy.top/gtyywnydws.html

structuredClone(obj)
来源：http://hz.gotoacloud.top/gtirznyutr.html

[U93] JS：模板字符串
来源：http://hz.yonumen.top/gtaapthkwx.html

`共 ${n} 条`
来源：http://hz.tanke756.top/gtouqcrxev.html

[U94] JS：箭头函数
来源：http://hz.ywan-chungtsiang.top/gtdcwgizcz.html

const double = x => x * 2;
来源：http://hz.gzhubu.top/gtiaxojujt.html

[U95] JS：Promise 包装
来源：http://hz.cucudq.cn/gtsjmvhylf.html

new Promise((resolve, reject) => {})
来源：http://hz.aibaodan.cn/gtmxmhzwat.html

[U96] JS：async/await 与异常
来源：http://hz.316326.xyz/gtxuyloutz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.wangdashe.top/gtcedjazkf.html

[U97] JS：并发请求
来源：http://hz.nanxinkj.top/gtvdpczibf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtmfjiqfpg.html

[U98] JS：fetch 带 JSON
来源：http://hz.sysykeji.top/gtlgunpgsb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.sufxvd.cn/gtyaasewpf.html

[U99] JS：事件监听
来源：http://hz.0kj1m.cn/gtsyueuons.html

el.addEventListener("click", e => {})
来源：http://hz.xingfuxueyuan.xyz/gthreysxwr.html

[U100] JS：DOM 查询
来源：http://hz.birdmap.top/gtiaekfhfx.html

document.querySelector(".item")
来源：http://hz.zhijiandao.cn/gtuljwjysi.html

[U101] JS：classList 操作
来源：http://hz.zhongyouzk.top/gtglmbqrgl.html

el.classList.toggle("active")
来源：http://hz.nanxinkj.top/gtbkfnqpvh.html

[U102] JS：本地存储
来源：http://hz.vqdsnc.cn/gtvuobxeuz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.quarkkingdee.top/gtrjhztwwz.html

[U103] JS：定时器
来源：http://hz.nanxinkj.top/gtyfiaxeti.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhoulong.xyz/gtrkneqwds.html

[U104] JS：防抖
来源：http://hz.zhengqikj.top/gtqlavusmx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtdoecbleu.html

[U105] JS：节流
来源：http://hz.tian-w.cn/gtxczelegt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gzhubu.top/gtctlzgnvr.html

[U106] JS：日期格式化
来源：http://hz.wangshuangyany.cn/gtozgdjttc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sxryk.cn/gtyerevgov.html

[U107] JS：数字千分位
来源：http://hz.ybcxt.top/gtninihryx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yvedp.cn/gtsunsddjf.html

[U108] JS：随机整数
来源：http://hz.kuanghao11.cn/gtxqccnjff.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.xziqi.cn/gterzyrwsq.html

[U109] JS：数组分组
来源：http://hz.c1oappe.top/gtyuycfrta.html

Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtyxhancow.html

[U110] JS：数组分块
来源：http://hz.gzhubu.top/gtczaofdhs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jianghu66.top/gtnpmnuuii.html

[U111] JS：对象转 Map
来源：http://hz.vqdsnc.cn/gtnybcfqkj.html

new Map(Object.entries(obj))
来源：http://hz.0kj1m.cn/gtfapotduz.html

[U112] JS：字符串补位
来源：http://hz.vqdsnc.cn/gtjywdyuzd.html

"7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtrqmhqcxu.html

[U113] JS：正则替换全部
来源：http://hz.jiagoushi.top/gtfcjleoly.html

s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtxdyxxfge.html

[U114] JS：JSON 深比较
来源：http://hz.52xcode.cn/gtpbkghird.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xingfuxueyuan.xyz/gtgevpiljk.html

[U115] JS：生成 UUID
来源：http://hz.dashuyun.cn/gttckydjij.html

crypto.randomUUID()
来源：http://hz.guannengcc.top/gtnxzgxusq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ydjk.org.cn/gtcxoeyfco.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sufxvd.cn/gtilluvwts.html

[U117] JS：单元测试
来源：http://hz.jqgfzy.top/gtpavpskuw.html

npm i -D vitest;  npx vitest
来源：http://hz.zhiwuduotai.top/gtpupboqwl.html

[U118] JS：开发服务器
来源：http://hz.jlsjyb.cn/gtneeeoxec.html

npm i -D vite;  npx vite
来源：http://hz.guannengcc.top/gtmscwfffh.html

[U119] JS：生产构建
来源：http://hz.vqdsnc.cn/gtfaumyagu.html

npx vite build
来源：http://hz.jiagoushi.top/gtwswbkvxp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.52xcode.cn/gtctjeejda.html

import.meta.env.VITE_API_URL
来源：http://hz.fzhhl.top/gtubexqqgw.html

================================================================================
来源：http://hz.aibaodan.cn/gtzvhvxmry.html

统计汇总
来源：http://hz.chenjidiqi.icu/gtqixwfmss.html

================================================================================
来源：http://hz.hysaishi.cn/gtqrzabkos.html

按语言统计（条）：
来源：http://hz.jinghuilouyu.cn/gtzjpeykzy.html

Python ......... 252
来源：http://hz.yonumen.top/gthbiazqcv.html

PHP ............ 252
来源：http://hz.zhengqikj.top/gtlpvodiba.html

JavaScript ..... 252
来源：http://hz.haohaochexian.top/gtvjroaudi.html

TypeScript ..... 212
来源：http://hz.shanyushiyangkeji.top/gtdczsukhd.html

Java ........... 212
来源：http://hz.svipenyu.cn/gtowkcmyfb.html

Go ............. 212
来源：http://hz.zhixingplan.top/gttcblnzgc.html

Ruby ........... 212
来源：http://hz.havefunace.top/gtakuzsznu.html

C# ............. 212
来源：http://hz.iojbl.cn/gttswavsmw.html

C .............. 30
来源：http://hz.zhengqikj.top/gtjrzsodiw.html

C++ ............ 30
来源：http://hz.daria6918.cn/gttitzjjbh.html

SQL ............ 90
来源：http://hz.yonumen.top/gttjduoypy.html

Bash ........... 80
来源：http://hz.nwbrower.top/gtiyvuiscp.html

Kotlin ......... 15
来源：http://hz.yvedp.cn/gtawvojuez.html

Swift .......... 15
来源：http://hz.cashguo.top/gtgqsfqdvd.html

Lua ............ 10
来源：http://hz.sysykeji.top/gtxpybyvgw.html

Perl ........... 10
来源：http://hz.jqgufenzy.top/gtwqsxweqx.html

Scala .......... 10
来源：http://hz.yj202588.top/gtepbcpazn.html

------------------------------------
来源：http://hz.hywenlv.cn/gtvfxdnqva.html

合计 ........... 2106 条
来源：http://hz.hnxiangtu.top/gtvpyrheec.html

按章节统计：
来源：http://hz.zhoulong.xyz/gtgghfljpa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.nwbrower.top/gtrtovvsvp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sufxvd.cn/gtrdzktuoz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.meibo888.top/gtxhhyntdr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jinghuilouyu.cn/gttopkjbws.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xylfe.cn/gtrltrjyaz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtfbwrezxy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gtlwwomxuw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtnaxlcmyy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtpzrovwcf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jiagoushi.top/gtreyfoeil.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtlocughsg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtyufopahz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtnulxvrsj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yanxiufei.cn/gthklirpzg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.daria6918.cn/gtrqvvgnyt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtxsbmvxvb.html

Q SQL 专题                              90
来源：http://hz.daxiang520.top/gtcbqrgcvb.html

R Bash 专题                             80
来源：http://hz.c1oappe.top/gttnlwyywg.html

S C / C++ 专题                          60
来源：http://hz.wangshuangyany.cn/gtktlkfngl.html

T 其他语言补充                          60
来源：http://hz.xuetiantiany.cn/gtwtvyfity.html

U 高频实用片段                         120
来源：http://hz.c1oappe.top/gtnomosflm.html

------------------------------------
来源：http://hz.redwolf501.top/gtltwjmghi.html

合计                                  2106 条
来源：http://hz.shanyushiyangkeji.top/gtlxtyouuf.html

--------------------------------------------------------------------------------
来源：http://hz.wangshuangyany.cn/gtgmhoonwo.html

使用提醒
来源：http://hz.jianghu66.top/gtjkkfdtju.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtuqfmoeca.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ydzc1.top/gtkmobseyz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jqgufenzy.top/gtvpbjnovm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.svipenyu.cn/gtreswwjrj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yj20258888.top/gttzrnvtfm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xuetiantiany.cn/gtfzhlomyu.html

—— 文件结束 ——
来源：http://hz.gaohongyu789.top/gtnrkbrrnn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtgzicpenx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xinyue.icu/gttrygtnjm.html

Common Programming Examples Cheat Book
来源：http://hz.xylfe.cn/gtclkccnca.html

================================================================================
来源：http://hz.jqgufenzy.top/gthkdswpst.html

【收录内容】
来源：http://hz.tian-w.cn/gtdupbdajo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.iojbl.cn/gtdskwtlrq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cucudq.cn/gtyzxlkffr.html

SQL · Bash · C · C++
来源：http://hz.haohaochexian.top/gtbpdbawkg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ywan-chungtsiang.top/gtncbhkwdg.html

【使用说明】
来源：http://hz.smart0.xyz/gtzcoerkzn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.gaohongyu789.top/gtlbgzkcdp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhiwuduotai.top/gtvgnpvzpl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yuxming.cn/gtsiovhnwa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.guowangkeji.top/gtdwdrmfvr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hnxiangtu.top/gtmhhtmqak.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hnxiangtu.top/gtunmfyhkl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ppjwa.cn/gtstsecrhg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.dianchejie.cn/gtakqkycsf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhijiandao.cn/gtoqenykwh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.vqdsnc.cn/gtdnazedxz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.mhx1999.top/gtdpvxcqep.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yueranfly.top/gtlrrzduqc.html

【文件统计】
来源：http://hz.yj20258888.top/gtstthcldi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.quarkkingdee.top/gtfehmquol.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtwnmftycz.html

目  录
来源：http://hz.nwbrower.top/gtnthnmftf.html

--------------------------------------------------------------------------------
来源：http://hz.meibo888.top/gtygkupjhc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.guannengcc.top/gtjqwsroaq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.52xcode.cn/gtjufejkvv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sxryk.cn/gtoimxukrd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yj202588.top/gtkpihicao.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xinyue.icu/gttqexzwjl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhoulong.xyz/gtpddtyibr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hywenlv.cn/gtrqavhnmb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jianghu66.top/gtpuoeymfh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.dianchejie.cn/gthvwuebbe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ivvv.top/gtrhtfutpt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtoekglert.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gttgrczbte.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtextxeasl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.cashguo.top/gtejqvpgfj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yuxming.cn/gtwrgyieas.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtspjzckzv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nanxuanxn.top/gttjthdjen.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zycfv.cn/gtnsvtbgyo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jiagoushi.top/gtgekzneda.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xinyue.icu/gtrowmudxi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hysaishi.cn/gtjqundcmz.html

================================================================================
来源：http://hz.pycfn.com/gtdjxourzm.html

A. 基础语法与类型
来源：http://hz.nwbrower.top/gtjknidjxa.html

================================================================================
来源：http://hz.sysykeji.top/gtqwjpiksd.html

[A01] Hello World
来源：http://hz.feifeiyinyue.top/gtridljbdf.html

Py:   print("Hello, World!")
来源：http://hz.jinghuilouyu.cn/gtiuqueark.html

PHP:  echo "Hello, World!";
来源：http://hz.xuanzx.com/gtqyfficyh.html

JS:   console.log("Hello, World!");
来源：http://hz.jqgufenzy.top/gtuxwrgqfn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.9152youxi.cn/gtgutkayhf.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhoulong.xyz/gtnwhxzrpw.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xylfe.cn/gtxavmyigx.html

Ruby: puts "Hello, World!"
来源：http://hz.gogol.net.cn/gtsffrvgsq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.shanyushiyangtech.top/gtlhkaxyde.html

[A02] 变量声明与赋值
来源：http://hz.cucudq.cn/gtyupcpcuc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yuanzhike.top/gtbpjhyomn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.kuanghao11.cn/gtcjrdutim.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jinqigfzy.top/gtykvoonfj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.quarkkingdee.top/gtqlkwbsnh.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ybcxt.top/gteajvldpy.html

Go:   name := "Alex"; age := 20
来源：http://hz.fzhhl.top/gtfikaxnpt.html

Ruby: name = "Alex"; age = 20
来源：http://hz.iojbl.cn/gtycaxgeve.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yuanzhike.top/gtffsfjnnm.html

[A03] 常量定义
来源：http://hz.ivvv.top/gtmriitarl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.nanxuanxn.top/gtyrlxodib.html

PHP:  const PI = 3.14159;
来源：http://hz.52xcode.cn/gtcohbfbsw.html

JS:   const PI = 3.14159;
来源：http://hz.yonumen.top/gtvbbpytox.html

TS:   const PI: number = 3.14159;
来源：http://hz.jqgufenzy.top/gtlbunidkb.html

Java: static final double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtbulhdtso.html

Go:   const PI = 3.14159
来源：http://hz.xziqi.cn/gtenwcutmz.html

Ruby: PI = 3.14159
来源：http://hz.nanxinkj.top/gtqyxhjguq.html

C#:   const double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtvtycddxq.html

[A04] 判断变量类型
来源：http://hz.feifeiyinyue.top/gtebqyviwb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nanxinkj.top/gtorbcusfv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.pycfn.com/gtzielnslw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hammf.cn/gtothledre.html

TS:   typeof x; x instanceof Date
来源：http://hz.cqqwz.cn/gtoncexzqs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.52xcode.cn/gtkneyadgp.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hongshengwenyu.top/gtbgprguhu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shzxlz.cn/gtfxcegwhg.html

C#:   x.GetType().Name; x is int
来源：http://hz.sweek.top/gtrufuhjhp.html

[A05] 整数除法与取模
来源：http://hz.xinyue.icu/gtbkhejinp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhaomingkeji.xyz/gtjolxdmca.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.xinyue.icu/gtnnmlmjtu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhengqikj.top/gtalfeduju.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtfcycbkoe.html

Java: 7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gtdoyyakom.html

Go:   7 / 2; 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtmgnaaamp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gtaiyukhve.html

C#:   7 / 2; 7 % 2
来源：http://hz.chenzaomai.com/gtkzeewmzr.html

[A06] 字符串转数字
来源：http://hz.yj20258.top/gtpxjdwdiq.html

Py:   int("42"); float("3.14")
来源：http://hz.yangfankeji.com/gtoisefirs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xingfuxueyuan.xyz/gtjntxyahg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yuxming.cn/gtgvsvwnek.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zhixingplan.top/gtodndpvjo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yanxiufei.cn/gtpsqxlxgq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.tianlin.xyz/gtaznbjrzm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.zhijiandao.cn/gtuzgshyzf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hfpthk.cn/gtoolmyrxj.html

[A07] 数字转字符串
来源：http://hz.pengpengdd.cyou/gtzqopcyvh.html

Py:   str(42)
来源：http://hz.ivvv.top/gtxawcsatg.html

PHP:  (string) 42; strval(42)
来源：http://hz.shanyushiyangtech.top/gtudijynqc.html

JS:   String(42); (42).toString()
来源：http://hz.shanyushiyangtech.top/gtdbekqgix.html

TS:   String(42)
来源：http://hz.nanxuanxn.top/gtxcmziwdp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.tian-w.cn/gtvlulkaga.html

Go:   strconv.Itoa(42)
来源：http://hz.svipenyu.cn/gtkqtklgeu.html

Ruby: 42.to_s
来源：http://hz.jinyuanbaomall.cn/gtsjctxlau.html

C#:   42.ToString()
来源：http://hz.dianchejie.cn/gtqbxgoscs.html

[A08] 取整与四舍五入
来源：http://hz.jlsjyb.cn/gtxrydkzhv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.zycfv.cn/gtrjamfagc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.dashuyun.cn/gtwrfinagy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhijiandao.cn/gtmbsywakz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.c1oappe.top/gtvyymehpg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.cucudq.cn/gtljkqyfxn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.nwbrower.top/gtucwmqpjq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.tanke756.top/gtjbptjffh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yuanzhike.top/gtgbtaitlg.html

[A09] 绝对值与最大最小值
来源：http://hz.jqgfzy.top/gtvofpummq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.vqdsnc.cn/gtqdgpbroi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jlsjyb.cn/gtzvwhlhgn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhixingplan.top/gtrzpnbljd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.cdnleiting.top/gtedkkczuh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.shzxlz.cn/gtgeuodfxs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.cheryme.top/gtpziemhgm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.gogol.net.cn/gtkdlzrdzm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.jinghuilouyu.cn/gtiwsgjkof.html

[A10] 生成随机数
来源：http://hz.pengpengdd.cyou/gtamzkwknx.html

Py:   import random; random.randint(1, 100)
来源：http://hz.quarkkingdee.top/gthzrwphmo.html

PHP:  random_int(1, 100);
来源：http://hz.cucudq.cn/gtxboafbvt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.birdmap.top/gteribdahf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yanxiufei.cn/gtbeqwqrrz.html

Java: new Random().nextInt(100) + 1
来源：http://hz.jiagoushi.top/gtewjuaiso.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.52xcode.cn/gthdgfovwo.html

Ruby: rand(1..100)
来源：http://hz.guannengcc.top/gtmtabexwh.html

C#:   new Random().Next(1, 101)
来源：http://hz.xuetiantiany.cn/gtlxwgfnnd.html

[A11] 条件表达式（三元）
来源：http://hz.yueranfly.top/gtykfjueqi.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.shangyingyoupin.top/gtghxlmyrk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jlsjyb.cn/gtrdpysikr.html


<!-- 参考信息 -->