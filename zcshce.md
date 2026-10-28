代发 wailian999

[U85] JS：可选链
来源：http://hz.shanyushiyangtech.top/gttrjkkssi.html

a?.b?.c
来源：http://hz.redwolf501.top/gtebeivgtl.html

[U86] JS：空值合并
来源：http://hz.tianlin.xyz/gtzfglodbr.html

a ?? b
来源：http://hz.xylfe.cn/gtyzyeqkgu.html

[U87] JS：解构默认值
来源：http://hz.cqqwz.cn/gtlzrquvmp.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zycfv.cn/gtqabyudht.html

[U88] JS：对象展开合并
来源：http://hz.shanyushiyangkeji.top/gtstyczqlx.html

{ ...a, ...b }
来源：http://hz.jinghuilouyu.cn/gtfrjbbhke.html

[U89] JS：数组去重
来源：http://hz.yuanzhike.top/gtkhwviopf.html

[...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtirypdrdy.html

[U90] JS：数字数组排序
来源：http://hz.fzhhl.top/gtbjsqxstw.html

[...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtczuavymh.html

[U91] JS：对象键值遍历
来源：http://hz.jlsjyb.cn/gtrhpglfzw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.meibo888.top/gthbrmlbyq.html

[U92] JS：深拷贝
来源：http://hz.0kj1m.cn/gtyuomvzsw.html

structuredClone(obj)
来源：http://hz.hnqzz.top/gtfbhaqfpp.html

[U93] JS：模板字符串
来源：http://hz.jianghu66.top/gtpqgbmsmm.html

`共 ${n} 条`
来源：http://hz.dianchejie.cn/gtdluzytag.html

[U94] JS：箭头函数
来源：http://hz.kuanghao11.cn/gtyryvucrv.html

const double = x => x * 2;
来源：http://hz.316326.xyz/gtqiudugvb.html

[U95] JS：Promise 包装
来源：http://hz.hysaishi.cn/gtzfjymmzg.html

new Promise((resolve, reject) => {})
来源：http://hz.zhiwuduotai.top/gtxxjjxtyr.html

[U96] JS：async/await 与异常
来源：http://hz.andypj.xyz/gthswcoejq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtcyupmfvf.html

[U97] JS：并发请求
来源：http://hz.tianlin.xyz/gtnsuvrdte.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtnjqzkzvz.html

[U98] JS：fetch 带 JSON
来源：http://hz.c1oappe.top/gtwlgvkotb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yongpay.top/gtnrihowtm.html

[U99] JS：事件监听
来源：http://hz.yueranfly.top/gtedyaarzy.html

el.addEventListener("click", e => {})
来源：http://hz.jiagoushi.top/gthfwuqkvu.html

[U100] JS：DOM 查询
来源：http://hz.yj20258888.top/gtdonfmtxu.html

document.querySelector(".item")
来源：http://hz.fzhhl.top/gtdwbixiru.html

[U101] JS：classList 操作
来源：http://hz.52xcode.cn/gtdblsxqsc.html

el.classList.toggle("active")
来源：http://hz.ydjk.org.cn/gtkqbtihgx.html

[U102] JS：本地存储
来源：http://hz.dashuyun.cn/gtjucwpsgt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.smart0.xyz/gtikcootzt.html

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtvotvqzse.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.guannengcc.top/gtwlasldaj.html

[U104] JS：防抖
来源：http://hz.yangfankeji.com/gtuxhsvtga.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtfeorbfkc.html

[U105] JS：节流
来源：http://hz.chenlongwang.top/gtyshydesr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xylfe.cn/gtifxdoulf.html

[U106] JS：日期格式化
来源：http://hz.sxryk.cn/gtesvnloom.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.aibaodan.cn/gtzrcddimd.html

[U107] JS：数字千分位
来源：http://hz.mhx1999.top/gtzuojngfl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hnxiangtu.top/gtargnjrvu.html

[U108] JS：随机整数
来源：http://hz.shanyushiyangkeji.top/gtvhvmgobb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shuidangran.top/gtqnavkrtp.html

[U109] JS：数组分组
来源：http://hz.nwbrower.top/gtromqarmf.html

Object.groupBy(arr, x => x.type)
来源：http://hz.pengpengdd.cyou/gtnoyvzvii.html

[U110] JS：数组分块
来源：http://hz.shanyushiyangtech.top/gtpqknaljl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tianlin.xyz/gtndhvmpvk.html

[U111] JS：对象转 Map
来源：http://hz.xuetiantiany.cn/gtidcvgyvx.html

new Map(Object.entries(obj))
来源：http://hz.ydjk.org.cn/gtycnlhakg.html

[U112] JS：字符串补位
来源：http://hz.dianchejie.cn/gtpsrioqth.html

"7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtcactpcvk.html

[U113] JS：正则替换全部
来源：http://hz.cdnleiting.top/gtcrvqgjsm.html

s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtswzvblri.html

[U114] JS：JSON 深比较
来源：http://hz.ydjk.org.cn/gtntxqmpos.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gtrnlsjzko.html

[U115] JS：生成 UUID
来源：http://hz.ydjk.org.cn/gtkjixmxvg.html

crypto.randomUUID()
来源：http://hz.dianchejie.cn/gtpjtqufxg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhaomingkeji.xyz/gtyjsepmvq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.chenzaomai.com/gtjmycxpfl.html

[U117] JS：单元测试
来源：http://hz.yj20258.top/gtkkdfpabl.html

npm i -D vitest;  npx vitest
来源：http://hz.jinqigfzy.top/gtgsxyeije.html

[U118] JS：开发服务器
来源：http://hz.sxryk.cn/gtaferrcsx.html

npm i -D vite;  npx vite
来源：http://hz.9152youxi.cn/gtlwcgcqsj.html

[U119] JS：生产构建
来源：http://hz.ywan-chungtsiang.top/gtpklfdbkq.html

npx vite build
来源：http://hz.nanxinkj.top/gtkqodackp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ehwqpu.com/gtfuohpdbk.html

import.meta.env.VITE_API_URL
来源：http://hz.9152youxi.cn/gthonbgmwo.html

================================================================================
来源：http://hz.9152youxi.cn/gtacxjgzpw.html

统计汇总
来源：http://hz.quarkkingdee.top/gtmvoxkfkl.html

================================================================================
来源：http://hz.daxiang520.top/gtindnadxl.html

按语言统计（条）：
来源：http://hz.gzhubu.top/gtcqtmrzqp.html

Python ......... 252
来源：http://hz.yonumen.top/gteenhtsux.html

PHP ............ 252
来源：http://hz.jlsjyb.cn/gtrsxkgxpz.html

JavaScript ..... 252
来源：http://hz.ydzc1.top/gtqnwtkrfm.html

TypeScript ..... 212
来源：http://hz.xylfe.cn/gtpkuiunlw.html

Java ........... 212
来源：http://hz.dashuyun.cn/gtiphfpyhv.html

Go ............. 212
来源：http://hz.gotoacloud.top/gtnvqmpkdt.html

Ruby ........... 212
来源：http://hz.hywenlv.cn/gtchmyilee.html

C# ............. 212
来源：http://hz.hywenlv.cn/gtfjqnbvcu.html

C .............. 30
来源：http://hz.jlsjyb.cn/gtwitpccgq.html

C++ ............ 30
来源：http://hz.zycfv.cn/gtvunphdns.html

SQL ............ 90
来源：http://hz.gogol.net.cn/gtyimheyrr.html

Bash ........... 80
来源：http://hz.zhiwuduotai.top/gtgqflortt.html

Kotlin ......... 15
来源：http://hz.chenlongwang.top/gtueavwlay.html

Swift .......... 15
来源：http://hz.xingfuxueyuan.xyz/gtyhacujgz.html

Lua ............ 10
来源：http://hz.hnqzz.top/gtjbsevdvy.html

Perl ........... 10
来源：http://hz.hfpthk.cn/gtyfrwejzs.html

Scala .......... 10
来源：http://hz.ehwqpu.com/gtcwezwuha.html

------------------------------------
来源：http://hz.hongshengwenyu.top/gtbjmwznfv.html

合计 ........... 2106 条
来源：http://hz.chenjidiqi.icu/gtxkquceca.html

按章节统计：
来源：http://hz.chenjidiqi.icu/gthfqisakk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhaomingkeji.xyz/gttostulky.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sufxvd.cn/gtegfymiri.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenjidiqi.icu/gtlmtulimc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sxryk.cn/gtxmwpwcmh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.guowangkeji.top/gtznhfkwci.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.pengpengdd.cyou/gtghpgsipa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gthteqolnw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xylfe.cn/gtooxmzryr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtbmybyvsu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yongpay.top/gtvkiglpgb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtoyravqvo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtsmkeyqgd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtwpkhmesf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zdqjudy.top/gtkgycxkta.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.wangshuangyany.cn/gtuzwbqbnv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtpqqxhjcu.html

Q SQL 专题                              90
来源：http://hz.316326.xyz/gtrtmumqex.html

R Bash 专题                             80
来源：http://hz.nanxinkj.top/gtvhabvsux.html

S C / C++ 专题                          60
来源：http://hz.jinqigfzy.top/gtrecxfwdq.html

T 其他语言补充                          60
来源：http://hz.ydzc1.top/gtcwlzsnvr.html

U 高频实用片段                         120
来源：http://hz.ydzc1.top/gtuqiyrnjv.html

------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtcchwsqci.html

合计                                  2106 条
来源：http://hz.nanxinkj.top/gtnhxzldkd.html

--------------------------------------------------------------------------------
来源：http://hz.sweek.top/gtlzvherso.html

使用提醒
来源：http://hz.kuanghao11.cn/gtwxcztzrq.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtzpcvpruz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yuanzhike.top/gtygqidaqd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shanyushiyangtech.top/gtpbbqtbnu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.svipenyu.cn/gtnthgeerw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yj20258888.top/gtvulsxahw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shangyingyoupin.top/gtwtrgeevf.html

—— 文件结束 ——
来源：http://hz.jinqigufen.top/gtdsqhmrcn.html

================================================================================
来源：http://hz.ehwqpu.com/gtgvvpshrj.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ydjk.org.cn/gturguxdip.html

Common Programming Examples Cheat Book
来源：http://hz.andypj.xyz/gtuwhfogsy.html

================================================================================
来源：http://hz.chenlongwang.top/gtxsaoivpz.html

【收录内容】
来源：http://hz.gzhubu.top/gtsffztnpc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shuidangran.top/gtrnydvnzr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.quarkkingdee.top/gtpnfswuxj.html

SQL · Bash · C · C++
来源：http://hz.chenzaomai.com/gtwwsdchmd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.gogol.net.cn/gthqcqcynm.html

【使用说明】
来源：http://hz.shanyushiyangkeji.top/gtyxbaewyy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.svipenyu.cn/gtkhvuehva.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cqqwz.cn/gtbinvoarj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shangyingyoupin.top/gtxgexrmps.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xinyue.icu/gtlvabbhjf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zdqjudy.top/gtmynjolhd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.daria6918.cn/gtquiaimnu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ivvv.top/gtpgklqekf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.aizwys.cn/gtsaoudcyu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yj202588.top/gttenfvxvd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ybcxt.top/gtwlpacijp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhaomingkeji.xyz/gtkayrvznq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cqqwz.cn/gtdvaizqpc.html

【文件统计】
来源：http://hz.daxiang520.top/gtceuckvxz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shangyingyoupin.top/gtgzmzylam.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtiszfggso.html

目  录
来源：http://hz.jianghu66.top/gtwjkhkrhk.html

--------------------------------------------------------------------------------
来源：http://hz.sxryk.cn/gtofsvwqgs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xziqi.cn/gtxlgmbwtp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtjdydrtgy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.aizwys.cn/gtmrueqlvk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.pycfn.com/gtanfznuyp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhoulong.xyz/gtwhksrfyk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.tian-w.cn/gtbargeboi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hammf.cn/gtukdpqsmy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.pycfn.com/gtgnwjzfwp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.dianchejie.cn/gtolsdzjnm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yj202588.top/gtdovwmgnf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.redwolf501.top/gtxfamwago.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtwyppzhlu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtsxctoxmt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhengqikj.top/gthrawzsqs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.tianlin.xyz/gtkxuxdjni.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtswhbylka.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.birdmap.top/gtinfbkszf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yanxiufei.cn/gtmrtmtamq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yanxiufei.cn/gtatsvfotl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tian-w.cn/gthwjywwzk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuanzx.com/gtwxjmybnc.html

================================================================================
来源：http://hz.haohaochexian.top/gtshuijydc.html

A. 基础语法与类型
来源：http://hz.yuanzhike.top/gtvkxfeamj.html

================================================================================
来源：http://hz.yvedp.cn/gtsllslxrt.html

[A01] Hello World
来源：http://hz.guowangkeji.top/gtodfdebzo.html

Py:   print("Hello, World!")
来源：http://hz.gotoacloud.top/gtrwegqoxj.html

PHP:  echo "Hello, World!";
来源：http://hz.sysykeji.top/gtafyexozr.html

JS:   console.log("Hello, World!");
来源：http://hz.fengsongda.top/gtfjpldqrz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gzhubu.top/gtrjiqvqtc.html

Java: System.out.println("Hello, World!");
来源：http://hz.nwbrower.top/gtlrppyfhs.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinqigufen.top/gtodeesvjo.html

Ruby: puts "Hello, World!"
来源：http://hz.quarkkingdee.top/gtwdtorsqe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ybcxt.top/gtdwkgxfuh.html

[A02] 变量声明与赋值
来源：http://hz.jlsjyb.cn/gtdegiuazt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shanyushiyangkeji.top/gtvdmzfhzj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhixingplan.top/gtnevcbbxp.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.iojbl.cn/gtpatcpkch.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.mhx1999.top/gtgvymhrgg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.0kj1m.cn/gtyzjybmwn.html

Go:   name := "Alex"; age := 20
来源：http://hz.hfpthk.cn/gtejcwrrxw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.fengsongda.top/gtzmdhxppm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.andypj.xyz/gtyqhbjyol.html

[A03] 常量定义
来源：http://hz.kuanghao11.cn/gtzwpabwqv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.cdnleiting.top/gtsepvylxq.html

PHP:  const PI = 3.14159;
来源：http://hz.jiagoushi.top/gtxxmahrjo.html

JS:   const PI = 3.14159;
来源：http://hz.dashuyun.cn/gtcrvrtbny.html

TS:   const PI: number = 3.14159;
来源：http://hz.ivvv.top/gtnyfltvuy.html

Java: static final double PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtbacczunl.html

Go:   const PI = 3.14159
来源：http://hz.iojbl.cn/gtzblwdvge.html

Ruby: PI = 3.14159
来源：http://hz.quarkkingdee.top/gtxswevnjy.html

C#:   const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gttqxdzjpu.html

[A04] 判断变量类型
来源：http://hz.gzhubu.top/gtobgtgqmv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhengqikj.top/gtovxjltjq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shuidangran.top/gtmuswdycq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.sufxvd.cn/gtkrrfmnsz.html

TS:   typeof x; x instanceof Date
来源：http://hz.hfpthk.cn/gtddfqfhtj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.snrcjt.cn/gtqemageny.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yangfankeji.com/gtzpwkhord.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.aibaodan.cn/gtahixppfr.html

C#:   x.GetType().Name; x is int
来源：http://hz.hammf.cn/gtnrtqxykv.html

[A05] 整数除法与取模
来源：http://hz.vqdsnc.cn/gtpxxpxuiw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.vqdsnc.cn/gtzyvwbrtn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.svipenyu.cn/gtbcfegpyv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xziqi.cn/gtgyjizepd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.fzhhl.top/gtlkjrgstm.html

Java: 7 / 2; 7 % 2
来源：http://hz.gogol.net.cn/gtjvhcxape.html

Go:   7 / 2; 7 % 2
来源：http://hz.snrcjt.cn/gtgxojfqbe.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtfmovtwns.html

C#:   7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gtszozrefj.html

[A06] 字符串转数字
来源：http://hz.shuidangran.top/gtfklgqgxy.html

Py:   int("42"); float("3.14")
来源：http://hz.redwolf501.top/gttvedicsb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.chenzaomai.com/gtobfkevkd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.nanxuanxn.top/gtvhxoopoq.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.pycfn.com/gtpdjurycn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jiagoushi.top/gtpyvffemu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ivvv.top/gtwrvlrmky.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ehwqpu.com/gtdxiebfto.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.cqqwz.cn/gtvsxwuojv.html

[A07] 数字转字符串
来源：http://hz.andypj.xyz/gtnzseakwf.html

Py:   str(42)
来源：http://hz.dianchejie.cn/gtmeusxaky.html

PHP:  (string) 42; strval(42)
来源：http://hz.hysaishi.cn/gtinsymquf.html

JS:   String(42); (42).toString()
来源：http://hz.jianghu66.top/gtspdoisow.html

TS:   String(42)
来源：http://hz.daxiang520.top/gtuuhrsijd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yonumen.top/gtpdvmkovc.html

Go:   strconv.Itoa(42)
来源：http://hz.yueranfly.top/gtktxojmlu.html

Ruby: 42.to_s
来源：http://hz.gotoacloud.top/gtlwbueeoh.html

C#:   42.ToString()
来源：http://hz.jyoumei.cn/gtsyvxtpat.html

[A08] 取整与四舍五入
来源：http://hz.zhiwuduotai.top/gtdyhhycvh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.nanxuanxn.top/gtjktqmxmu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhengqikj.top/gtjsiysdxx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.chenzaomai.com/gtjxbvxnwo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ppjwa.cn/gtbsliinco.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jqgufenzy.top/gtakorlwvd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jqgufenzy.top/gtlkbabeok.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.havefunace.top/gtdwhitmhp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yuanzhike.top/gtrgccahdu.html

[A09] 绝对值与最大最小值
来源：http://hz.yvedp.cn/gtbatafgyo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.9152youxi.cn/gtyrktndzb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.nanxinkj.top/gtpcxfnjfj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zycfv.cn/gtkkvrgyph.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.aizwys.cn/gtldctedfy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.yj20258888.top/gtufmsbqkc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.vqdsnc.cn/gtayhfrcll.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.yueranfly.top/gtavszsocn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.jinghuilouyu.cn/gtwcnuvivb.html

[A10] 生成随机数
来源：http://hz.tianlin.xyz/gtepbjecjn.html

Py:   import random; random.randint(1, 100)
来源：http://hz.haohaochexian.top/gtovpjdkwr.html

PHP:  random_int(1, 100);
来源：http://hz.guowangkeji.top/gtnjdlwaxe.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.redwolf501.top/gtglmsnxbq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.redwolf501.top/gtlqabngwc.html

Java: new Random().nextInt(100) + 1
来源：http://hz.fzhhl.top/gtvtlaxglp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.fengsongda.top/gtphpbddlp.html

Ruby: rand(1..100)
来源：http://hz.shzxlz.cn/gtzxgkojnd.html

C#:   new Random().Next(1, 101)
来源：http://hz.jinqigfzy.top/gtwhmmepli.html

[A11] 条件表达式（三元）
来源：http://hz.jqgfzy.top/gttbnqdzxu.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.cucudq.cn/gtlkkprnqd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.ivvv.top/gtdkoctwip.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.xuetiantiany.cn/gtbzjqmltp.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.chenlongwang.top/gtjipheaxu.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ppjwa.cn/gtiylpzblb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jiagoushi.top/gtofbjrhzf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.tanke756.top/gtewmihaju.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.sysykeji.top/gtspcbfame.html

[A12] 字符串插值 / 格式化
来源：http://hz.smart0.xyz/gtjajyqjgi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.guannengcc.top/gtjhghyqbo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.tian-w.cn/gtqknomndc.html

JS:   `Hello, ${name}!`
来源：http://hz.snrcjt.cn/gthkuwipjr.html

TS:   `Hello, ${name}!`
来源：http://hz.sufxvd.cn/gtznvlcmie.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zycfv.cn/gtnsuxrkoq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.feifeiyinyue.top/gtzsqwopgx.html

Ruby: "Hello, #{name}!"
来源：http://hz.zycfv.cn/gttkhasolb.html

C#:   $"Hello, {name}!"
来源：http://hz.xziqi.cn/gthmkmuhei.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.wangshuangyany.cn/gtpiomdmmv.html

Py:   "第一行\n第二行"
来源：http://hz.jiagoushi.top/gtrkpwwcbl.html

PHP:  "第一行\n第二行"
来源：http://hz.zhoulong.xyz/gtujjhzckv.html

JS:   "第一行\n第二行"
来源：http://hz.ybcxt.top/gtlntyaagm.html

TS:   "第一行\n第二行"
来源：http://hz.cashguo.top/gtrslgjfop.html

Java: "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtjpfwervq.html

Go:   "第一行\n第二行"
来源：http://hz.gaohongyu789.top/gtyxbogutb.html

Ruby: "第一行\n第二行"
来源：http://hz.zdqjudy.top/gtokkzjucq.html

C#:   "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gtkidjbnyw.html

[A14] 注释写法
来源：http://hz.dashuyun.cn/gtxcrgdfil.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.pycfn.com/gtffwoosfo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.cucudq.cn/gtjfacjmrt.html

JS:   // 单行；/* 多行 */
来源：http://hz.cdnleiting.top/gtbuoiqwht.html


<!-- 参考信息 -->