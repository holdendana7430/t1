代发 wailian999

[U95] JS：Promise 包装
来源：http://hz.quarkkingdee.top/gtlcqujuwz.html

new Promise((resolve, reject) => {})
来源：http://hz.andypj.xyz/gtoussdnpz.html

[U96] JS：async/await 与异常
来源：http://hz.xuetiantiany.cn/gtuuqjjtoa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yvedp.cn/gtkpylvcdn.html

[U97] JS：并发请求
来源：http://hz.yvedp.cn/gtfxcxgglf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtbcfecpbv.html

[U98] JS：fetch 带 JSON
来源：http://hz.hfpthk.cn/gtvsvrmzjo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ydzc1.top/gtlywlydnp.html

[U99] JS：事件监听
来源：http://hz.snrcjt.cn/gtaywfsfjq.html

el.addEventListener("click", e => {})
来源：http://hz.0kj1m.cn/gtmwrpigmi.html

[U100] JS：DOM 查询
来源：http://hz.jiagoushi.top/gtiqwdlpjs.html

document.querySelector(".item")
来源：http://hz.jyoumei.cn/gtmhvgmzme.html

[U101] JS：classList 操作
来源：http://hz.haohaochexian.top/gtjkibonye.html

el.classList.toggle("active")
来源：http://hz.jinqigfzy.top/gtcrannmem.html

[U102] JS：本地存储
来源：http://hz.yangfankeji.com/gtqqqicekr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ehwqpu.com/gthbgmkzct.html

[U103] JS：定时器
来源：http://hz.shanyushiyangtech.top/gtxtukefbr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.c1oappe.top/gtnhdrbqbn.html

[U104] JS：防抖
来源：http://hz.aibaodan.cn/gttfqiuuxz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtnqvsiyrc.html

[U105] JS：节流
来源：http://hz.jinghuilouyu.cn/gtmdpkbice.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dashuyun.cn/gtpifzruyh.html

[U106] JS：日期格式化
来源：http://hz.haohaochexian.top/gtfaqyugfi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hnqzz.top/gtomyezqgg.html

[U107] JS：数字千分位
来源：http://hz.9152youxi.cn/gthmmcgdgi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.aibaodan.cn/gtuevqhuii.html

[U108] JS：随机整数
来源：http://hz.zycfv.cn/gtymxaunjh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sweek.top/gtlbmkgqog.html

[U109] JS：数组分组
来源：http://hz.xylfe.cn/gtevosmqvv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jlsjyb.cn/gtwihpzzex.html

[U110] JS：数组分块
来源：http://hz.0kj1m.cn/gtlxohfebw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.chenzaomai.com/gtqsvjgzgz.html

[U111] JS：对象转 Map
来源：http://hz.gaohongyu789.top/gtqldlmbxq.html

new Map(Object.entries(obj))
来源：http://hz.ehwqpu.com/gtrgoasjkj.html

[U112] JS：字符串补位
来源：http://hz.ybcxt.top/gtohsuejks.html

"7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtuitqcblt.html

[U113] JS：正则替换全部
来源：http://hz.cqqwz.cn/gtbdfndrbb.html

s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtxuoisnvy.html

[U114] JS：JSON 深比较
来源：http://hz.chenjidiqi.icu/gtmvkmheks.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtqbqxcqis.html

[U115] JS：生成 UUID
来源：http://hz.gotoacloud.top/gtsuqchomd.html

crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gtskszfvha.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.c1oappe.top/gtviosnrsg.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sxryk.cn/gtcjyqcgvd.html

[U117] JS：单元测试
来源：http://hz.daria6918.cn/gtpztxgwfc.html

npm i -D vitest;  npx vitest
来源：http://hz.yj20258.top/gtphcsbwcc.html

[U118] JS：开发服务器
来源：http://hz.hongshengwenyu.top/gtltavkpal.html

npm i -D vite;  npx vite
来源：http://hz.yj20258888.top/gtwyrnvuwz.html

[U119] JS：生产构建
来源：http://hz.daria6918.cn/gtdrufwuvz.html

npx vite build
来源：http://hz.9152youxi.cn/gtkozjcpzu.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.pengpengdd.cyou/gtblrxecsd.html

import.meta.env.VITE_API_URL
来源：http://hz.daria6918.cn/gtqitiahtg.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgftcpzuh.html

