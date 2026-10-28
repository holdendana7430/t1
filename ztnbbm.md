代发 wailian999

[U87] JS：解构默认值
来源：http://hz.zhaomingkeji.xyz/gtdwtqpyjm.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xuetiantiany.cn/gtsjdhaiht.html

[U88] JS：对象展开合并
来源：http://hz.iojbl.cn/gtzbgplaww.html

{ ...a, ...b }
来源：http://hz.cqqwz.cn/gtwcxvljxv.html

[U89] JS：数组去重
来源：http://hz.ivvv.top/gtzrhxqrbh.html

[...new Set(arr)]
来源：http://hz.cheryme.top/gtejliimxl.html

[U90] JS：数字数组排序
来源：http://hz.yj202588.top/gtpywhkauv.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtajhjmkhu.html

[U91] JS：对象键值遍历
来源：http://hz.tian-w.cn/gttcqorrmh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.316326.xyz/gtbhwdaedh.html

[U92] JS：深拷贝
来源：http://hz.pycfn.com/gtspzexswv.html

structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtzaidpjew.html

[U93] JS：模板字符串
来源：http://hz.jiagoushi.top/gtnjevvekf.html

`共 ${n} 条`
来源：http://hz.ydjk.org.cn/gtgpxruwgb.html

[U94] JS：箭头函数
来源：http://hz.zhijiandao.cn/gtovkirnpe.html

const double = x => x * 2;
来源：http://hz.aizwys.cn/gttsvkxkgw.html

[U95] JS：Promise 包装
来源：http://hz.birdmap.top/gtjnmuqsni.html

new Promise((resolve, reject) => {})
来源：http://hz.smart0.xyz/gtladhchtm.html

[U96] JS：async/await 与异常
来源：http://hz.gaohongyu789.top/gtgxparzts.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtlszdopwv.html

[U97] JS：并发请求
来源：http://hz.yuxming.cn/gtjdlcwxhe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtolkzpcco.html

[U98] JS：fetch 带 JSON
来源：http://hz.shzxlz.cn/gtvcjyrmqb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhoulong.xyz/gtwqvqpwqp.html

[U99] JS：事件监听
来源：http://hz.quarkkingdee.top/gtgihqthgv.html

el.addEventListener("click", e => {})
来源：http://hz.zhongyouzk.top/gtjvjxnhim.html

[U100] JS：DOM 查询
来源：http://hz.ivvv.top/gtoxpquruh.html

document.querySelector(".item")
来源：http://hz.haohaochexian.top/gtqjbmvsyk.html

[U101] JS：classList 操作
来源：http://hz.redwolf501.top/gtqslwpnyv.html

el.classList.toggle("active")
来源：http://hz.yonumen.top/gtpnedygab.html

[U102] JS：本地存储
来源：http://hz.tian-w.cn/gtudasjqfc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.tianlin.xyz/gtehqdvigg.html

[U103] JS：定时器
来源：http://hz.fengsongda.top/gtyzqgodgf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jianghu66.top/gthokzxzlb.html

[U104] JS：防抖
来源：http://hz.kuanghao11.cn/gtjecbufuh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtvarckobc.html

[U105] JS：节流
来源：http://hz.yuxming.cn/gtnybiezre.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.pengpengdd.cyou/gteabrdqzu.html

[U106] JS：日期格式化
来源：http://hz.kuanghao11.cn/gtbesbqvuq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.0kj1m.cn/gtjprcjmfy.html

[U107] JS：数字千分位
来源：http://hz.cqqwz.cn/gtsjiysjsh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ydzc1.top/gtxpiozfab.html

[U108] JS：随机整数
来源：http://hz.yj20258888.top/gtkuoljwvf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.redwolf501.top/gttdbxqtle.html

[U109] JS：数组分组
来源：http://hz.zhaomingkeji.xyz/gtwyndyslg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shangyingyoupin.top/gtniquvnoh.html

[U110] JS：数组分块
来源：http://hz.yangfankeji.com/gtihatkpgx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sysykeji.top/gtspmspipm.html

[U111] JS：对象转 Map
来源：http://hz.jianghu66.top/gtfdwubsov.html

new Map(Object.entries(obj))
来源：http://hz.hnxiangtu.top/gtmtqixgdd.html

