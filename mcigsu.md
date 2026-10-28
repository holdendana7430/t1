代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://hz.mhx1999.top/gtxskcstxd.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shzxlz.cn/gtmfekdohm.html

[U84] JS：CommonJS 写法
来源：http://hz.chenlongwang.top/gtvdwveyxe.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zycfv.cn/gtaadwzeww.html

[U85] JS：可选链
来源：http://hz.svipenyu.cn/gtinxzbtvl.html

a?.b?.c
来源：http://hz.birdmap.top/gtyzephtau.html

[U86] JS：空值合并
来源：http://hz.zhengqikj.top/gtbkcqeugc.html

a ?? b
来源：http://hz.xingfuxueyuan.xyz/gtvwbpejoe.html

[U87] JS：解构默认值
来源：http://hz.shanyushiyangkeji.top/gtuwqnekfu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gotoacloud.top/gtngmccmlo.html

[U88] JS：对象展开合并
来源：http://hz.quarkkingdee.top/gtqnsstcpj.html

{ ...a, ...b }
来源：http://hz.316326.xyz/gtyiullvrb.html

[U89] JS：数组去重
来源：http://hz.nanxinkj.top/gtqpyuvlwr.html

[...new Set(arr)]
来源：http://hz.havefunace.top/gtxuhqahjs.html

[U90] JS：数字数组排序
来源：http://hz.sxryk.cn/gtnkztbsct.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtwrvbntak.html

[U91] JS：对象键值遍历
来源：http://hz.tanke756.top/gtcqfgndhz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shanyushiyangkeji.top/gtwkyxacgh.html

[U92] JS：深拷贝
来源：http://hz.kuanghao11.cn/gthdsmbbtx.html

structuredClone(obj)
来源：http://hz.sweek.top/gthgdnklva.html

[U93] JS：模板字符串
来源：http://hz.fengsongda.top/gtlmpadpac.html

`共 ${n} 条`
来源：http://hz.316326.xyz/gtxwmrbkir.html

[U94] JS：箭头函数
来源：http://hz.wangshuangyany.cn/gtidvzbpxm.html

const double = x => x * 2;
来源：http://hz.guannengcc.top/gtlilmyeit.html

[U95] JS：Promise 包装
来源：http://hz.cheryme.top/gtlwttxiur.html

new Promise((resolve, reject) => {})
来源：http://hz.chenzaomai.com/gtukiurqhx.html

[U96] JS：async/await 与异常
来源：http://hz.zdqjudy.top/gtmvnfhrmk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigufen.top/gtwtljdbtz.html

[U97] JS：并发请求
来源：http://hz.jqgfzy.top/gtcixeqyds.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtgsyyduev.html

[U98] JS：fetch 带 JSON
来源：http://hz.yonumen.top/gtfgnhysue.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hongshengwenyu.top/gtjiattfiu.html

[U99] JS：事件监听
来源：http://hz.xylfe.cn/gtzqmijson.html

el.addEventListener("click", e => {})
来源：http://hz.jqgfzy.top/gtsspvkkum.html

[U100] JS：DOM 查询
来源：http://hz.zhixingplan.top/gtusytvpcy.html

document.querySelector(".item")
来源：http://hz.xingfuxueyuan.xyz/gtmosnktcs.html

[U101] JS：classList 操作
来源：http://hz.xylfe.cn/gtnqcfqtvs.html

el.classList.toggle("active")
来源：http://hz.zhongyouzk.top/gtlppsftnh.html

[U102] JS：本地存储
来源：http://hz.sxryk.cn/gtqnnttowx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zdqjudy.top/gtmdsduvje.html

[U103] JS：定时器
来源：http://hz.jyoumei.cn/gtzqezrxpo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shzxlz.cn/gtlkbvthzo.html

[U104] JS：防抖
来源：http://hz.shzxlz.cn/gtvaeugtsk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtfvcfogry.html

[U105] JS：节流
来源：http://hz.havefunace.top/gtslvsvudf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ywan-chungtsiang.top/gtzceylvsi.html

[U106] JS：日期格式化
来源：http://hz.gotoacloud.top/gthdjwwuzp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhongyouzk.top/gtdgswtulq.html

[U107] JS：数字千分位
来源：http://hz.wangshuangyany.cn/gtezhgngaz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gaohongyu789.top/gthbkwwgtk.html

