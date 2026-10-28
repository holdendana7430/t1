代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://hz.yanxiufei.cn/gtpidukepj.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jinyuanbaomall.cn/gtvzepudwb.html

[U84] JS：CommonJS 写法
来源：http://hz.zhiwuduotai.top/gtpycamhbo.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.snrcjt.cn/gtefpozqpx.html

[U85] JS：可选链
来源：http://hz.0kj1m.cn/gtdcfstiag.html

a?.b?.c
来源：http://hz.yangfankeji.com/gtcxzgajya.html

[U86] JS：空值合并
来源：http://hz.52xcode.cn/gtfciphukz.html

a ?? b
来源：http://hz.ydjk.org.cn/gtujnjxakm.html

[U87] JS：解构默认值
来源：http://hz.yuanzhike.top/gttgpeuaeg.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yj202588.top/gtzzexbwve.html

[U88] JS：对象展开合并
来源：http://hz.xuanzx.com/gtjighggcs.html

{ ...a, ...b }
来源：http://hz.quarkkingdee.top/gtrmspakid.html

[U89] JS：数组去重
来源：http://hz.mhx1999.top/gtpkfolgiv.html

[...new Set(arr)]
来源：http://hz.dianchejie.cn/gtwruymugf.html

[U90] JS：数字数组排序
来源：http://hz.cdnleiting.top/gthkblodtk.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtglcgpbzu.html

[U91] JS：对象键值遍历
来源：http://hz.zhixingplan.top/gtmdzmjiel.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.fengsongda.top/gtsowerxbh.html

[U92] JS：深拷贝
来源：http://hz.316326.xyz/gtzvrbbpsd.html

structuredClone(obj)
来源：http://hz.yuanzhike.top/gteuxlrzuz.html

[U93] JS：模板字符串
来源：http://hz.cheryme.top/gtlmgijykt.html

`共 ${n} 条`
来源：http://hz.ppjwa.cn/gtrxzcfhcv.html

[U94] JS：箭头函数
来源：http://hz.zhaomingkeji.xyz/gtjipdfymu.html

const double = x => x * 2;
来源：http://hz.nwbrower.top/gtcmmgdknh.html

[U95] JS：Promise 包装
来源：http://hz.316326.xyz/gtsvjcdcyr.html

new Promise((resolve, reject) => {})
来源：http://hz.yangfankeji.com/gtxvzovqaa.html

[U96] JS：async/await 与异常
来源：http://hz.cqqwz.cn/gtdphxmdfd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.redwolf501.top/gtkfnspvgd.html

[U97] JS：并发请求
来源：http://hz.nanxuanxn.top/gtlliwrmog.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtxslikgbv.html

[U98] JS：fetch 带 JSON
来源：http://hz.xylfe.cn/gtiraxplqp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jinqigufen.top/gterqtdvak.html

[U99] JS：事件监听
来源：http://hz.zhijiandao.cn/gtcgzylsoo.html

el.addEventListener("click", e => {})
来源：http://hz.xylfe.cn/gtwekiwcxw.html

[U100] JS：DOM 查询
来源：http://hz.ydjk.org.cn/gtbmsqbnah.html

document.querySelector(".item")
来源：http://hz.dashuyun.cn/gtmksoxgcb.html

[U101] JS：classList 操作
来源：http://hz.feifeiyinyue.top/gtdjtxvdqu.html

el.classList.toggle("active")
来源：http://hz.snrcjt.cn/gtlsjjkxaq.html

[U102] JS：本地存储
来源：http://hz.hammf.cn/gtjpxastyi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shanyushiyangkeji.top/gtzpsudwcp.html

[U103] JS：定时器
来源：http://hz.cheryme.top/gteazvklro.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhiwuduotai.top/gtvnwodnea.html

[U104] JS：防抖
来源：http://hz.havefunace.top/gttyeyqlvq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.birdmap.top/gtfxahauzm.html

[U105] JS：节流
来源：http://hz.shzxlz.cn/gtwmiefvnb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ybcxt.top/gtoihpapqd.html

[U106] JS：日期格式化
来源：http://hz.gotoacloud.top/gtwdwetnpg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxuanxn.top/gtrrpumsqu.html

[U107] JS：数字千分位
来源：http://hz.chenjidiqi.icu/gtbspspejv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jqgufenzy.top/gtnrbsfaed.html