[U112] JS：字符串补位
来源：http://hz.ywan-chungtsiang.top/gtpoggbxqb.html

"7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gtxmpgbkbs.html

[U113] JS：正则替换全部
来源：http://hz.hywenlv.cn/gtoccrwhij.html

s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtqhzfryws.html

[U114] JS：JSON 深比较
来源：http://hz.shanyushiyangtech.top/gtrriglkjs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258.top/gtsixxsqsg.html

[U115] JS：生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtrkjxwagf.html

crypto.randomUUID()
来源：http://hz.nwbrower.top/gtbpygetur.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guannengcc.top/gtbcziuags.html

/** @param {string} name */ function f(name) {}
来源：http://hz.daxiang520.top/gtnrnjlvmt.html

[U117] JS：单元测试
来源：http://hz.fengsongda.top/gtxgmicudo.html

npm i -D vitest;  npx vitest
来源：http://hz.yj20258.top/gturrbwgcg.html

[U118] JS：开发服务器
来源：http://hz.nanxuanxn.top/gtohvzjbei.html

npm i -D vite;  npx vite
来源：http://hz.tian-w.cn/gtzsboocos.html

[U119] JS：生产构建
来源：http://hz.cheryme.top/gtibmhffrp.html

npx vite build
来源：http://hz.hnqzz.top/gtaotrbcof.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xuetiantiany.cn/gtbhdyprwi.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangtech.top/gtraisgwrc.html

================================================================================
来源：http://hz.gogol.net.cn/gtknzxdwor.html

统计汇总
来源：http://hz.sysykeji.top/gtafwddsjv.html

================================================================================
来源：http://hz.hammf.cn/gtnuxbusku.html

按语言统计（条）：
来源：http://hz.gzhubu.top/gtryvapowb.html

Python ......... 252
来源：http://hz.ppjwa.cn/gtyiqtbdpu.html

PHP ............ 252
来源：http://hz.daxiang520.top/gtrgrrvone.html

JavaScript ..... 252
来源：http://hz.cucudq.cn/gtsacujjek.html

TypeScript ..... 212
来源：http://hz.chenjidiqi.icu/gtypsdtuqz.html

Java ........... 212
来源：http://hz.ywan-chungtsiang.top/gtzwpgquba.html

Go ............. 212
来源：http://hz.bjfxy.top/gtxrtibuuy.html

Ruby ........... 212
来源：http://hz.smart0.xyz/gtlizjpoaz.html

C# ............. 212
来源：http://hz.yuxming.cn/gtlekxabhy.html

C .............. 30
来源：http://hz.redwolf501.top/gtpddmjqsh.html

C++ ............ 30
来源：http://hz.svipenyu.cn/gtiyerjvhx.html

SQL ............ 90
来源：http://hz.yangfankeji.com/gtxlbzklsi.html

Bash ........... 80
来源：http://hz.fengsongda.top/gtkexuhdvg.html

Kotlin ......... 15
来源：http://hz.xuanzx.com/gtasjhejdw.html

Swift .......... 15
来源：http://hz.cashguo.top/gtalbgzape.html

Lua ............ 10
来源：http://hz.pengpengdd.cyou/gtdmlybhwg.html

Perl ........... 10
来源：http://hz.pengpengdd.cyou/gtljmewoio.html

Scala .......... 10
来源：http://hz.redwolf501.top/gtaikmugqk.html

------------------------------------
来源：http://hz.zhoulong.xyz/gtkkouskag.html

合计 ........... 2106 条
来源：http://hz.jlsjyb.cn/gtrqnyadis.html

按章节统计：
来源：http://hz.ydjk.org.cn/gtsmngoght.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.daxiang520.top/gtsckujabh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.haohaochexian.top/gthxwnbzpl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zycfv.cn/gtdmmvotmv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.daxiang520.top/gtghmnvgly.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jyoumei.cn/gtabfmndrd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.mhx1999.top/gthzsdskqf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtdzwzjatc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.fengsongda.top/gtxnfgdzet.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtkjmoxdnk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yvedp.cn/gtitedumte.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gttksaaszc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtqawsswbm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtjvzfiwhj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.haohaochexian.top/gtxxuffhhx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sweek.top/gtuquyfogg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtgsbaylgz.html