统计汇总
来源：http://hz.c1oappe.top/gtqjbbpols.html

================================================================================
来源：http://hz.nanxinkj.top/gtpbhubtbm.html

按语言统计（条）：
来源：http://hz.9152youxi.cn/gtbqziwvhs.html

Python ......... 252
来源：http://hz.nwbrower.top/gtgwaznmns.html

PHP ............ 252
来源：http://hz.sxryk.cn/gtlmfgocdv.html

JavaScript ..... 252
来源：http://hz.yangfankeji.com/gtflgzssjf.html

TypeScript ..... 212
来源：http://hz.nanxinkj.top/gtgizpaiid.html

Java ........... 212
来源：http://hz.sweek.top/gtflptmmkz.html

Go ............. 212
来源：http://hz.tanke756.top/gtqxsqajgr.html

Ruby ........... 212
来源：http://hz.jyoumei.cn/gtxzlgqgls.html

C# ............. 212
来源：http://hz.yj20258888.top/gtzjcoaffv.html

C .............. 30
来源：http://hz.quarkkingdee.top/gtcptvteej.html

C++ ............ 30
来源：http://hz.shangyingyoupin.top/gtxncjdnsg.html

SQL ............ 90
来源：http://hz.cucudq.cn/gtvwjbxqoq.html

Bash ........... 80
来源：http://hz.ppjwa.cn/gtjfvxovuo.html

Kotlin ......... 15
来源：http://hz.daxiang520.top/gtnjxxvmrl.html

Swift .......... 15
来源：http://hz.haohaochexian.top/gtyzyxvujf.html

Lua ............ 10
来源：http://hz.jlsjyb.cn/gtqntbxvdr.html

Perl ........... 10
来源：http://hz.yvedp.cn/gtrlvablgu.html

Scala .......... 10
来源：http://hz.52xcode.cn/gtpmowxmlr.html

------------------------------------
来源：http://hz.jinqigufen.top/gtiobpishw.html

合计 ........... 2106 条
来源：http://hz.svipenyu.cn/gtstqxxpon.html

按章节统计：
来源：http://hz.sweek.top/gtvyeupibt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.sweek.top/gtlrsrpccm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.wangdashe.top/gthjwccrim.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtverohntt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.aibaodan.cn/gtxbyzoiiu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.birdmap.top/gtouipmjiy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jqgfzy.top/gtgavlieff.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gtmszqzxsh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ehwqpu.com/gtqwcflxwc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtxzyutgee.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jlsjyb.cn/gtzaednwry.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtqxlkzujh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtafpzhgsf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtnxkmhqkp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhijiandao.cn/gtcexjxakg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shanyushiyangtech.top/gtamqldaus.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtvzuyfxsc.html

Q SQL 专题                              90
来源：http://hz.zhoulong.xyz/gtdwyrhecz.html

R Bash 专题                             80
来源：http://hz.yuxming.cn/gttumxlgam.html

S C / C++ 专题                          60
来源：http://hz.xylfe.cn/gtuerhseop.html

T 其他语言补充                          60
来源：http://hz.ehwqpu.com/gtgztqlmor.html

U 高频实用片段                         120
来源：http://hz.pengpengdd.cyou/gtoxxxlqvf.html

------------------------------------
来源：http://hz.tian-w.cn/gtotikxute.html

合计                                  2106 条
来源：http://hz.jyoumei.cn/gtvqdvzpqf.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtehksmnbq.html

使用提醒
来源：http://hz.havefunace.top/gtnlwozhas.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtbopbgtvb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.havefunace.top/gthrtyuudy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ydjk.org.cn/gtnzgsbzhv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhengqikj.top/gtmvllfqbr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ydjk.org.cn/gtlmbjatlt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jianghu66.top/gtagcjbpan.html

—— 文件结束 ——
来源：http://hz.yuxming.cn/gtldklsklr.html

================================================================================
来源：http://hz.zhengqikj.top/gtnftlwjwj.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.guowangkeji.top/gtwppejjuo.html

Common Programming Examples Cheat Book
来源：http://hz.xuanzx.com/gtwgcmhiqb.html

================================================================================
来源：http://hz.cheryme.top/gtviqroagc.html

【收录内容】
来源：http://hz.ppjwa.cn/gthdftbdiz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cqqwz.cn/gtilgcfwvx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shzxlz.cn/gtwnbeblrn.html