[U108] JS：随机整数
来源：http://hz.zhongyouzk.top/gtuxdfhoka.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sweek.top/gtntbqighs.html

[U109] JS：数组分组
来源：http://hz.ydzc1.top/gttmgsuulu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinghuilouyu.cn/gtsqkamegm.html

[U110] JS：数组分块
来源：http://hz.yj20258888.top/gtdwhqzgyb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yangfankeji.com/gttjorvwzo.html

[U111] JS：对象转 Map
来源：http://hz.ehwqpu.com/gtrjlrjivk.html

new Map(Object.entries(obj))
来源：http://hz.jinyuanbaomall.cn/gtiebczurk.html

[U112] JS：字符串补位
来源：http://hz.jqgfzy.top/gthvnsqadz.html

"7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtmmbqzqtl.html

[U113] JS：正则替换全部
来源：http://hz.gzhubu.top/gtsrqolkre.html

s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtsjqmbgdy.html

[U114] JS：JSON 深比较
来源：http://hz.tianlin.xyz/gthwpqkibb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtjbcsaarv.html

[U115] JS：生成 UUID
来源：http://hz.tian-w.cn/gtodqxyylf.html

crypto.randomUUID()
来源：http://hz.hfpthk.cn/gtehahiqkt.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.chenjidiqi.icu/gtlumpnyut.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinqigfzy.top/gtmzwbpagm.html

[U117] JS：单元测试
来源：http://hz.yonumen.top/gtbahsyuxo.html

npm i -D vitest;  npx vitest
来源：http://hz.yj20258888.top/gtjllgxkdi.html

[U118] JS：开发服务器
来源：http://hz.jinghuilouyu.cn/gtcyldjxck.html

npm i -D vite;  npx vite
来源：http://hz.jiagoushi.top/gtgicqeadw.html

[U119] JS：生产构建
来源：http://hz.nwbrower.top/gtttqmcxal.html

npx vite build
来源：http://hz.hysaishi.cn/gtbwdfggdn.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ppjwa.cn/gtzpivydyy.html

import.meta.env.VITE_API_URL
来源：http://hz.cqqwz.cn/gtongunrrg.html

================================================================================
来源：http://hz.chenlongwang.top/gtzhmtoekq.html

统计汇总
来源：http://hz.shuidangran.top/gtsshmffnw.html

================================================================================
来源：http://hz.zhixingplan.top/gtzebugaji.html

按语言统计（条）：
来源：http://hz.yj20258888.top/gtzlrmrawr.html

Python ......... 252
来源：http://hz.xuanzx.com/gtooboiuoz.html

PHP ............ 252
来源：http://hz.jinqigfzy.top/gtiimtigzo.html

JavaScript ..... 252
来源：http://hz.zhongyouzk.top/gtvseejsep.html

TypeScript ..... 212
来源：http://hz.wangshuangyany.cn/gtnnxbgbjo.html

Java ........... 212
来源：http://hz.guowangkeji.top/gtupjwobtf.html

Go ............. 212
来源：http://hz.guowangkeji.top/gtxckmsdtu.html

Ruby ........... 212
来源：http://hz.yvedp.cn/gtjdnxlzdt.html

C# ............. 212
来源：http://hz.hnqzz.top/gtzuhjdeex.html

C .............. 30
来源：http://hz.zhongyouzk.top/gtyiwkuvwz.html

C++ ............ 30
来源：http://hz.yuanzhike.top/gtywerfmuu.html

SQL ............ 90
来源：http://hz.gotoacloud.top/gtwmctohla.html

Bash ........... 80
来源：http://hz.9152youxi.cn/gtcykhwcbo.html

Kotlin ......... 15
来源：http://hz.zhiwuduotai.top/gtmntqkmbc.html

Swift .......... 15
来源：http://hz.shanyushiyangkeji.top/gtdyfmjilz.html

Lua ............ 10
来源：http://hz.birdmap.top/gtcptjotru.html

Perl ........... 10
来源：http://hz.jinyuanbaomall.cn/gttwijoaxm.html

Scala .......... 10
来源：http://hz.zhengqikj.top/gtyidbforr.html

------------------------------------
来源：http://hz.hywenlv.cn/gtdxuiyucz.html

合计 ........... 2106 条
来源：http://hz.ehwqpu.com/gtplrvoezt.html

