代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://hz.yueranfly.top/gthxrywtks.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.nwbrower.top/gtuqwrzxbt.html

[U84] JS：CommonJS 写法
来源：http://hz.jianghu66.top/gtkakdpftn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinqigfzy.top/gtyqtifsub.html

[U85] JS：可选链
来源：http://hz.fengsongda.top/gttexvoohb.html

a?.b?.c
来源：http://hz.gogol.net.cn/gtpohfyngt.html

[U86] JS：空值合并
来源：http://hz.feifeiyinyue.top/gtvgvaqnle.html

a ?? b
来源：http://hz.hongshengwenyu.top/gttefwgwam.html

[U87] JS：解构默认值
来源：http://hz.yj20258888.top/gtsqhqigga.html

const { a = 1, b = 2 } = obj;
来源：http://hz.316326.xyz/gthoemmcwc.html

[U88] JS：对象展开合并
来源：http://hz.cucudq.cn/gtbjvapfdo.html

{ ...a, ...b }
来源：http://hz.fengsongda.top/gtexaoipiv.html

[U89] JS：数组去重
来源：http://hz.yonumen.top/gtpmquxdcr.html

[...new Set(arr)]
来源：http://hz.svipenyu.cn/gtvevxsxbu.html

[U90] JS：数字数组排序
来源：http://hz.jianghu66.top/gtvgkqipyn.html