[U108] JS：随机整数
来源：http://hz.daria6918.cn/gtxpddvzit.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hysaishi.cn/gtgvrgyvub.html

[U109] JS：数组分组
来源：http://hz.feifeiyinyue.top/gtipssolxg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtrhwntzam.html

[U110] JS：数组分块
来源：http://hz.xingfuxueyuan.xyz/gtjadcptyh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.redwolf501.top/gtapchdcgv.html

[U111] JS：对象转 Map
来源：http://hz.fengsongda.top/gtdkqhvkac.html

new Map(Object.entries(obj))
来源：http://hz.jqgfzy.top/gtuzibgikv.html

[U112] JS：字符串补位
来源：http://hz.snrcjt.cn/gtrqojsyqt.html

"7".padStart(3, "0")
来源：http://hz.cashguo.top/gtjhygexfz.html

[U113] JS：正则替换全部
来源：http://hz.gzhubu.top/gtxpmlfxmo.html

s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtdprbjldi.html

[U114] JS：JSON 深比较
来源：http://hz.chenlongwang.top/gtzjypkniq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtjyxeznay.html

[U115] JS：生成 UUID
来源：http://hz.zhijiandao.cn/gtbyittjtj.html

crypto.randomUUID()
来源：http://hz.meibo888.top/gtemdvtqel.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinqigfzy.top/gtncveaozq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.aizwys.cn/gthabqhbbi.html

[U117] JS：单元测试
来源：http://hz.mhx1999.top/gtyhouqolq.html

npm i -D vitest;  npx vitest
来源：http://hz.nanxuanxn.top/gtrqinffgh.html

[U118] JS：开发服务器
来源：http://hz.zdqjudy.top/gtostvrsfz.html

npm i -D vite;  npx vite
来源：http://hz.wangshuangyany.cn/gtqfgzazpg.html

[U119] JS：生产构建
来源：http://hz.bjfxy.top/gtzyogytuq.html

npx vite build
来源：http://hz.feifeiyinyue.top/gtmpuxtytd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.haohaochexian.top/gtxjasbmfi.html

import.meta.env.VITE_API_URL
来源：http://hz.jlsjyb.cn/gtmnrjlssq.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdkcfvuef.html

统计汇总
来源：http://hz.yuanzhike.top/gtlkwtxubj.html

================================================================================
来源：http://hz.wangdashe.top/gtqxtmgxaj.html

按语言统计（条）：
来源：http://hz.cashguo.top/gtbavldblr.html

Python ......... 252
来源：http://hz.guannengcc.top/gtaqreylqt.html

PHP ............ 252
来源：http://hz.yvedp.cn/gtlkuxunix.html

JavaScript ..... 252
来源：http://hz.jyoumei.cn/gtmdrtthlt.html

TypeScript ..... 212
来源：http://hz.shangyingyoupin.top/gtzkyzxtas.html

Java ........... 212
来源：http://hz.hysaishi.cn/gtensbepst.html

Go ............. 212
来源：http://hz.vqdsnc.cn/gtjponsusi.html

Ruby ........... 212
来源：http://hz.guannengcc.top/gtdqwuvxtq.html

C# ............. 212
来源：http://hz.zdqjudy.top/gtavglcpoo.html

C .............. 30
来源：http://hz.snrcjt.cn/gteyjhvnll.html

C++ ............ 30
来源：http://hz.ivvv.top/gtscuvmwil.html

SQL ............ 90
来源：http://hz.gotoacloud.top/gtrcbsxsbe.html

Bash ........... 80
来源：http://hz.ywan-chungtsiang.top/gtgyfctcxh.html

Kotlin ......... 15
来源：http://hz.zhaomingkeji.xyz/gtatsjwciv.html

Swift .......... 15
来源：http://hz.nanxinkj.top/gtrsqeuxjw.html

Lua ............ 10
来源：http://hz.kuanghao11.cn/gttqbuevgb.html

Perl ........... 10
来源：http://hz.xuetiantiany.cn/gtrjorzvjo.html

Scala .......... 10
来源：http://hz.hongshengwenyu.top/gtdjrcadnh.html

------------------------------------
来源：http://hz.dianchejie.cn/gtdccvnisx.html

合计 ........... 2106 条
来源：http://hz.gotoacloud.top/gtibpmirfc.html