SQL · Bash · C · C++
来源：http://hz.zhengqikj.top/gtghhrompk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hywenlv.cn/gtrnlkkmuh.html

【使用说明】
来源：http://hz.jqgufenzy.top/gtupruuxfq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yueranfly.top/gtdbkbxjqz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.gotoacloud.top/gtomevelof.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.meibo888.top/gtnyjrchwp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.nanxuanxn.top/gtsqknxezv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.pengpengdd.cyou/gtfyneqbrf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.nwbrower.top/gtulnxnnsv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xuanzx.com/gtpcjcurvs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.sufxvd.cn/gtrijjsljy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.52xcode.cn/gtclhqkkwk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ybcxt.top/gtddkbjyms.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ybcxt.top/gtytaeblrh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.nwbrower.top/gtnybszwag.html

【文件统计】
来源：http://hz.fengsongda.top/gtdbrdqzxz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.guowangkeji.top/gtqgtydihr.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtaavvsuoj.html

目  录
来源：http://hz.dianchejie.cn/gtggfpopfu.html

--------------------------------------------------------------------------------
来源：http://hz.ywan-chungtsiang.top/gtqdgodgmv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.svipenyu.cn/gtxclpfgoq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhiwuduotai.top/gtxwzuvqjd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.daria6918.cn/gtmmlpfoes.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ydjk.org.cn/gtmcytlhsk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jiagoushi.top/gtvxqikcdn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.kuanghao11.cn/gtlwmwmzlr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.c1oappe.top/gtkpqqjpji.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shangyingyoupin.top/gtblzjqjlr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtbbxsbjqg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.52xcode.cn/gtcaspsgyy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtudqmixcf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtpsloaiqo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtvroxpkrd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhengqikj.top/gtpoqtfgjq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ydzc1.top/gtkaopqvzq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtgafdnytz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.chenlongwang.top/gtedtoybnm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhoulong.xyz/gtgnpspxob.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.meibo888.top/gtmfekcoas.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hammf.cn/gtyvrhxfwu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.gotoacloud.top/gtnjkrupmu.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtevqzrdub.html

A. 基础语法与类型
来源：http://hz.bjfxy.top/gtbdhukimc.html

================================================================================
来源：http://hz.guannengcc.top/gtncyzvadz.html

[A01] Hello World
来源：http://hz.ybcxt.top/gtlliqoshg.html

Py:   print("Hello, World!")
来源：http://hz.vqdsnc.cn/gtrzfofdbm.html

PHP:  echo "Hello, World!";
来源：http://hz.jinqigufen.top/gtewcsgwcc.html

JS:   console.log("Hello, World!");
来源：http://hz.zdqjudy.top/gtrvrxuyyu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ehwqpu.com/gtmjnbyifi.html

Java: System.out.println("Hello, World!");
来源：http://hz.aibaodan.cn/gtzlknfimp.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.feifeiyinyue.top/gtzqlvcujd.html

Ruby: puts "Hello, World!"
来源：http://hz.yongpay.top/gttmldmzze.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cucudq.cn/gtyjwhsdgk.html

[A02] 变量声明与赋值
来源：http://hz.svipenyu.cn/gtxomvpycr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.chenjidiqi.icu/gtvvyuzubh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yuanzhike.top/gtkfzipdft.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ybcxt.top/gtazeokgpq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yonumen.top/gteckcdyhv.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zdqjudy.top/gtsytqkjzm.html

Go:   name := "Alex"; age := 20
来源：http://hz.ivvv.top/gtakegvdin.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yuxming.cn/gtjrlxxtde.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jqgfzy.top/gtzcysuwga.html

[A03] 常量定义
来源：http://hz.pycfn.com/gthjdydjoi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.quarkkingdee.top/gtnxbcakec.html

PHP:  const PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtqeyztuea.html

JS:   const PI = 3.14159;
来源：http://hz.daria6918.cn/gtcckderxw.html

TS:   const PI: number = 3.14159;
来源：http://hz.jqgfzy.top/gtisoszngb.html

Java: static final double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtjfynddav.html

Go:   const PI = 3.14159
来源：http://hz.xinyue.icu/gtefrauhdb.html

Ruby: PI = 3.14159
来源：http://hz.c1oappe.top/gtjnbxatjf.html