Q SQL 专题                              90
来源：http://hz.yanxiufei.cn/gtuemciqbl.html

R Bash 专题                             80
来源：http://hz.zdqjudy.top/gtpfopeels.html

S C / C++ 专题                          60
来源：http://hz.xziqi.cn/gtrddkdyfp.html

T 其他语言补充                          60
来源：http://hz.xingfuxueyuan.xyz/gtcsmbyndf.html

U 高频实用片段                         120
来源：http://hz.pycfn.com/gtnzdhjjvr.html

------------------------------------
来源：http://hz.feifeiyinyue.top/gtmivajqga.html

合计                                  2106 条
来源：http://hz.tanke756.top/gtxnleyluw.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gtupibmxqf.html

使用提醒
来源：http://hz.yuanzhike.top/gtzxdoxbrp.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258.top/gtpjnveieo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xinyue.icu/gtqzqhizzs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.sufxvd.cn/gtwgyrhsxv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhijiandao.cn/gthioxniri.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.wangdashe.top/gthataicip.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhoulong.xyz/gtbqgxwnov.html

—— 文件结束 ——
来源：http://hz.jinqigufen.top/gtuxigzolz.html

================================================================================
来源：http://hz.zdqjudy.top/gtofamdvqj.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ydjk.org.cn/gtvehfqhpu.html

Common Programming Examples Cheat Book
来源：http://hz.hfpthk.cn/gtfeqgkkeu.html

================================================================================
来源：http://hz.yj20258.top/gtzdvckewu.html

【收录内容】
来源：http://hz.ivvv.top/gtnswhrvtm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.iojbl.cn/gtlytibwmk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cashguo.top/gtujqgokyr.html

SQL · Bash · C · C++
来源：http://hz.yuanzhike.top/gtmvlxfnqh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.daxiang520.top/gtdxeoypsi.html

【使用说明】
来源：http://hz.zhaomingkeji.xyz/gtlawjyioj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yj202588.top/gtniurrnvi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.sxryk.cn/gtnfsfxznc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hnxiangtu.top/gtsczzunba.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xylfe.cn/gtezhsrfen.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yanxiufei.cn/gtrdxtwicq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shzxlz.cn/gtxkisijde.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shanyushiyangkeji.top/gtmwpvuvrn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.cashguo.top/gtnkezqlfs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jyoumei.cn/gtyjdppppy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.hfpthk.cn/gtkooszaoj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhiwuduotai.top/gtjthxdfbp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhixingplan.top/gtyfnhrsht.html

【文件统计】
来源：http://hz.tianlin.xyz/gtzbdbzcje.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.nwbrower.top/gtfxfhfxqz.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtjxklsddz.html

目  录
来源：http://hz.daria6918.cn/gtgilqymbm.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtioxvezmp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhiwuduotai.top/gtxyzgasvh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.chenlongwang.top/gtwfyzmxuv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sufxvd.cn/gttcioakvd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.meibo888.top/gtjzbqgzhe.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jianghu66.top/gttbcpopqp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.tian-w.cn/gtlmoqfbeh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.birdmap.top/gtvlmbhmxx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.svipenyu.cn/gthaupwroi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gtbuodyhms.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.wangshuangyany.cn/gtiogsfzjv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zdqjudy.top/gtkxbuhisb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtvuwfjmsr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtxdhfxdyb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xuanzx.com/gtakrdybfg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yueranfly.top/gtrgfhmtla.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtjmjiijmt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.smart0.xyz/gtaufdauwf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.hfpthk.cn/gtaxylsded.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yj20258888.top/gtzkxmzcyz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gtndccdwho.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangshuangyany.cn/gtjntupwzl.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqrhmoepz.html

A. 基础语法与类型
来源：http://hz.bjfxy.top/gtzpbgylps.html

================================================================================
来源：http://hz.bjfxy.top/gtltfiyggj.html

[A01] Hello World
来源：http://hz.tanke756.top/gtrjccjlgt.html

Py:   print("Hello, World!")
来源：http://hz.snrcjt.cn/gtwsicpiem.html

PHP:  echo "Hello, World!";
来源：http://hz.jinghuilouyu.cn/gtrwtiaefg.html

JS:   console.log("Hello, World!");
来源：http://hz.haohaochexian.top/gtgxxctuaj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hfpthk.cn/gtjynjvpcx.html