按章节统计：
来源：http://hz.jqgfzy.top/gtdbvmaxis.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.smart0.xyz/gtfccgvuov.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.kuanghao11.cn/gtxgqqcdav.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zycfv.cn/gtldjiqxhu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jyoumei.cn/gtwgsvneoj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.havefunace.top/gtkqaipmtk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigfzy.top/gtwsqdpjig.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gthwufkeoc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yvedp.cn/gtkfvbcqwg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtgyskyfvi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinyuanbaomall.cn/gtvcevzlef.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtuqedoqsk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtqdhazbwf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtrkzvzmzi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.pycfn.com/gthrtwoyut.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhoulong.xyz/gtvrptuzoy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtuzmlfuou.html

Q SQL 专题                              90
来源：http://hz.hnxiangtu.top/gttlmxqcja.html

R Bash 专题                             80
来源：http://hz.bjfxy.top/gtwoonxgbw.html

S C / C++ 专题                          60
来源：http://hz.tian-w.cn/gtcwjjdrzl.html

T 其他语言补充                          60
来源：http://hz.iojbl.cn/gtqcjpgliy.html

U 高频实用片段                         120
来源：http://hz.smart0.xyz/gtjktuqxku.html

------------------------------------
来源：http://hz.yangfankeji.com/gtlcrmrvru.html

合计                                  2106 条
来源：http://hz.nanxuanxn.top/gtepmbijjr.html

--------------------------------------------------------------------------------
来源：http://hz.xinyue.icu/gtyjrxfqsh.html

使用提醒
来源：http://hz.0kj1m.cn/gtglspzkgb.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtsnjloiyg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.aizwys.cn/gtmvsdqtro.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhijiandao.cn/gtkdtqsroz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ydjk.org.cn/gtoiqpcstk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ywan-chungtsiang.top/gtqxpolxlg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.guowangkeji.top/gttwjrjrzr.html

—— 文件结束 ——
来源：http://hz.yvedp.cn/gtbjhubhxh.html

================================================================================
来源：http://hz.jinqigufen.top/gtkxqrvemi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jinqigfzy.top/gtctkvwmho.html

Common Programming Examples Cheat Book
来源：http://hz.c1oappe.top/gtjjyjwzml.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqpppnoco.html

【收录内容】
来源：http://hz.hysaishi.cn/gtjrsnkuol.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hywenlv.cn/gtulxrnzod.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jinqigfzy.top/gtaopegdjn.html

SQL · Bash · C · C++
来源：http://hz.shzxlz.cn/gttgjvhvhz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sweek.top/gtlbaxwnvn.html

【使用说明】
来源：http://hz.iojbl.cn/gtxqgickeb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hammf.cn/gtbrbwqmvs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ybcxt.top/gtucuglxdp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258888.top/gtvwodweoi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xuetiantiany.cn/gtskhrrzhb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.dianchejie.cn/gtipedrswm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jinqigufen.top/gtbctevwzg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shzxlz.cn/gteujjdgft.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.c1oappe.top/gtipregbho.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nanxuanxn.top/gtxoqsafmz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhiwuduotai.top/gtbdwvosfg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jiagoushi.top/gtsbvrzzcb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tian-w.cn/gtxeurvnux.html

【文件统计】
来源：http://hz.quarkkingdee.top/gtdwjkyyzs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xuetiantiany.cn/gtlanbtejm.html

--------------------------------------------------------------------------------
来源：http://hz.yangfankeji.com/gtjfsdxrxz.html

目  录
来源：http://hz.cashguo.top/gthzopzubo.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gtbpemccdw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhongyouzk.top/gtvshxsbej.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.andypj.xyz/gttziwemfp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.mhx1999.top/gtsinbkyxu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.aizwys.cn/gtgsohwafc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shanyushiyangtech.top/gtvxjoxylb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.birdmap.top/gtbhsdurkk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cqqwz.cn/gtlunvyuxd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gttuwdqdua.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.sweek.top/gtbgtwgqgz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cqqwz.cn/gtvtnbsebx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtidvyfscx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtbbcyxmpc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhongyouzk.top/gtcniwoobs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtdxyuotdj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhixingplan.top/gtvvttsesn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gthyaujrlo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jyoumei.cn/gtrgajuxjw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinqigufen.top/gteurlific.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cashguo.top/gtwhwiywxi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xinyue.icu/gtfxxrqavr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnxiangtu.top/gtxctjmjzh.html

================================================================================
来源：http://hz.xylfe.cn/gtunljeccs.html