C#:   const double PI = 3.14159;
来源：http://hz.andypj.xyz/gtlxvyqxgo.html

[A04] 判断变量类型
来源：http://hz.hnxiangtu.top/gtkhijirqw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinqigfzy.top/gtcqhkeoyb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ivvv.top/gteyyqvctc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.xinyue.icu/gtpeofhmro.html

TS:   typeof x; x instanceof Date
来源：http://hz.xuetiantiany.cn/gtkqkpudgn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.dashuyun.cn/gtduqmrywd.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shuidangran.top/gtgzhjssqw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zycfv.cn/gtwddtkzvb.html

C#:   x.GetType().Name; x is int
来源：http://hz.nanxinkj.top/gtoqukqfpm.html

[A05] 整数除法与取模
来源：http://hz.dashuyun.cn/gtswkkajgd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.smart0.xyz/gtuiauictx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.dianchejie.cn/gtiqczofre.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tian-w.cn/gtwstwlyxw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yongpay.top/gtjaehrzcd.html

Java: 7 / 2; 7 % 2
来源：http://hz.zycfv.cn/gtzbskhysa.html

Go:   7 / 2; 7 % 2
来源：http://hz.ivvv.top/gtxaqsoopi.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtdbnzsupu.html

C#:   7 / 2; 7 % 2
来源：http://hz.jiagoushi.top/gtebbmalsw.html

[A06] 字符串转数字
来源：http://hz.tian-w.cn/gtjvatsaww.html

Py:   int("42"); float("3.14")
来源：http://hz.yangfankeji.com/gtgeehhamd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jqgfzy.top/gtwujjnfya.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.snrcjt.cn/gtsbvrlnft.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ydjk.org.cn/gtkiyqrfwv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.chenjidiqi.icu/gticyuvrwk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.haohaochexian.top/gtbwvctqow.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yuanzhike.top/gtwjsowcyh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.9152youxi.cn/gtpsvmgfyo.html

[A07] 数字转字符串
来源：http://hz.yangfankeji.com/gtwfwwkdjc.html

Py:   str(42)
来源：http://hz.xylfe.cn/gtudpylqty.html

PHP:  (string) 42; strval(42)
来源：http://hz.jqgfzy.top/gtjllninzp.html

JS:   String(42); (42).toString()
来源：http://hz.birdmap.top/gtatkrolpn.html

TS:   String(42)
来源：http://hz.xylfe.cn/gtgqjsjofy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.gotoacloud.top/gtvjtqdskr.html

Go:   strconv.Itoa(42)
来源：http://hz.havefunace.top/gtyqwzufsb.html

Ruby: 42.to_s
来源：http://hz.hnqzz.top/gtruhjywyz.html

C#:   42.ToString()
来源：http://hz.mhx1999.top/gtqpkhfmcw.html

[A08] 取整与四舍五入
来源：http://hz.ydjk.org.cn/gtlcdaibid.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtpqrycftl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.ydjk.org.cn/gtcusmvunf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.tianlin.xyz/gtexckwhta.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.aibaodan.cn/gtttpcjuve.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.cdnleiting.top/gthvlbxwsp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.vqdsnc.cn/gtxpjgkpud.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.sysykeji.top/gtgdonjfeb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtebjcgbqy.html

[A09] 绝对值与最大最小值
来源：http://hz.shanyushiyangtech.top/gtvxrgugwz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.316326.xyz/gtzswdkwjf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.snrcjt.cn/gtszkqgnea.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.quarkkingdee.top/gtcpxgecoq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shuidangran.top/gtrqunexxp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhiwuduotai.top/gtfkndrhvc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.hammf.cn/gtltcceuiv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.yangfankeji.com/gtxaojwexk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.vqdsnc.cn/gtscjswhbq.html

[A10] 生成随机数
来源：http://hz.fengsongda.top/gtwdugqlla.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ppjwa.cn/gtbbrhfaph.html

PHP:  random_int(1, 100);
来源：http://hz.smart0.xyz/gtogwvdagc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhoulong.xyz/gtiejsekmc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ppjwa.cn/gtpxmafney.html

Java: new Random().nextInt(100) + 1
来源：http://hz.meibo888.top/gtjiyvmeyu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.daxiang520.top/gtgxzwudff.html

