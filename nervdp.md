代发 wailian999

[U87] JS：解构默认值
来源：http://hz.ydjk.org.cn/gtxklyvnmx.html

const { a = 1, b = 2 } = obj;
来源：http://hz.dianchejie.cn/gtbeznjkzg.html

[U88] JS：对象展开合并
来源：http://hz.aizwys.cn/gtaamejamp.html

{ ...a, ...b }
来源：http://hz.yanxiufei.cn/gtsrldydqf.html

[U89] JS：数组去重
来源：http://hz.tian-w.cn/gtpqlescvo.html

[...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtjzhcoqkr.html

[U90] JS：数字数组排序
来源：http://hz.vqdsnc.cn/gtrkuqifea.html

[...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gttlpgersb.html

[U91] JS：对象键值遍历
来源：http://hz.zhiwuduotai.top/gtuvbenctc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.mhx1999.top/gtlzhoddrc.html

[U92] JS：深拷贝
来源：http://hz.xylfe.cn/gtgzjwpgzh.html

structuredClone(obj)
来源：http://hz.sysykeji.top/gtnefjqrfo.html

[U93] JS：模板字符串
来源：http://hz.kuanghao11.cn/gtvqkneqme.html

`共 ${n} 条`
来源：http://hz.jinqigufen.top/gtnlwwshys.html

[U94] JS：箭头函数
来源：http://hz.iojbl.cn/gtjbkivpvh.html

const double = x => x * 2;
来源：http://hz.gotoacloud.top/gtlcftefuf.html

[U95] JS：Promise 包装
来源：http://hz.andypj.xyz/gttyfxtkgd.html

new Promise((resolve, reject) => {})
来源：http://hz.yangfankeji.com/gthhmphkpk.html

[U96] JS：async/await 与异常
来源：http://hz.wangdashe.top/gtokngksju.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtkhgmvddq.html

[U97] JS：并发请求
来源：http://hz.xuetiantiany.cn/gtdwzjuvxz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtkjppigxh.html

[U98] JS：fetch 带 JSON
来源：http://hz.meibo888.top/gtfifocrmm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.chenjidiqi.icu/gtjnpfzwqk.html

[U99] JS：事件监听
来源：http://hz.feifeiyinyue.top/gtzwfdztyw.html

el.addEventListener("click", e => {})
来源：http://hz.316326.xyz/gtnrxraimi.html

[U100] JS：DOM 查询
来源：http://hz.hammf.cn/gthotdmsds.html

document.querySelector(".item")
来源：http://hz.zhongyouzk.top/gtokbzqala.html

[U101] JS：classList 操作
来源：http://hz.wangdashe.top/gtygklplcj.html

el.classList.toggle("active")
来源：http://hz.hysaishi.cn/gtgvtimtiy.html

[U102] JS：本地存储
来源：http://hz.jinyuanbaomall.cn/gtpcqogojf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.dianchejie.cn/gtbvrtvfgh.html

[U103] JS：定时器
来源：http://hz.gzhubu.top/gtpajnmmkr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aizwys.cn/gtfuvjeseb.html

[U104] JS：防抖
来源：http://hz.ppjwa.cn/gtpodgpqab.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtsgkmpbai.html

[U105] JS：节流
来源：http://hz.zdqjudy.top/gtamznlawz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yongpay.top/gtduhcqkgt.html

[U106] JS：日期格式化
来源：http://hz.wangdashe.top/gttdqshtyl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhengqikj.top/gtoagjzhdi.html

[U107] JS：数字千分位
来源：http://hz.chenzaomai.com/gtacotidib.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xinyue.icu/gtumioqzfn.html

[U108] JS：随机整数
来源：http://hz.chenjidiqi.icu/gtwojpfviv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sxryk.cn/gtunxozadh.html

[U109] JS：数组分组
来源：http://hz.daxiang520.top/gtahsxhzux.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gaohongyu789.top/gtcjzfzqdi.html

[U110] JS：数组分块
来源：http://hz.yj20258888.top/gtqwoibbwa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gaohongyu789.top/gtinyvtmwa.html

[U111] JS：对象转 Map
来源：http://hz.svipenyu.cn/gtgthtfrkh.html

new Map(Object.entries(obj))
来源：http://hz.shuidangran.top/gtcjywjics.html

[U112] JS：字符串补位
来源：http://hz.xingfuxueyuan.xyz/gtnxwudmkz.html

"7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtrvwatryz.html

[U113] JS：正则替换全部
来源：http://hz.shuidangran.top/gtxsdebkpd.html

s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtrgrtmtuy.html

[U114] JS：JSON 深比较
来源：http://hz.vqdsnc.cn/gtqygtkzvt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtbmlppmuc.html

[U115] JS：生成 UUID
来源：http://hz.yj20258888.top/gtftentygc.html

crypto.randomUUID()
来源：http://hz.fengsongda.top/gtgkoenqio.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yj20258.top/gtvbehahob.html

/** @param {string} name */ function f(name) {}
来源：http://hz.pycfn.com/gtvfeuphwi.html

[U117] JS：单元测试
来源：http://hz.bjfxy.top/gtaixqkape.html

npm i -D vitest;  npx vitest
来源：http://hz.wangdashe.top/gtehieugiq.html

[U118] JS：开发服务器
来源：http://hz.xinyue.icu/gtyhqqdcof.html

npm i -D vite;  npx vite
来源：http://hz.sysykeji.top/gttgefgnwp.html

[U119] JS：生产构建
来源：http://hz.zdqjudy.top/gtnygytlzz.html

npx vite build
来源：http://hz.jlsjyb.cn/gtitxvrbec.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenjidiqi.icu/gtepwzpffl.html

import.meta.env.VITE_API_URL
来源：http://hz.havefunace.top/gtafbxzxqj.html

================================================================================
来源：http://hz.xuetiantiany.cn/gthpwujnpb.html

统计汇总
来源：http://hz.c1oappe.top/gtfcmlzuic.html

================================================================================
来源：http://hz.hfpthk.cn/gtudokbxth.html

按语言统计（条）：
来源：http://hz.smart0.xyz/gtktbxhfhk.html

Python ......... 252
来源：http://hz.andypj.xyz/gtqycqzxiu.html

PHP ............ 252
来源：http://hz.chenzaomai.com/gtbyuazgvq.html

JavaScript ..... 252
来源：http://hz.shuidangran.top/gtzbhqjnkw.html

TypeScript ..... 212
来源：http://hz.jianghu66.top/gtyxonoyjm.html

Java ........... 212
来源：http://hz.jinyuanbaomall.cn/gtqodbrdbb.html

Go ............. 212
来源：http://hz.hammf.cn/gtxuukphgn.html

Ruby ........... 212
来源：http://hz.cashguo.top/gtjisqmlia.html

C# ............. 212
来源：http://hz.gogol.net.cn/gtwuuxciro.html

C .............. 30
来源：http://hz.iojbl.cn/gtayzkzspu.html

C++ ............ 30
来源：http://hz.hongshengwenyu.top/gtkthtpihz.html

SQL ............ 90
来源：http://hz.guannengcc.top/gtuhqauhyq.html

Bash ........... 80
来源：http://hz.fengsongda.top/gtvrdupobp.html

Kotlin ......... 15
来源：http://hz.yj20258888.top/gtgjzoyguw.html

Swift .......... 15
来源：http://hz.hammf.cn/gtnfjvzqrn.html

Lua ............ 10
来源：http://hz.svipenyu.cn/gtjdgipqun.html

Perl ........... 10
来源：http://hz.snrcjt.cn/gtmhynlirp.html

Scala .......... 10
来源：http://hz.haohaochexian.top/gtohtlgztt.html

------------------------------------
来源：http://hz.wangdashe.top/gtcfykfmlp.html

合计 ........... 2106 条
来源：http://hz.cqqwz.cn/gtnzcmqrgu.html

按章节统计：
来源：http://hz.shangyingyoupin.top/gtrsjpsbad.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangdashe.top/gtecbyezkb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtinrtxwjm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtjfayfdwk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.c1oappe.top/gtlojmpxvl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.svipenyu.cn/gtauiiebpd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtntzwgfjm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yuxming.cn/gtkwdukkka.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.52xcode.cn/gtamrtpxfh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gtgivjaxqz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yvedp.cn/gtvxjncizh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtokxaqbom.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtxpoyxqkx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtjkbhxapl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinghuilouyu.cn/gtjiaprqha.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tian-w.cn/gtuqufiaac.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtdykaufhd.html

Q SQL 专题                              90
来源：http://hz.bjfxy.top/gtalurgphm.html

R Bash 专题                             80
来源：http://hz.wangdashe.top/gtaddlktzu.html

S C / C++ 专题                          60
来源：http://hz.pengpengdd.cyou/gtaiqqmhph.html

T 其他语言补充                          60
来源：http://hz.xuetiantiany.cn/gthsfvuwiz.html

U 高频实用片段                         120
来源：http://hz.ppjwa.cn/gtqqiwwlex.html

------------------------------------
来源：http://hz.yj20258.top/gtlprukxed.html

合计                                  2106 条
来源：http://hz.shanyushiyangtech.top/gtrrkknzxy.html

--------------------------------------------------------------------------------
来源：http://hz.nanxuanxn.top/gtpwpdogpv.html

使用提醒
来源：http://hz.nanxuanxn.top/gtapenjbso.html

--------------------------------------------------------------------------------
来源：http://hz.jqgfzy.top/gthofzjqcv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ywan-chungtsiang.top/gtzskhntht.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.9152youxi.cn/gtadktxjkf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sufxvd.cn/gtuldjqkev.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sweek.top/gtyjpomkhg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hywenlv.cn/gtlqhfzzev.html

—— 文件结束 ——
来源：http://hz.nanxuanxn.top/gtsjtdadlx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmqhjjsas.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.chenzaomai.com/gtdviqlhcf.html

Common Programming Examples Cheat Book
来源：http://hz.smart0.xyz/gtqtmhtucy.html

================================================================================
来源：http://hz.zycfv.cn/gtjpwvnblm.html

【收录内容】
来源：http://hz.9152youxi.cn/gtvdqjqavp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zdqjudy.top/gtqowfuwgi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.redwolf501.top/gtthxjwsnz.html

SQL · Bash · C · C++
来源：http://hz.tian-w.cn/gticsyozhd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.pengpengdd.cyou/gtzznvqrur.html

【使用说明】
来源：http://hz.jyoumei.cn/gtjubdcbmf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.nanxuanxn.top/gtidoegvjv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.bjfxy.top/gtxfdywjnl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ydzc1.top/gtfccpgdzp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yanxiufei.cn/gtnevffnjn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jlsjyb.cn/gtqnqvjlwn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.dianchejie.cn/gttmifqhmo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hfpthk.cn/gtcgwxkfgt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.quarkkingdee.top/gtoksgjaud.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.bjfxy.top/gtmcmzmbhd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.havefunace.top/gtuvqdatsf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.dianchejie.cn/gtdyhjkrdl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yj20258888.top/gtwuzmccmb.html

【文件统计】
来源：http://hz.cheryme.top/gtoefbeelp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhixingplan.top/gtcwrrwnco.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gthyzeneef.html

目  录
来源：http://hz.jinghuilouyu.cn/gthrrutkov.html

--------------------------------------------------------------------------------
来源：http://hz.aizwys.cn/gtcgwurogo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.fengsongda.top/gtfxyfzzoh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinyuanbaomall.cn/gtwcytbejf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hnqzz.top/gtmtstkzng.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.cqqwz.cn/gtioaxesrc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hysaishi.cn/gtbdninptm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinyuanbaomall.cn/gtdresmbli.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cdnleiting.top/gtcwhmqdmq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.aibaodan.cn/gtxdnajquz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zdqjudy.top/gtvpkpqmzl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.sweek.top/gthhcchmbb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gtucrqmraq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gtjnqpsixc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gtwnddjowj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hfpthk.cn/gtbzdaisah.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.gogol.net.cn/gtwydilkrf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.c1oappe.top/gtjbwujqhs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.sweek.top/gtoyymbeyh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ehwqpu.com/gtrlsuirlg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.pengpengdd.cyou/gtjqypwnnw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gotoacloud.top/gtzsworequ.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.tianlin.xyz/gtpzvpxqvf.html

================================================================================
来源：http://hz.sxryk.cn/gtisfaniku.html

A. 基础语法与类型
来源：http://hz.hammf.cn/gtjqemlxps.html

================================================================================
来源：http://hz.ivvv.top/gtmddsmdnk.html

[A01] Hello World
来源：http://hz.yueranfly.top/gthcjpdckz.html

Py:   print("Hello, World!")
来源：http://hz.jianghu66.top/gtnkatrtej.html

PHP:  echo "Hello, World!";
来源：http://hz.tian-w.cn/gtayzfxejz.html

JS:   console.log("Hello, World!");
来源：http://hz.redwolf501.top/gtozmeowbm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.tanke756.top/gtdzyftfhy.html

Java: System.out.println("Hello, World!");
来源：http://hz.9152youxi.cn/gtjlxgqczk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.snrcjt.cn/gtaadldvob.html

Ruby: puts "Hello, World!"
来源：http://hz.fengsongda.top/gtnslwltng.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.snrcjt.cn/gtwyymkoav.html

[A02] 变量声明与赋值
来源：http://hz.mhx1999.top/gtwaufqtlc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.nanxuanxn.top/gtpjwdmzgz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.havefunace.top/gtxxpjgxzt.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.tanke756.top/gtlrnygzhz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.redwolf501.top/gtyhybxipx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yj20258.top/gtkitnntaw.html

Go:   name := "Alex"; age := 20
来源：http://hz.xingfuxueyuan.xyz/gtyontvzfq.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hammf.cn/gtowiszlyu.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.pycfn.com/gtehcximqd.html

[A03] 常量定义
来源：http://hz.9152youxi.cn/gthzczathu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.0kj1m.cn/gtbhpteulc.html

PHP:  const PI = 3.14159;
来源：http://hz.xylfe.cn/gtzorlonsd.html

JS:   const PI = 3.14159;
来源：http://hz.sysykeji.top/gtsvrzjyzb.html

TS:   const PI: number = 3.14159;
来源：http://hz.feifeiyinyue.top/gtdjbpvinl.html

Java: static final double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtuuegqwnk.html

Go:   const PI = 3.14159
来源：http://hz.shzxlz.cn/gthprdoyfj.html

Ruby: PI = 3.14159
来源：http://hz.hnqzz.top/gtrfatthld.html

C#:   const double PI = 3.14159;
来源：http://hz.xziqi.cn/gtstbnbben.html

[A04] 判断变量类型
来源：http://hz.yuxming.cn/gtugimwaah.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ppjwa.cn/gtznbjtlkl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.chenlongwang.top/gtaqpffnth.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hnxiangtu.top/gtjlbrvodi.html

TS:   typeof x; x instanceof Date
来源：http://hz.ivvv.top/gtyillovdw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yvedp.cn/gtvikmzrzc.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jinyuanbaomall.cn/gtluidkkdo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zhaomingkeji.xyz/gtciymvpww.html

C#:   x.GetType().Name; x is int
来源：http://hz.vqdsnc.cn/gtcuabbsin.html

[A05] 整数除法与取模
来源：http://hz.meibo888.top/gtgjtaenvp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zycfv.cn/gtanylvxmv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.wangdashe.top/gtffnvwtgv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.feifeiyinyue.top/gtnphspwck.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gotoacloud.top/gtrajngxzr.html

Java: 7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtjwsghdrz.html

Go:   7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtkjdexerc.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.mhx1999.top/gtsorrjsir.html

C#:   7 / 2; 7 % 2
来源：http://hz.dianchejie.cn/gtwunsioly.html

[A06] 字符串转数字
来源：http://hz.0kj1m.cn/gtxjfbhwqe.html

Py:   int("42"); float("3.14")
来源：http://hz.chenjidiqi.icu/gtlunkigux.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.meibo888.top/gtqyzyhqak.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xziqi.cn/gtfesfegtj.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ydjk.org.cn/gtplzbosmp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.pengpengdd.cyou/gtmvgtuwer.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jinghuilouyu.cn/gtpgjzfmic.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.0kj1m.cn/gtwzpjlghl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hysaishi.cn/gtqlsesfkf.html

[A07] 数字转字符串
来源：http://hz.aibaodan.cn/gtdiwdogig.html

Py:   str(42)
来源：http://hz.9152youxi.cn/gtmzvnacpz.html

PHP:  (string) 42; strval(42)
来源：http://hz.hysaishi.cn/gtmrzwrwvt.html

JS:   String(42); (42).toString()
来源：http://hz.nanxinkj.top/gtskjwlfjp.html

TS:   String(42)
来源：http://hz.zdqjudy.top/gtmegtompw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.9152youxi.cn/gtowjwrpwf.html

Go:   strconv.Itoa(42)
来源：http://hz.guowangkeji.top/gtcyiaeoss.html

Ruby: 42.to_s
来源：http://hz.daxiang520.top/gthsmyqcdl.html

C#:   42.ToString()
来源：http://hz.ywan-chungtsiang.top/gtluvdujvs.html

[A08] 取整与四舍五入
来源：http://hz.daria6918.cn/gtbbmdrbrp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jinghuilouyu.cn/gtmpenugur.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.quarkkingdee.top/gtktaubdoc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hammf.cn/gtzqzogorx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zhaomingkeji.xyz/gtwegjedoc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.shzxlz.cn/gtlemicyyg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.cdnleiting.top/gtmibpipmp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.mhx1999.top/gtcvvrcxav.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.aizwys.cn/gtlkepxgdu.html

[A09] 绝对值与最大最小值
来源：http://hz.nwbrower.top/gtmnblvkla.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.dashuyun.cn/gtulowljbd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.sufxvd.cn/gtcuzagjgy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.ppjwa.cn/gtuuhiiumr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.gogol.net.cn/gtlgckyyya.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.0kj1m.cn/gtriferrnk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yuanzhike.top/gtquxgghik.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.fzhhl.top/gtceluwgtm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.havefunace.top/gtcsnhyxpo.html

[A10] 生成随机数
来源：http://hz.jqgfzy.top/gthrsxyhtq.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hywenlv.cn/gtqmimpfec.html

PHP:  random_int(1, 100);
来源：http://hz.ywan-chungtsiang.top/gtgabmnxic.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ybcxt.top/gtyhfkwtfj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.haohaochexian.top/gthrcevhjw.html

Java: new Random().nextInt(100) + 1
来源：http://hz.xylfe.cn/gtnnyiywdu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jyoumei.cn/gtcrvxitgy.html

Ruby: rand(1..100)
来源：http://hz.jiagoushi.top/gtusxqejba.html

C#:   new Random().Next(1, 101)
来源：http://hz.pengpengdd.cyou/gtecqloxph.html

[A11] 条件表达式（三元）
来源：http://hz.zhengqikj.top/gtytrrtpyo.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zhaomingkeji.xyz/gtoeyrjbca.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.fengsongda.top/gtsjhcbpgd.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jinqigufen.top/gtoltjxlzm.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.aizwys.cn/gtfzzmgxqj.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yanxiufei.cn/gtdfxpjeol.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.hfpthk.cn/gtrljvimej.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.redwolf501.top/gtseubtumj.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.xylfe.cn/gtpfwpojau.html

[A12] 字符串插值 / 格式化
来源：http://hz.havefunace.top/gtxvwxuoro.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.wangdashe.top/gtqveezuwi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.pycfn.com/gthetwknhu.html

JS:   `Hello, ${name}!`
来源：http://hz.quarkkingdee.top/gtringbqvi.html

TS:   `Hello, ${name}!`
来源：http://hz.hongshengwenyu.top/gtwiixqdra.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hysaishi.cn/gtuhmlgwvt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.kuanghao11.cn/gtcpquauln.html

Ruby: "Hello, #{name}!"
来源：http://hz.xuanzx.com/gtxzdeqjew.html

C#:   $"Hello, {name}!"
来源：http://hz.sysykeji.top/gtylkrumai.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.redwolf501.top/gtsieyjdly.html

Py:   "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtcvqmygtz.html

PHP:  "第一行\n第二行"
来源：http://hz.pycfn.com/gtpmsxkslo.html

JS:   "第一行\n第二行"
来源：http://hz.pengpengdd.cyou/gtdkqkcech.html

TS:   "第一行\n第二行"
来源：http://hz.yuxming.cn/gteuokayuu.html

Java: "第一行\n第二行"
来源：http://hz.zycfv.cn/gtmzjuorrf.html

Go:   "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtassuvpew.html

Ruby: "第一行\n第二行"
来源：http://hz.sxryk.cn/gtkxrkfbys.html

C#:   "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtkdexowbp.html

[A14] 注释写法
来源：http://hz.hywenlv.cn/gtvgzcgcyp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.gotoacloud.top/gtcqxezghs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.jqgufenzy.top/gtrgryipju.html

JS:   // 单行；/* 多行 */
来源：http://hz.yangfankeji.com/gtcaoplbvi.html

TS:   // 单行；/* 多行 */
来源：http://hz.ywan-chungtsiang.top/gtkrhqqkmc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.aibaodan.cn/gttintwgyo.html

Go:   // 单行；/* 多行 */
来源：http://hz.vqdsnc.cn/gtydtwgdfe.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.9152youxi.cn/gtagsffbrc.html


<!-- 参考信息 -->