按章节统计：
来源：http://hz.meibo888.top/gtoeydtdpz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenjidiqi.icu/gtwvvakqny.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtmliuxkcl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gteinooymy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sufxvd.cn/gtercemixu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.aibaodan.cn/gtuudtlqgf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sysykeji.top/gtqmnkzfcn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xziqi.cn/gtnsfevaet.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhaomingkeji.xyz/gthuizipdw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtlrpddaun.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinghuilouyu.cn/gttjxcrlhv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtgvuyvzfn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtjplupfqs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtduvwnaks.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtwukgiqgi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.pycfn.com/gtutqbpyog.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtcqyntiin.html

Q SQL 专题                              90
来源：http://hz.9152youxi.cn/gtibkxaplx.html

R Bash 专题                             80
来源：http://hz.yongpay.top/gtexuhbnse.html

S C / C++ 专题                          60
来源：http://hz.xuanzx.com/gtcorwvxmi.html

T 其他语言补充                          60
来源：http://hz.sweek.top/gtfmuuluiz.html

U 高频实用片段                         120
来源：http://hz.sysykeji.top/gtccghroqb.html

------------------------------------
来源：http://hz.ywan-chungtsiang.top/gtbveldiqz.html

合计                                  2106 条
来源：http://hz.shanyushiyangtech.top/gtjddjkslt.html

--------------------------------------------------------------------------------
来源：http://hz.wangdashe.top/gtmlsoseuy.html

使用提醒
来源：http://hz.fengsongda.top/gthtsvaqzu.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtmhwuapqg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinyuanbaomall.cn/gtfjijcypz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xylfe.cn/gtfpwilmup.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cashguo.top/gtvkvjhqxt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.wangdashe.top/gtmwdvpdcs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cucudq.cn/gtwmhojgsp.html

—— 文件结束 ——
来源：http://hz.ydzc1.top/gtrbqhreau.html

================================================================================
来源：http://hz.bjfxy.top/gtvaiicyia.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.wangshuangyany.cn/gtpttmncsy.html

Common Programming Examples Cheat Book
来源：http://hz.shanyushiyangkeji.top/gtciedmuvk.html

================================================================================
来源：http://hz.nanxinkj.top/gtleznlfrz.html

【收录内容】
来源：http://hz.smart0.xyz/gtdnhkedvp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.mhx1999.top/gtbwoxicrq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.daxiang520.top/gthuigcczh.html

SQL · Bash · C · C++
来源：http://hz.gaohongyu789.top/gtovblavgk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.nwbrower.top/gtcplobqca.html

【使用说明】
来源：http://hz.gogol.net.cn/gtocjvosgt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.chenlongwang.top/gtnnctdngs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yueranfly.top/gtlnhepevg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.52xcode.cn/gtlhscsxmv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zycfv.cn/gtwaoaxnwg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yj20258888.top/gtkvvoxwry.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xylfe.cn/gtiqzxkebc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zhoulong.xyz/gtxkwdbrnh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.guannengcc.top/gtfspvwcjk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xingfuxueyuan.xyz/gtnokbvrlb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhixingplan.top/gtyuqlvxxt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xinyue.icu/gtdkuiftgn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinqigufen.top/gtrvuipxcc.html

【文件统计】
来源：http://hz.wangshuangyany.cn/gtoshnszbz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.feifeiyinyue.top/gtpiedixan.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtzahcagud.html

目  录
来源：http://hz.sysykeji.top/gtxwqscyuz.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gthuwycfdz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hammf.cn/gtursejuri.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhiwuduotai.top/gtwddxwsoq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.fzhhl.top/gtzvmscduk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.9152youxi.cn/gtdtalhjjj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.vqdsnc.cn/gtpuzrmxig.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.havefunace.top/gthdyiulmh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xingfuxueyuan.xyz/gtvcnrghpw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.tian-w.cn/gtgtvfugza.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.sysykeji.top/gtsubbajtw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cashguo.top/gtxumlwxwl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.pycfn.com/gtzzzhtbyb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtcauckzjf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtabgolxbn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.chenjidiqi.icu/gttoatanyv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.gotoacloud.top/gtktdsemji.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zhijiandao.cn/gtydspnchk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhijiandao.cn/gtduuyfmax.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.chenlongwang.top/gtqxdooyin.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhixingplan.top/gtjhqjtrju.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhiwuduotai.top/gtfupvdxzl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj202588.top/gtfuqsuivs.html

================================================================================
来源：http://hz.c1oappe.top/gtxacvghee.html