Java: System.out.println("Hello, World!");
来源：http://hz.iojbl.cn/gttchzwonb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zdqjudy.top/gtpnkfpccr.html

Ruby: puts "Hello, World!"
来源：http://hz.jqgufenzy.top/gtixcmfgmt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hywenlv.cn/gtdaiwhzdv.html

[A02] 变量声明与赋值
来源：http://hz.guannengcc.top/gtbsnltddk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhijiandao.cn/gtzqedrgzd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jiagoushi.top/gtynylfewk.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.guowangkeji.top/gtjogzilwj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.meibo888.top/gtmoznrokg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ydzc1.top/gtnswtcasy.html

Go:   name := "Alex"; age := 20
来源：http://hz.chenlongwang.top/gtcuiumdja.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hywenlv.cn/gtidjjhxfd.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gzhubu.top/gtcttgacvk.html

[A03] 常量定义
来源：http://hz.gaohongyu789.top/gtpjmlagle.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.316326.xyz/gtngkjluxp.html

PHP:  const PI = 3.14159;
来源：http://hz.shuidangran.top/gtepeezgnp.html

JS:   const PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtcbwrizsz.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhengqikj.top/gtwekdggun.html

Java: static final double PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtginingkm.html

Go:   const PI = 3.14159
来源：http://hz.dianchejie.cn/gtelbzxgey.html

Ruby: PI = 3.14159
来源：http://hz.jlsjyb.cn/gtaycawerv.html

C#:   const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtfblmyelp.html

[A04] 判断变量类型
来源：http://hz.xuetiantiany.cn/gtmuwdkppk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.tianlin.xyz/gtmqbeqdvv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ivvv.top/gttvbjahyv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shanyushiyangkeji.top/gtoksysmvh.html

TS:   typeof x; x instanceof Date
来源：http://hz.tanke756.top/gtgouxxyys.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.smart0.xyz/gtrxblyqit.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.gaohongyu789.top/gtxedxykxc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinyuanbaomall.cn/gttbnedlej.html

C#:   x.GetType().Name; x is int
来源：http://hz.tian-w.cn/gtnzbveqik.html

[A05] 整数除法与取模
来源：http://hz.zhijiandao.cn/gtuirovwxp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yonumen.top/gtmadkcjqy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ybcxt.top/gtdiksohjv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj202588.top/gtegyyrrhh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.quarkkingdee.top/gtkqufeupp.html

Java: 7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtrvszjddh.html

Go:   7 / 2; 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtndmfthum.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.nanxuanxn.top/gtekkheinl.html

C#:   7 / 2; 7 % 2
来源：http://hz.cqqwz.cn/gtgfyfmrcv.html

[A06] 字符串转数字
来源：http://hz.shanyushiyangtech.top/gtvejycasa.html

Py:   int("42"); float("3.14")
来源：http://hz.chenlongwang.top/gthdhrlrbb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yuxming.cn/gtjwsbvcma.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ivvv.top/gtlgbwuiak.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.aizwys.cn/gtbiqzqucn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jlsjyb.cn/gtltrnuoha.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.mhx1999.top/gtslmepjoq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ydjk.org.cn/gtenulzfhp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.shangyingyoupin.top/gtnrqozsuw.html

[A07] 数字转字符串
来源：http://hz.sufxvd.cn/gtfyzayixm.html

Py:   str(42)
来源：http://hz.chenjidiqi.icu/gttohcsvls.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhoulong.xyz/gtaucnfjnx.html

JS:   String(42); (42).toString()
来源：http://hz.jinqigufen.top/gtcycmpqqu.html

TS:   String(42)
来源：http://hz.yuxming.cn/gtvfmjozjt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xuetiantiany.cn/gtlhfedjln.html

Go:   strconv.Itoa(42)
来源：http://hz.quarkkingdee.top/gthfqnwfzd.html

Ruby: 42.to_s
来源：http://hz.zycfv.cn/gtxodfywlx.html

C#:   42.ToString()
来源：http://hz.aizwys.cn/gtybvfpvxq.html