A. 基础语法与类型
来源：http://hz.jiagoushi.top/gtvtfrpcbd.html

================================================================================
来源：http://hz.yangfankeji.com/gtncpjgbxa.html

[A01] Hello World
来源：http://hz.iojbl.cn/gtsnqgedkw.html

Py:   print("Hello, World!")
来源：http://hz.yj202588.top/gthqjntglg.html

PHP:  echo "Hello, World!";
来源：http://hz.tanke756.top/gtpseqhljp.html

JS:   console.log("Hello, World!");
来源：http://hz.tanke756.top/gtoyeobkgp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.sysykeji.top/gtomuymnnh.html

Java: System.out.println("Hello, World!");
来源：http://hz.wangshuangyany.cn/gtxgpbrkyv.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hnxiangtu.top/gttmpujrxk.html

Ruby: puts "Hello, World!"
来源：http://hz.aizwys.cn/gtudqyiygf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhaomingkeji.xyz/gtewbmdbyq.html

[A02] 变量声明与赋值
来源：http://hz.dianchejie.cn/gtfdliipss.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jinqigfzy.top/gtezfikxkm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ydzc1.top/gtorbzykwo.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jianghu66.top/gtyeqtjcww.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.svipenyu.cn/gtsoiierhu.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.dianchejie.cn/gtsfgyghpm.html

Go:   name := "Alex"; age := 20
来源：http://hz.xinyue.icu/gtkwiupgfb.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinqigufen.top/gtftqqfkuc.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.316326.xyz/gtuubkbuuo.html

[A03] 常量定义
来源：http://hz.shanyushiyangkeji.top/gtumejlnom.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yuxming.cn/gtjllwtquo.html

PHP:  const PI = 3.14159;
来源：http://hz.wangdashe.top/gtxiunycqy.html

JS:   const PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtmfhmbphc.html

TS:   const PI: number = 3.14159;
来源：http://hz.ydzc1.top/gtuvrulmoc.html

Java: static final double PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtwtssufls.html

Go:   const PI = 3.14159
来源：http://hz.yuxming.cn/gtemffgvxx.html

Ruby: PI = 3.14159
来源：http://hz.jinghuilouyu.cn/gtyupkpokn.html

C#:   const double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtrqoigjbk.html

[A04] 判断变量类型
来源：http://hz.jianghu66.top/gtmiqlwkib.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.havefunace.top/gtuznmpzsi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zdqjudy.top/gtwrytsbts.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jianghu66.top/gtorujivbq.html

TS:   typeof x; x instanceof Date
来源：http://hz.jqgufenzy.top/gtjcjtrgcs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.chenzaomai.com/gtjqyggfnu.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hysaishi.cn/gtmlrlutak.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.ivvv.top/gtpjgxnpqp.html

C#:   x.GetType().Name; x is int
来源：http://hz.yvedp.cn/gtamwyrmwj.html

[A05] 整数除法与取模
来源：http://hz.xylfe.cn/gtprjuyrdo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.gotoacloud.top/gtbkttqokw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zdqjudy.top/gtaptmjrxk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xziqi.cn/gtbvbvowdq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenjidiqi.icu/gtsnhphnjr.html

Java: 7 / 2; 7 % 2
来源：http://hz.nanxinkj.top/gtmoipyceo.html

Go:   7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtpmwpwcis.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.andypj.xyz/gtfefjnoqg.html

C#:   7 / 2; 7 % 2
来源：http://hz.kuanghao11.cn/gtxrvnhdez.html

[A06] 字符串转数字
来源：http://hz.snrcjt.cn/gtedjmfjpt.html

Py:   int("42"); float("3.14")
来源：http://hz.jqgufenzy.top/gtnophlymx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhiwuduotai.top/gtuehxhbvi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.wangdashe.top/gtxczzrcvo.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jinyuanbaomall.cn/gtqgrytdtc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ivvv.top/gtozsnfmdi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xinyue.icu/gtzdcwevrn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.0kj1m.cn/gtexoqegyt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jinqigufen.top/gtcwhhywqw.html

[A07] 数字转字符串
来源：http://hz.nanxinkj.top/gtnblrownd.html

Py:   str(42)
来源：http://hz.hnqzz.top/gtnftrdnrr.html

PHP:  (string) 42; strval(42)
来源：http://hz.9152youxi.cn/gtrbwjdokp.html