A. 基础语法与类型
来源：http://hz.jyoumei.cn/gtjklggmvq.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvwqscsoj.html

[A01] Hello World
来源：http://hz.zhiwuduotai.top/gtsbsujmht.html

Py:   print("Hello, World!")
来源：http://hz.ybcxt.top/gthwbrbksi.html

PHP:  echo "Hello, World!";
来源：http://hz.quarkkingdee.top/gtubiszmvr.html

JS:   console.log("Hello, World!");
来源：http://hz.sxryk.cn/gtuawaohlv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj20258888.top/gtekjsctse.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenzaomai.com/gtjcrychip.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.0kj1m.cn/gtjqdqdszu.html

Ruby: puts "Hello, World!"
来源：http://hz.yj20258.top/gtwmuxxoev.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cashguo.top/gtbglcxmjj.html

[A02] 变量声明与赋值
来源：http://hz.shanyushiyangkeji.top/gtpgkmolmk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.tian-w.cn/gthjvvcbmh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.svipenyu.cn/gtnmyonxaz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenlongwang.top/gtdfvdkysx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.mhx1999.top/gttybacmgl.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.chenlongwang.top/gtplrhjuxt.html

Go:   name := "Alex"; age := 20
来源：http://hz.shzxlz.cn/gtqpxsljss.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cqqwz.cn/gttwevvhhj.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xinyue.icu/gtjzxudawb.html

[A03] 常量定义
来源：http://hz.yuxming.cn/gtxyemjoix.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.nwbrower.top/gtsfizwnds.html

PHP:  const PI = 3.14159;
来源：http://hz.gzhubu.top/gtsykrdbbt.html

JS:   const PI = 3.14159;
来源：http://hz.jiagoushi.top/gtdjxxbccp.html

TS:   const PI: number = 3.14159;
来源：http://hz.xuanzx.com/gtjdkvkhdh.html

Java: static final double PI = 3.14159;
来源：http://hz.c1oappe.top/gtixmpzhqf.html

Go:   const PI = 3.14159
来源：http://hz.yangfankeji.com/gtgadmsjgn.html

Ruby: PI = 3.14159
来源：http://hz.meibo888.top/gtmsmqeltm.html

C#:   const double PI = 3.14159;
来源：http://hz.birdmap.top/gtlizinvkm.html

[A04] 判断变量类型
来源：http://hz.ehwqpu.com/gtpditrnmc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.vqdsnc.cn/gtrmrgdtki.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zycfv.cn/gtfnhcynib.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.havefunace.top/gtkiljfkzs.html

TS:   typeof x; x instanceof Date
来源：http://hz.yj202588.top/gtnwmvrhri.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hnxiangtu.top/gtalsizpuw.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.andypj.xyz/gtmjlfdtwk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.mhx1999.top/gtvwahydxp.html

C#:   x.GetType().Name; x is int
来源：http://hz.xuanzx.com/gtngmfjnoj.html

[A05] 整数除法与取模
来源：http://hz.jinghuilouyu.cn/gtvufgzuix.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.tianlin.xyz/gtvfuvitou.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.gotoacloud.top/gtesvcseic.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yuanzhike.top/gtkzeqpgnm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tian-w.cn/gtlyfpxcgo.html

Java: 7 / 2; 7 % 2
来源：http://hz.meibo888.top/gtqhyduohf.html

Go:   7 / 2; 7 % 2
来源：http://hz.fengsongda.top/gtovmsknmz.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zhiwuduotai.top/gtxjpqfrik.html

C#:   7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtrgsktkod.html

[A06] 字符串转数字
来源：http://hz.hysaishi.cn/gtqypwhpwk.html

Py:   int("42"); float("3.14")
来源：http://hz.xingfuxueyuan.xyz/gtjezftidd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ybcxt.top/gtgbuqyrfo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hnqzz.top/gtrjsynodq.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.iojbl.cn/gtbiqivcad.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.gzhubu.top/gtcbzdhpim.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.pycfn.com/gtkovnlgay.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.shanyushiyangtech.top/gtctrkazuw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zhaomingkeji.xyz/gtvnjwtshr.html

[A07] 数字转字符串
来源：http://hz.gotoacloud.top/gtgitfkroi.html

Py:   str(42)
来源：http://hz.cheryme.top/gtspzwljqg.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhixingplan.top/gtrwkxammh.html