Ruby: rand(1..100)
来源：http://hz.ywan-chungtsiang.top/gtbhuoxnhm.html

C#:   new Random().Next(1, 101)
来源：http://hz.jinqigufen.top/gtggftzbdy.html

[A11] 条件表达式（三元）
来源：http://hz.svipenyu.cn/gtdqrbesub.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jqgufenzy.top/gtcscdnwij.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.haohaochexian.top/gtaitsxpgu.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.316326.xyz/gtpbummmzr.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.gotoacloud.top/gtknuvcubr.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.pycfn.com/gtoxngubvs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.aibaodan.cn/gtsoesliqi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.cheryme.top/gtrrgnpodf.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.andypj.xyz/gtvdrafvby.html

[A12] 字符串插值 / 格式化
来源：http://hz.smart0.xyz/gtnyiwsbec.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.gogol.net.cn/gtbmkdnhbh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.svipenyu.cn/gtgacdvawz.html

JS:   `Hello, ${name}!`
来源：http://hz.cheryme.top/gtvzbgvzvt.html

TS:   `Hello, ${name}!`
来源：http://hz.hongshengwenyu.top/gttcugyrkv.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.sxryk.cn/gtshfyuzzj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jinqigufen.top/gtpaifcfei.html

Ruby: "Hello, #{name}!"
来源：http://hz.52xcode.cn/gtukanulvg.html

C#:   $"Hello, {name}!"
来源：http://hz.jinghuilouyu.cn/gttsgrmudb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.cqqwz.cn/gtdvwrfhib.html

Py:   "第一行\n第二行"
来源：http://hz.cucudq.cn/gtlgoteoqe.html

PHP:  "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtlxowmvpz.html

JS:   "第一行\n第二行"
来源：http://hz.fzhhl.top/gthqymerik.html

TS:   "第一行\n第二行"
来源：http://hz.jinqigfzy.top/gtnaqbtnfb.html

Java: "第一行\n第二行"
来源：http://hz.52xcode.cn/gtnqstbclc.html

Go:   "第一行\n第二行"
来源：http://hz.smart0.xyz/gtqgkiaamp.html

Ruby: "第一行\n第二行"
来源：http://hz.ybcxt.top/gtwzudygps.html

C#:   "第一行\n第二行"
来源：http://hz.c1oappe.top/gtrurfiukd.html

[A14] 注释写法
来源：http://hz.mhx1999.top/gtqtslmptk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.gogol.net.cn/gtypsfuenk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hywenlv.cn/gtlbkkubdb.html

JS:   // 单行；/* 多行 */
来源：http://hz.sufxvd.cn/gtwhtjtpmy.html

TS:   // 单行；/* 多行 */
来源：http://hz.shangyingyoupin.top/gtnaadnrlk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.guannengcc.top/gtmbuohqkr.html

Go:   // 单行；/* 多行 */
来源：http://hz.fengsongda.top/gtcopltnnz.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.chenlongwang.top/gtleecomjs.html

C#:   // 单行；/* 多行 */
来源：http://hz.kuanghao11.cn/gtluhwbyhx.html

[A15] 空值判断与默认值
来源：http://hz.jianghu66.top/gtkgxnmiuy.html

Py:   value = data or "默认值"
来源：http://hz.yangfankeji.com/gtaohlaopb.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.shangyingyoupin.top/gtiodqhvsl.html

JS:   const value = data ?? "默认值";
来源：http://hz.mhx1999.top/gtqthzmave.html

TS:   const value = data ?? "默认值";
来源：http://hz.iojbl.cn/gtdxbtlisc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.daxiang520.top/gtoouevwya.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.ppjwa.cn/gtqzacjtes.html

Ruby: value = data || "默认值"
来源：http://hz.feifeiyinyue.top/gtnjwcjwyx.html

C#:   var value = data ?? "默认值";
来源：http://hz.zhoulong.xyz/gtmjkeufgi.html

[A16] 真假值判断规则
来源：http://hz.hysaishi.cn/gttldgsoje.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yonumen.top/gtrjioofmc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.birdmap.top/gtafbjuirc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.hysaishi.cn/gtzunigfvl.html

TS:   if (!x) {}
来源：http://hz.yuanzhike.top/gtoslmaazr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.cdnleiting.top/gtlrpxdlic.html


<!-- 参考信息 -->