[A08] 取整与四舍五入
来源：http://hz.jinghuilouyu.cn/gtbqqdmlsc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.aizwys.cn/gtcmcugcnj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.aibaodan.cn/gtjnrsxwuq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yj20258.top/gtuoajrcax.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yj20258888.top/gtkenfwoqh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.smart0.xyz/gtvmyfoduf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.ppjwa.cn/gtjcgdrabn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.kuanghao11.cn/gtblfgucxk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtgqdzgqcu.html

[A09] 绝对值与最大最小值
来源：http://hz.jlsjyb.cn/gtqbzvbyun.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yangfankeji.com/gtoyzturgi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.aizwys.cn/gtmacekqev.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhiwuduotai.top/gtgwdlniqy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.fengsongda.top/gtipkamfyw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.yongpay.top/gtrpoddmvg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhiwuduotai.top/gtouooddto.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.c1oappe.top/gtrnxehbnz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hammf.cn/gtgwxxhlth.html

[A10] 生成随机数
来源：http://hz.shanyushiyangkeji.top/gtlbncckej.html

Py:   import random; random.randint(1, 100)
来源：http://hz.aizwys.cn/gtqkuzmgiw.html

PHP:  random_int(1, 100);
来源：http://hz.yanxiufei.cn/gtbxnvukds.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.fengsongda.top/gtxnyiwnsl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shuidangran.top/gtberzhvsg.html

Java: new Random().nextInt(100) + 1
来源：http://hz.daria6918.cn/gtkaagwbky.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zdqjudy.top/gtbbtdbjfw.html

Ruby: rand(1..100)
来源：http://hz.aibaodan.cn/gtsnvpsfwf.html

C#:   new Random().Next(1, 101)
来源：http://hz.pycfn.com/gtlzjahkna.html

[A11] 条件表达式（三元）
来源：http://hz.yj20258.top/gtyhmqwfbv.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.aizwys.cn/gtcdnvctpp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.hfpthk.cn/gturehgqps.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.dianchejie.cn/gtqtgcucri.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.shzxlz.cn/gtshmtwzyw.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yj202588.top/gtlezpaqvc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.nanxuanxn.top/gtounovjkr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.ehwqpu.com/gtvcpqimxi.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.jlsjyb.cn/gtpjtktmux.html

[A12] 字符串插值 / 格式化
来源：http://hz.zdqjudy.top/gtdqleqhpv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.wangdashe.top/gtmxtrbnni.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.shuidangran.top/gttkswdcze.html

JS:   `Hello, ${name}!`
来源：http://hz.chenzaomai.com/gtflpaypgj.html

TS:   `Hello, ${name}!`
来源：http://hz.52xcode.cn/gthnowgoke.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.feifeiyinyue.top/gtirugznds.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.gaohongyu789.top/gtyqplmxqt.html

Ruby: "Hello, #{name}!"
来源：http://hz.yangfankeji.com/gtulgddfef.html

C#:   $"Hello, {name}!"
来源：http://hz.fzhhl.top/gtczmcmaoy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.hysaishi.cn/gtpphivjsh.html

Py:   "第一行\n第二行"
来源：http://hz.pengpengdd.cyou/gtdrkmilsl.html

PHP:  "第一行\n第二行"
来源：http://hz.xuanzx.com/gtsytgqzfc.html

JS:   "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtcusdnllg.html

TS:   "第一行\n第二行"
来源：http://hz.vqdsnc.cn/gtohrfntpt.html

Java: "第一行\n第二行"
来源：http://hz.cheryme.top/gtgxcdeejo.html

Go:   "第一行\n第二行"
来源：http://hz.sxryk.cn/gtcrnkzcry.html

Ruby: "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtqpywlymu.html

C#:   "第一行\n第二行"
来源：http://hz.xinyue.icu/gtshbaxbii.html

[A14] 注释写法
来源：http://hz.jqgufenzy.top/gtongjragw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.c1oappe.top/gtsyndhkvu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.mhx1999.top/gtcjiaihdp.html

JS:   // 单行；/* 多行 */
来源：http://hz.guowangkeji.top/gtnjbijbqo.html

TS:   // 单行；/* 多行 */
来源：http://hz.52xcode.cn/gtvwncolhx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.dianchejie.cn/gtaqybfieg.html

Go:   // 单行；/* 多行 */
来源：http://hz.ywan-chungtsiang.top/gtcxnldfxy.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.hnxiangtu.top/gteorxrses.html


<!-- 参考信息 -->