JS:   String(42); (42).toString()
来源：http://hz.9152youxi.cn/gtwctadmkt.html

TS:   String(42)
来源：http://hz.sxryk.cn/gttxaqjcsk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yanxiufei.cn/gtjozxftle.html

Go:   strconv.Itoa(42)
来源：http://hz.quarkkingdee.top/gtwdcjsrjp.html

Ruby: 42.to_s
来源：http://hz.meibo888.top/gtsjvlhayy.html

C#:   42.ToString()
来源：http://hz.sufxvd.cn/gtudymfqqh.html

[A08] 取整与四舍五入
来源：http://hz.hnqzz.top/gtldpicbic.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jinghuilouyu.cn/gtwtefmges.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.ydzc1.top/gtfgcrnezs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jqgfzy.top/gtfbvfnlld.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jlsjyb.cn/gtemyajbqd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.ywan-chungtsiang.top/gtbpifgmdc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hywenlv.cn/gtdzitlkmx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.sweek.top/gtmfvhlvdp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.sysykeji.top/gtstrrlxxf.html

[A09] 绝对值与最大最小值
来源：http://hz.vqdsnc.cn/gtmxybejls.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cucudq.cn/gtdbxtoven.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.sysykeji.top/gteqjgqjqw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.wangshuangyany.cn/gtwkjnevpn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.fzhhl.top/gtaafmbexv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.sysykeji.top/gtokgisxgc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yj202588.top/gticzosvqk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.yj20258888.top/gtinrolnqh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ybcxt.top/gtxdyyzisj.html

[A10] 生成随机数
来源：http://hz.c1oappe.top/gtclkcqwds.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zhixingplan.top/gtnyomdsuj.html

PHP:  random_int(1, 100);
来源：http://hz.daria6918.cn/gtcfpwdcwd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.aibaodan.cn/gtwlrwzgwj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.xziqi.cn/gtjjljvblg.html

Java: new Random().nextInt(100) + 1
来源：http://hz.aizwys.cn/gtspxeosit.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.daria6918.cn/gtqbefuxwm.html

Ruby: rand(1..100)
来源：http://hz.vqdsnc.cn/gtqrxnhwtx.html

C#:   new Random().Next(1, 101)
来源：http://hz.guowangkeji.top/gttfzxskfy.html

[A11] 条件表达式（三元）
来源：http://hz.yj202588.top/gtcvivxohv.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.52xcode.cn/gtrcmaowqh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gtquloqkpe.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jinyuanbaomall.cn/gtkgwigzmh.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.yueranfly.top/gtimpdxnlz.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.nanxinkj.top/gtsamsbonv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.gotoacloud.top/gtlfpoimze.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.shzxlz.cn/gtmfcjqyax.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.jiagoushi.top/gtplfburju.html

[A12] 字符串插值 / 格式化
来源：http://hz.pycfn.com/gtnkhcatkh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.cdnleiting.top/gtzveksbzz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.chenlongwang.top/gtifkzwgbi.html

JS:   `Hello, ${name}!`
来源：http://hz.smart0.xyz/gtrkvnjhuf.html

TS:   `Hello, ${name}!`
来源：http://hz.zhoulong.xyz/gtpewbdjdc.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.tanke756.top/gtwbitenyr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.c1oappe.top/gtdrvfpncg.html

Ruby: "Hello, #{name}!"
来源：http://hz.zhixingplan.top/gtqieuicue.html

C#:   $"Hello, {name}!"
来源：http://hz.hywenlv.cn/gtgbmhrldv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jinghuilouyu.cn/gtlqlyohnm.html

Py:   "第一行\n第二行"
来源：http://hz.sufxvd.cn/gtebhsaovn.html

PHP:  "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtqkddckhn.html

JS:   "第一行\n第二行"
来源：http://hz.tanke756.top/gtonxkshgu.html

TS:   "第一行\n第二行"
来源：http://hz.vqdsnc.cn/gtqkqwdmua.html

Java: "第一行\n第二行"
来源：http://hz.0kj1m.cn/gtleodchur.html

Go:   "第一行\n第二行"
来源：http://hz.wangshuangyany.cn/gttakigtvk.html

Ruby: "第一行\n第二行"
来源：http://hz.andypj.xyz/gtxuadzwxu.html

C#:   "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtjwmmclbs.html


<!-- 参考信息 -->