[...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtobhellqf.html

[U91] JS：对象键值遍历
来源：http://hz.ybcxt.top/gtkjkjpbdw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.0kj1m.cn/gtocubnjsz.html

[U92] JS：深拷贝
来源：http://hz.ybcxt.top/gtkryxvxma.html

structuredClone(obj)
来源：http://hz.guannengcc.top/gtfifhbyre.html

[U93] JS：模板字符串
来源：http://hz.smart0.xyz/gtxjalimef.html

`共 ${n} 条`
来源：http://hz.fzhhl.top/gtypajirim.html

[U94] JS：箭头函数
来源：http://hz.shangyingyoupin.top/gtcwktzwwo.html

const double = x => x * 2;
来源：http://hz.sysykeji.top/gtlqgdockv.html

[U95] JS：Promise 包装
来源：http://hz.hammf.cn/gtcsxiduew.html

new Promise((resolve, reject) => {})
来源：http://hz.sweek.top/gtirvvgygm.html

[U96] JS：async/await 与异常
来源：http://hz.chenlongwang.top/gtgwrwvltw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tian-w.cn/gtnxnslvon.html

[U97] JS：并发请求
来源：http://hz.0kj1m.cn/gtbripmkcr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnqzz.top/gtemvivyrv.html

[U98] JS：fetch 带 JSON
来源：http://hz.yuxming.cn/gtadddrxsk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhaomingkeji.xyz/gtathotvrg.html

[U99] JS：事件监听
来源：http://hz.zycfv.cn/gtzajpuwaf.html

el.addEventListener("click", e => {})
来源：http://hz.mhx1999.top/gtwdbqzwud.html

[U100] JS：DOM 查询
来源：http://hz.cdnleiting.top/gtpwbcjupm.html

document.querySelector(".item")
来源：http://hz.hywenlv.cn/gtfzeypskf.html

[U101] JS：classList 操作
来源：http://hz.hfpthk.cn/gtbkaqfsxa.html

el.classList.toggle("active")
来源：http://hz.dashuyun.cn/gtytkawang.html

[U102] JS：本地存储
来源：http://hz.ywan-chungtsiang.top/gtnbzzztwv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.smart0.xyz/gteifctwym.html

[U103] JS：定时器
来源：http://hz.nanxuanxn.top/gtvtmkhjbk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hysaishi.cn/gtquyegfxh.html

[U104] JS：防抖
来源：http://hz.guannengcc.top/gtsxvgfxkv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gteqhmydba.html

[U105] JS：节流
来源：http://hz.nwbrower.top/gtrqskecih.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xylfe.cn/gtvncuamug.html

[U106] JS：日期格式化
来源：http://hz.sweek.top/gtamwsecsc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ehwqpu.com/gtenxidfdz.html

[U107] JS：数字千分位
来源：http://hz.iojbl.cn/gtuzdnigvu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.feifeiyinyue.top/gtrsdysdgd.html

[U108] JS：随机整数
来源：http://hz.guowangkeji.top/gtcxvcjznn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ydjk.org.cn/gtcjxfvfkt.html

[U109] JS：数组分组
来源：http://hz.andypj.xyz/gtuehvgfsk.html

Object.groupBy(arr, x => x.type)
来源：http://hz.nanxuanxn.top/gtillvppar.html

[U110] JS：数组分块
来源：http://hz.bjfxy.top/gtrevzbenu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ydjk.org.cn/gtpujkjmps.html

[U111] JS：对象转 Map
来源：http://hz.yueranfly.top/gtwhjcanzb.html

new Map(Object.entries(obj))
来源：http://hz.shanyushiyangkeji.top/gtwadijaln.html

[U112] JS：字符串补位
来源：http://hz.fzhhl.top/gtxolehipj.html

"7".padStart(3, "0")
来源：http://hz.pycfn.com/gtpofthzzv.html

[U113] JS：正则替换全部
来源：http://hz.hnxiangtu.top/gtxpqnxfaj.html

s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtuserjwzw.html

[U114] JS：JSON 深比较
来源：http://hz.yj202588.top/gtyyhdfqnf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gtzmzjyqvn.html

[U115] JS：生成 UUID
来源：http://hz.guannengcc.top/gtpcabtlvx.html

crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtknsfqxaq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hnxiangtu.top/gtpimffcrf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zdqjudy.top/gtclguikyb.html

[U117] JS：单元测试
来源：http://hz.gzhubu.top/gtwbepajgu.html

npm i -D vitest;  npx vitest
来源：http://hz.nanxinkj.top/gtixrtrhkt.html

[U118] JS：开发服务器
来源：http://hz.hongshengwenyu.top/gtvhfowdkf.html

npm i -D vite;  npx vite
来源：http://hz.xziqi.cn/gtoijjwsja.html

[U119] JS：生产构建
来源：http://hz.ywan-chungtsiang.top/gttdfhdoir.html

npx vite build
来源：http://hz.iojbl.cn/gtvjovypwn.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhoulong.xyz/gtfdayjzfg.html

import.meta.env.VITE_API_URL
来源：http://hz.jqgufenzy.top/gtthxzvvjs.html

================================================================================
来源：http://hz.cucudq.cn/gtjjpwwvlz.html

统计汇总
来源：http://hz.snrcjt.cn/gtmlfhbien.html

================================================================================
来源：http://hz.daxiang520.top/gtcczdzkac.html

按语言统计（条）：
来源：http://hz.gzhubu.top/gtkhzxseco.html

Python ......... 252
来源：http://hz.shanyushiyangtech.top/gtjvvjuyrj.html

PHP ............ 252
来源：http://hz.hywenlv.cn/gtueygpdik.html

JavaScript ..... 252
来源：http://hz.nanxinkj.top/gtztvtytlj.html

TypeScript ..... 212
来源：http://hz.chenjidiqi.icu/gtppniacif.html

Java ........... 212
来源：http://hz.feifeiyinyue.top/gtzsrkfuzd.html

Go ............. 212
来源：http://hz.xylfe.cn/gtedjleiif.html

Ruby ........... 212
来源：http://hz.jqgfzy.top/gtvpitncte.html

C# ............. 212
来源：http://hz.tanke756.top/gtepirposy.html

C .............. 30
来源：http://hz.zhongyouzk.top/gteycdxtew.html

C++ ............ 30
来源：http://hz.shzxlz.cn/gtjnjmadsq.html

SQL ............ 90
来源：http://hz.zhoulong.xyz/gtkfkwszfz.html

Bash ........... 80
来源：http://hz.xuetiantiany.cn/gtqeiabvcz.html

Kotlin ......... 15
来源：http://hz.sweek.top/gtiglbogla.html

Swift .......... 15
来源：http://hz.fengsongda.top/gtnpcrpobu.html

Lua ............ 10
来源：http://hz.ydjk.org.cn/gtirjahjbi.html

Perl ........... 10
来源：http://hz.hongshengwenyu.top/gtmsgcimxc.html

Scala .......... 10
来源：http://hz.tanke756.top/gtrcjgavzl.html

------------------------------------
来源：http://hz.jqgfzy.top/gthodaunyu.html

合计 ........... 2106 条
来源：http://hz.vqdsnc.cn/gtubwamsqf.html

按章节统计：
来源：http://hz.nwbrower.top/gtykgyzrkx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj202588.top/gtsxtfdmsk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtsuxdkxmw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtfsamsuen.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sysykeji.top/gthgvvqnks.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shangyingyoupin.top/gtuwosbgrr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtziotmzsq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xylfe.cn/gtzhmkofeh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj20258888.top/gthcmqqgat.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtejckslag.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yvedp.cn/gtetbwkcpl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtjggqusma.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtcuezltvs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtuawdflkw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ybcxt.top/gtrgwoaecj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhengqikj.top/gtmubjqfqm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtowxzvuiw.html

Q SQL 专题                              90
来源：http://hz.xuetiantiany.cn/gtupvqxqul.html

R Bash 专题                             80
来源：http://hz.dianchejie.cn/gtimsalypa.html

S C / C++ 专题                          60
来源：http://hz.cdnleiting.top/gtfipxwhah.html

T 其他语言补充                          60
来源：http://hz.pengpengdd.cyou/gtcadqiuoq.html

U 高频实用片段                         120
来源：http://hz.sweek.top/gtsoaxocpi.html

------------------------------------
来源：http://hz.0kj1m.cn/gtupotdich.html

合计                                  2106 条
来源：http://hz.xuetiantiany.cn/gtqsjbgepo.html

--------------------------------------------------------------------------------
来源：http://hz.sxryk.cn/gtbaqgexfb.html

使用提醒
来源：http://hz.zycfv.cn/gtsyllszha.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtadprrwmm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jiagoushi.top/gtruojgsqo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hnxiangtu.top/gtavrdhelm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hnxiangtu.top/gtscaumlzi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cucudq.cn/gtgqgaqsjo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cheryme.top/gtutlhbkvz.html

—— 文件结束 ——
来源：http://hz.yuxming.cn/gtkookjxig.html

================================================================================
来源：http://hz.cdnleiting.top/gttcpubjdr.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.birdmap.top/gteehbzlym.html

Common Programming Examples Cheat Book
来源：http://hz.zhengqikj.top/gtskjjlcal.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtcglyuahf.html

【收录内容】
来源：http://hz.zhongyouzk.top/gtkfeijpnv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shanyushiyangkeji.top/gtnqgdqqyh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.c1oappe.top/gtlqytbqsl.html

SQL · Bash · C · C++
来源：http://hz.c1oappe.top/gtjvzbkxit.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yangfankeji.com/gtdrllsmnh.html

【使用说明】
来源：http://hz.havefunace.top/gtcsirzhyf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.guannengcc.top/gtegangkyf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.aibaodan.cn/gtgoesfcpa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sufxvd.cn/gtfkltlxxi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.meibo888.top/gtbtzswawg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yonumen.top/gtyvuplleh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shanyushiyangkeji.top/gtnrkxjnyt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jqgfzy.top/gtxyinznyt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yuxming.cn/gtpckkbkoq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cheryme.top/gtusnxrirz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jianghu66.top/gtcuwpchtf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhengqikj.top/gtcubazqoh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yuxming.cn/gtxycudfxw.html

【文件统计】
来源：http://hz.chenlongwang.top/gtokujcotr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shzxlz.cn/gtktfezaei.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gtvtxndgfb.html

目  录
来源：http://hz.fengsongda.top/gtwdohigdl.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtglydpalw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zycfv.cn/gtxhrmnxjb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.316326.xyz/gtuueezkry.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.316326.xyz/gtjzztcoey.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.316326.xyz/gtvdlmgkqa.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ywan-chungtsiang.top/gtoytrxjou.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yj202588.top/gtypmmlwxz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtzgxjykge.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sweek.top/gtmhctjqke.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.pycfn.com/gtchcxlvpf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hysaishi.cn/gtkfkkjury.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.gotoacloud.top/gtjtxipbwy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gttgayuxfc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtjigxycxf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xuanzx.com/gteuakufuh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cucudq.cn/gthdmjucop.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gtisvlssok.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.dianchejie.cn/gtgfqancrr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ivvv.top/gtcqohbpth.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hfpthk.cn/gtrdzzhszo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuetiantiany.cn/gtzossgfgg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yongpay.top/gtssirsemh.html

================================================================================
来源：http://hz.cdnleiting.top/gtnznkqebp.html

A. 基础语法与类型
来源：http://hz.ppjwa.cn/gtqbkrnbem.html

================================================================================
来源：http://hz.gogol.net.cn/gtwtpqdskr.html

[A01] Hello World
来源：http://hz.0kj1m.cn/gtdfurgusl.html

Py:   print("Hello, World!")
来源：http://hz.ybcxt.top/gtjtixixbg.html

PHP:  echo "Hello, World!";
来源：http://hz.daria6918.cn/gtkmdpdwzf.html

JS:   console.log("Hello, World!");
来源：http://hz.xingfuxueyuan.xyz/gtqbtpscjh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hysaishi.cn/gtfhvrxgtp.html

Java: System.out.println("Hello, World!");
来源：http://hz.feifeiyinyue.top/gtggnnfcrr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shanyushiyangtech.top/gtmkjpwauw.html

Ruby: puts "Hello, World!"
来源：http://hz.hfpthk.cn/gtrysdvzuu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yj20258888.top/gtrdcrlxmj.html

[A02] 变量声明与赋值
来源：http://hz.cqqwz.cn/gtksaqyehz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hammf.cn/gthcbhfnpl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.gzhubu.top/gtetwbaube.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yj202588.top/gtviaomesn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ydzc1.top/gtxoniybjj.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.vqdsnc.cn/gtdrjpgxbp.html

Go:   name := "Alex"; age := 20
来源：http://hz.svipenyu.cn/gtlzyvmaqu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yueranfly.top/gtglsnoysr.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yvedp.cn/gtfefubnhd.html

[A03] 常量定义
来源：http://hz.gzhubu.top/gtyozvybeo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ybcxt.top/gtxipxekne.html

PHP:  const PI = 3.14159;
来源：http://hz.cheryme.top/gtajjmobcw.html

JS:   const PI = 3.14159;
来源：http://hz.zhoulong.xyz/gthybarfxn.html

TS:   const PI: number = 3.14159;
来源：http://hz.yuxming.cn/gtkcioknrl.html

Java: static final double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtbforbees.html

Go:   const PI = 3.14159
来源：http://hz.guannengcc.top/gtmujeuboy.html

Ruby: PI = 3.14159
来源：http://hz.xinyue.icu/gtkojyztbw.html

C#:   const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtlreohxjm.html

[A04] 判断变量类型
来源：http://hz.mhx1999.top/gtsomjmmje.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhaomingkeji.xyz/gtfushhwxg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shanyushiyangkeji.top/gtccwxpqep.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jinqigfzy.top/gteedxtkue.html

TS:   typeof x; x instanceof Date
来源：http://hz.hnxiangtu.top/gthyajbttj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.aizwys.cn/gtrccnkfdo.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yj202588.top/gtgusldddq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sxryk.cn/gtuezpxgwi.html

C#:   x.GetType().Name; x is int
来源：http://hz.xinyue.icu/gtvapmhedz.html

[A05] 整数除法与取模
来源：http://hz.ywan-chungtsiang.top/gtgrflhpcm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ehwqpu.com/gteyzrcjne.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.svipenyu.cn/gtmhrzgnwx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.smart0.xyz/gtwbtgkyni.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hnqzz.top/gtrstostzv.html

Java: 7 / 2; 7 % 2
来源：http://hz.zhiwuduotai.top/gtfwlbdeax.html

Go:   7 / 2; 7 % 2
来源：http://hz.xuanzx.com/gtkcpqzwhc.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ivvv.top/gtqtxklpsd.html

C#:   7 / 2; 7 % 2
来源：http://hz.zhongyouzk.top/gtkiiphgeg.html

[A06] 字符串转数字
来源：http://hz.aizwys.cn/gtjkbkpmhe.html

Py:   int("42"); float("3.14")
来源：http://hz.vqdsnc.cn/gtyjhtkokn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.daria6918.cn/gtzsckkczp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.wangdashe.top/gtjgzbbaic.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.nwbrower.top/gtmylispmp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jinyuanbaomall.cn/gtcdjzmtcy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.cdnleiting.top/gtmucrduve.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.9152youxi.cn/gtszrmfyji.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.0kj1m.cn/gtmlrhzxku.html

[A07] 数字转字符串
来源：http://hz.zhixingplan.top/gtwymwzyzn.html

Py:   str(42)
来源：http://hz.xziqi.cn/gtmvkgbfkn.html

PHP:  (string) 42; strval(42)
来源：http://hz.tanke756.top/gtsjhqzave.html

JS:   String(42); (42).toString()
来源：http://hz.316326.xyz/gtchgyinxt.html

TS:   String(42)
来源：http://hz.yuanzhike.top/gtqeegtcat.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xingfuxueyuan.xyz/gtyorbpdcf.html

Go:   strconv.Itoa(42)
来源：http://hz.smart0.xyz/gtkjfodsfp.html

Ruby: 42.to_s
来源：http://hz.shuidangran.top/gtdimxejmr.html

C#:   42.ToString()
来源：http://hz.hongshengwenyu.top/gttwdoqglu.html

[A08] 取整与四舍五入
来源：http://hz.52xcode.cn/gtagjrkjes.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.feifeiyinyue.top/gtmgfrdhqc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jinyuanbaomall.cn/gttrsxioiy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ydjk.org.cn/gtxondmzbt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.xuetiantiany.cn/gtdvpembfk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.aibaodan.cn/gtppqycdnt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.vqdsnc.cn/gtmalqucge.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.vqdsnc.cn/gtcndlqrfc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.0kj1m.cn/gtwuvzcsjd.html

[A09] 绝对值与最大最小值
来源：http://hz.tanke756.top/gtnlljstzt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.guannengcc.top/gtactxdncy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jlsjyb.cn/gtgraggjws.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zycfv.cn/gtvgagibtm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gtiippjlxr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.yvedp.cn/gtrudijqyn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.shanyushiyangkeji.top/gthfwbbqnu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.shanyushiyangkeji.top/gtighfmtrd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.vqdsnc.cn/gttosixidu.html

[A10] 生成随机数
来源：http://hz.xuetiantiany.cn/gtsxvutgpv.html

Py:   import random; random.randint(1, 100)
来源：http://hz.sxryk.cn/gtbdzjvjje.html

PHP:  random_int(1, 100);
来源：http://hz.cheryme.top/gtwvfpbswd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhaomingkeji.xyz/gtpwnjamzz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zycfv.cn/gtkcbbqvtp.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yj20258888.top/gtkegcbimy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.fzhhl.top/gtdwnhmffv.html

Ruby: rand(1..100)
来源：http://hz.fzhhl.top/gtumyriryr.html

C#:   new Random().Next(1, 101)
来源：http://hz.mhx1999.top/gtqmtzrhzi.html

[A11] 条件表达式（三元）
来源：http://hz.daria6918.cn/gtngfegild.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.aizwys.cn/gtkbjdvkht.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.guannengcc.top/gtemdyxzzr.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.gotoacloud.top/gtfkiksclj.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.c1oappe.top/gtnjhxrlma.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ydzc1.top/gtevzziqrl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jinqigufen.top/gtmzptjrvm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.yueranfly.top/gtnyttmjry.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gttsfmuebw.html

[A12] 字符串插值 / 格式化
来源：http://hz.sweek.top/gtbtgrxwsx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hywenlv.cn/gtisqpllwm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.316326.xyz/gtpasbyryq.html

JS:   `Hello, ${name}!`
来源：http://hz.cashguo.top/gtfyyfkpsa.html

TS:   `Hello, ${name}!`
来源：http://hz.ydjk.org.cn/gtpwipbsrx.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.sysykeji.top/gtzrjfkykw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.aizwys.cn/gtmjihkfll.html

Ruby: "Hello, #{name}!"
来源：http://hz.quarkkingdee.top/gtlcqpyoma.html

C#:   $"Hello, {name}!"
来源：http://hz.zhijiandao.cn/gtgshbrsrv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.cdnleiting.top/gttfigqxcu.html

Py:   "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtsgatipxa.html

PHP:  "第一行\n第二行"
来源：http://hz.fzhhl.top/gtbbafcoaa.html

JS:   "第一行\n第二行"
来源：http://hz.chenlongwang.top/gtqunbkwli.html

TS:   "第一行\n第二行"
来源：http://hz.ivvv.top/gtvalyqngd.html

Java: "第一行\n第二行"
来源：http://hz.hywenlv.cn/gtoonnhljs.html

Go:   "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtijnuxdcn.html

Ruby: "第一行\n第二行"
来源：http://hz.0kj1m.cn/gtyfytkgix.html

C#:   "第一行\n第二行"
来源：http://hz.xinyue.icu/gtukvigjih.html


<!-- 参考信息 -->