JS:   String(42); (42).toString()
来源：http://hz.guowangkeji.top/gtdvgltqrg.html

TS:   String(42)
来源：http://hz.guowangkeji.top/gtrghmylyg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zdqjudy.top/gtnhmorgkp.html

Go:   strconv.Itoa(42)
来源：http://hz.yueranfly.top/gtillxvnrp.html

Ruby: 42.to_s
来源：http://hz.yanxiufei.cn/gtjyswcdls.html

C#:   42.ToString()
来源：http://hz.pengpengdd.cyou/gtqfzwfstv.html

[A08] 取整与四舍五入
来源：http://hz.hnqzz.top/gtiiudwtll.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.dashuyun.cn/gtwjzeyrsv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.shangyingyoupin.top/gtsdwlosxf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.52xcode.cn/gtueawksoq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.0kj1m.cn/gteddusins.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.pycfn.com/gtnvllljge.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yj202588.top/gtyoerzcrt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.gotoacloud.top/gtkwdjgkec.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.sysykeji.top/gtunekqyhy.html

[A09] 绝对值与最大最小值
来源：http://hz.yj20258.top/gtxlyujhpm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.fengsongda.top/gtansleisy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.gaohongyu789.top/gtecbjlqug.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.andypj.xyz/gtcjcdcrzc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.cheryme.top/gtpeqgwvtw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.haohaochexian.top/gtapviicsj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.havefunace.top/gtmnnwlbxt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.ydjk.org.cn/gtilyfzmel.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yongpay.top/gtefzmjyqo.html

[A10] 生成随机数
来源：http://hz.yj20258.top/gtwpgwqreo.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zhijiandao.cn/gtpeyysxcw.html

PHP:  random_int(1, 100);
来源：http://hz.jyoumei.cn/gteauqtukv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hnxiangtu.top/gtbcumwozk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.redwolf501.top/gtyokqksbg.html

Java: new Random().nextInt(100) + 1
来源：http://hz.snrcjt.cn/gthkkfapno.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.sysykeji.top/gtikduaraz.html

Ruby: rand(1..100)
来源：http://hz.yangfankeji.com/gtqnqguipu.html

C#:   new Random().Next(1, 101)
来源：http://hz.xuanzx.com/gtliszdkqb.html

[A11] 条件表达式（三元）
来源：http://hz.ydjk.org.cn/gtolokfrjl.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.cucudq.cn/gthpmwzyiq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.xinyue.icu/gtbhbtxfew.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yongpay.top/gtpnxvgpve.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.andypj.xyz/gtiyhfiacq.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.redwolf501.top/gtepbszncb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.hfpthk.cn/gtmppgjsdf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.fzhhl.top/gtemeanycp.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.dashuyun.cn/gtwljoocmc.html

[A12] 字符串插值 / 格式化
来源：http://hz.birdmap.top/gtavzzahcb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.pengpengdd.cyou/gtqwdtpyba.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.pengpengdd.cyou/gtovozygcq.html

JS:   `Hello, ${name}!`
来源：http://hz.cdnleiting.top/gthrxczrlg.html

TS:   `Hello, ${name}!`
来源：http://hz.zhixingplan.top/gthhmammsi.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.tian-w.cn/gtulgjdefs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.zhiwuduotai.top/gtirzrfguh.html

Ruby: "Hello, #{name}!"
来源：http://hz.jyoumei.cn/gtpwjvktrd.html

C#:   $"Hello, {name}!"
来源：http://hz.yonumen.top/gtekdfozsm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.c1oappe.top/gtqketttcn.html

Py:   "第一行\n第二行"
来源：http://hz.tianlin.xyz/gtotpzdsym.html

PHP:  "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gttwsmvtrw.html

JS:   "第一行\n第二行"
来源：http://hz.yj20258.top/gtyjpfukdb.html

TS:   "第一行\n第二行"
来源：http://hz.meibo888.top/gthigajbmo.html

Java: "第一行\n第二行"
来源：http://hz.jianghu66.top/gtiqjyrycq.html

Go:   "第一行\n第二行"
来源：http://hz.yuanzhike.top/gtlrmbrpsl.html

Ruby: "第一行\n第二行"
来源：http://hz.9152youxi.cn/gtstemymmf.html

C#:   "第一行\n第二行"
来源：http://hz.andypj.xyz/gtnidyviay.html


<!-- 参考信息 -->