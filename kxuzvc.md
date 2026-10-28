代发 wailian999

[U87] JS：解构默认值
来源：http://hz.bjfxy.top/gtqtingglq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ydjk.org.cn/gtyuigtzal.html

[U88] JS：对象展开合并
来源：http://hz.xingfuxueyuan.xyz/gtdmwqqjjw.html

{ ...a, ...b }
来源：http://hz.tian-w.cn/gtgfmxioeg.html

[U89] JS：数组去重
来源：http://hz.hysaishi.cn/gtlyyylktd.html

[...new Set(arr)]
来源：http://hz.birdmap.top/gtafesmxfw.html

[U90] JS：数字数组排序
来源：http://hz.shanyushiyangkeji.top/gternftdpi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtlxxfozfg.html

[U91] JS：对象键值遍历
来源：http://hz.nanxuanxn.top/gtrniunwsy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yangfankeji.com/gtmsafzrnw.html

[U92] JS：深拷贝
来源：http://hz.hfpthk.cn/gtamjhbgze.html

structuredClone(obj)
来源：http://hz.birdmap.top/gtvlrwfouj.html

[U93] JS：模板字符串
来源：http://hz.cqqwz.cn/gtlbfcqkpq.html

`共 ${n} 条`
来源：http://hz.hnxiangtu.top/gtfpxwchpd.html

[U94] JS：箭头函数
来源：http://hz.sweek.top/gtwhxnwjsl.html

const double = x => x * 2;
来源：http://hz.cdnleiting.top/gtcymhejlt.html

[U95] JS：Promise 包装
来源：http://hz.cdnleiting.top/gtqhdogeho.html

new Promise((resolve, reject) => {})
来源：http://hz.nanxinkj.top/gttilaosqz.html

[U96] JS：async/await 与异常
来源：http://hz.xziqi.cn/gtwlhcyblr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sxryk.cn/gtkalslfjd.html

[U97] JS：并发请求
来源：http://hz.zhijiandao.cn/gteezigzux.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtvtdoblmx.html

[U98] JS：fetch 带 JSON
来源：http://hz.xuanzx.com/gtrvjrgxgz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.chenlongwang.top/gtpsdqnvwc.html

[U99] JS：事件监听
来源：http://hz.nanxuanxn.top/gtqlozlabl.html

el.addEventListener("click", e => {})
来源：http://hz.iojbl.cn/gtdknphvbn.html

[U100] JS：DOM 查询
来源：http://hz.vqdsnc.cn/gtauhchaxh.html

document.querySelector(".item")
来源：http://hz.yangfankeji.com/gtcmnbodbx.html

[U101] JS：classList 操作
来源：http://hz.zycfv.cn/gtdcchsdhc.html

el.classList.toggle("active")
来源：http://hz.hammf.cn/gtfluilufw.html

[U102] JS：本地存储
来源：http://hz.kuanghao11.cn/gtwlxeuctv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xinyue.icu/gtpjphgmzq.html

[U103] JS：定时器
来源：http://hz.ydzc1.top/gthczxivxi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sufxvd.cn/gtwgsmvkkp.html

[U104] JS：防抖
来源：http://hz.smart0.xyz/gtyrarcnvg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtxtrzxmqg.html

[U105] JS：节流
来源：http://hz.tanke756.top/gtcfzqwxir.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.iojbl.cn/gtocnjmbxf.html

[U106] JS：日期格式化
来源：http://hz.nwbrower.top/gtqmavmxdn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxinkj.top/gtexrdgbfd.html

[U107] JS：数字千分位
来源：http://hz.zhongyouzk.top/gtouzgdqls.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinqigfzy.top/gtydgvmjsh.html

[U108] JS：随机整数
来源：http://hz.jqgufenzy.top/gtvstuzdza.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.daxiang520.top/gtihqxnlfq.html

[U109] JS：数组分组
来源：http://hz.jqgufenzy.top/gtdmzufhuq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigfzy.top/gtenoaxlxq.html

[U110] JS：数组分块
来源：http://hz.hfpthk.cn/gtimgmnbgw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhengqikj.top/gtlfbjliyn.html

[U111] JS：对象转 Map
来源：http://hz.zhengqikj.top/gtvxmyicrr.html

new Map(Object.entries(obj))
来源：http://hz.gogol.net.cn/gtwnsiurqj.html

[U112] JS：字符串补位
来源：http://hz.kuanghao11.cn/gturakkyux.html

"7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtrwttfjnm.html

[U113] JS：正则替换全部
来源：http://hz.gzhubu.top/gtzivtywkw.html

s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gttephjaqn.html

[U114] JS：JSON 深比较
来源：http://hz.yonumen.top/gtcmtqvzfh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtwhlzqwnd.html

[U115] JS：生成 UUID
来源：http://hz.ywan-chungtsiang.top/gtnvmxgapo.html

crypto.randomUUID()
来源：http://hz.wangshuangyany.cn/gttjnblrlp.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhixingplan.top/gtefnyzzvy.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shanyushiyangkeji.top/gtxzgkgnzl.html

[U117] JS：单元测试
来源：http://hz.dianchejie.cn/gtmqqjeuws.html

npm i -D vitest;  npx vitest
来源：http://hz.xuetiantiany.cn/gtxwpvznwp.html

[U118] JS：开发服务器
来源：http://hz.quarkkingdee.top/gtwsvxphzm.html

npm i -D vite;  npx vite
来源：http://hz.zhengqikj.top/gtpmrehrqf.html

[U119] JS：生产构建
来源：http://hz.yuanzhike.top/gtuzsztwqh.html

npx vite build
来源：http://hz.sufxvd.cn/gtvyqnhugr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ydzc1.top/gtlutoceqz.html

import.meta.env.VITE_API_URL
来源：http://hz.redwolf501.top/gtlnnqqzbb.html

================================================================================
来源：http://hz.ydjk.org.cn/gtotghipvk.html

统计汇总
来源：http://hz.wangshuangyany.cn/gtcoeknolb.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtymarptsu.html

按语言统计（条）：
来源：http://hz.hnxiangtu.top/gtrwozrlkg.html

Python ......... 252
来源：http://hz.meibo888.top/gtaugqhczf.html

PHP ............ 252
来源：http://hz.sysykeji.top/gtqyjklqgx.html

JavaScript ..... 252
来源：http://hz.yvedp.cn/gtkxigivtk.html

TypeScript ..... 212
来源：http://hz.tianlin.xyz/gtqnkpnarr.html

Java ........... 212
来源：http://hz.xinyue.icu/gtdeioqfnx.html

Go ............. 212
来源：http://hz.gotoacloud.top/gtkvcqlvvl.html

Ruby ........... 212
来源：http://hz.guannengcc.top/gtwwmhyjma.html

C# ............. 212
来源：http://hz.zdqjudy.top/gtknqgrxwp.html

C .............. 30
来源：http://hz.cheryme.top/gtrijjzumf.html

C++ ............ 30
来源：http://hz.yueranfly.top/gtjphtxyei.html

SQL ............ 90
来源：http://hz.yueranfly.top/gtiawprjek.html

Bash ........... 80
来源：http://hz.316326.xyz/gtlykbnarq.html

Kotlin ......... 15
来源：http://hz.jqgfzy.top/gtnisunsob.html

Swift .......... 15
来源：http://hz.daxiang520.top/gtbegsgwvi.html

Lua ............ 10
来源：http://hz.sxryk.cn/gtjtpjrtsz.html

Perl ........... 10
来源：http://hz.meibo888.top/gtbxusvlos.html

Scala .......... 10
来源：http://hz.wangdashe.top/gtzmzlrcxd.html

------------------------------------
来源：http://hz.sxryk.cn/gtpqfqsoge.html

合计 ........... 2106 条
来源：http://hz.jqgufenzy.top/gtwqnkcfoc.html

按章节统计：
来源：http://hz.quarkkingdee.top/gtqiibhwbd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.sweek.top/gtnyqqstor.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.52xcode.cn/gtnopsruqy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sufxvd.cn/gtpmdygjjs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtlrkqnprn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.aizwys.cn/gtphrvxfdm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.mhx1999.top/gtsrbwobah.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nwbrower.top/gtjopbwbih.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yangfankeji.com/gtewadxglh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtiygpshsr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hnqzz.top/gttekcjoeo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtmnepmjsy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtijkhqbrb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtxhbsaunv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.smart0.xyz/gtsfuetyqu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.cqqwz.cn/gtjsouqzll.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtdulgltvs.html

Q SQL 专题                              90
来源：http://hz.cucudq.cn/gtpngagows.html

R Bash 专题                             80
来源：http://hz.birdmap.top/gtautijhsn.html

S C / C++ 专题                          60
来源：http://hz.meibo888.top/gthpxkpefq.html

T 其他语言补充                          60
来源：http://hz.snrcjt.cn/gtbyopyjny.html

U 高频实用片段                         120
来源：http://hz.gaohongyu789.top/gtezoicbtt.html

------------------------------------
来源：http://hz.yongpay.top/gtaynbtizn.html

合计                                  2106 条
来源：http://hz.wangdashe.top/gtavxmcvnz.html

--------------------------------------------------------------------------------
来源：http://hz.nanxinkj.top/gtohegivpy.html

使用提醒
来源：http://hz.sufxvd.cn/gtmlkyazve.html

--------------------------------------------------------------------------------
来源：http://hz.zhongyouzk.top/gtppqmnkos.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ivvv.top/gtnszlutgu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.kuanghao11.cn/gtkontynvp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.fengsongda.top/gtrijvehyy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zdqjudy.top/gtamijdlsh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hfpthk.cn/gtwjvekolb.html

—— 文件结束 ——
来源：http://hz.zhoulong.xyz/gtogllypnc.html

================================================================================
来源：http://hz.ivvv.top/gttzherfgi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sxryk.cn/gtgpwhspax.html

Common Programming Examples Cheat Book
来源：http://hz.cdnleiting.top/gtbtmvvmak.html

================================================================================
来源：http://hz.316326.xyz/gtrvknfeqh.html

【收录内容】
来源：http://hz.yonumen.top/gtwdgcnpkl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cheryme.top/gtoapfirmw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xinyue.icu/gtqqcchwzg.html

SQL · Bash · C · C++
来源：http://hz.yj202588.top/gtsqjcsowj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.feifeiyinyue.top/gtpgnnphwp.html

【使用说明】
来源：http://hz.9152youxi.cn/gtwmbvnrlt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cheryme.top/gtjbhmojdp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.sufxvd.cn/gtmfsavyef.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.snrcjt.cn/gtvrgmwyva.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.pycfn.com/gtlmigzqsf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.sysykeji.top/gtgymfhhqa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tanke756.top/gtafpuarxu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.aibaodan.cn/gtbsjmmjey.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.mhx1999.top/gtmwgrscha.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yuxming.cn/gtyuvpkvwr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xingfuxueyuan.xyz/gtfcjnulfs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.shangyingyoupin.top/gthhmahdpq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jyoumei.cn/gtthunsiga.html

【文件统计】
来源：http://hz.shangyingyoupin.top/gtepvheben.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jiagoushi.top/gtlwhajkwa.html

--------------------------------------------------------------------------------
来源：http://hz.xylfe.cn/gttroxdysj.html

目  录
来源：http://hz.yj202588.top/gtpyejtidy.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gtcolnhffi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ydjk.org.cn/gtgbbbqamd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gtaqfptxws.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gzhubu.top/gtfiguqqjs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yangfankeji.com/gtrznnijls.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nwbrower.top/gtljkhrpak.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.shanyushiyangtech.top/gtyodisdxz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.chenjidiqi.icu/gtkchwltul.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.haohaochexian.top/gtqjjubkfq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtlmlfkzqb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.fzhhl.top/gtkrtzwdrw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jiagoushi.top/gtwwqgcbzg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtbzwuzqzi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtqiqobbvi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.aibaodan.cn/gtowafvhjq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.fzhhl.top/gtydolnvqr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtsrzgcoiz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jlsjyb.cn/gtzpcmexip.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.tian-w.cn/gtughoxeug.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhiwuduotai.top/gtsgywrgyq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.snrcjt.cn/gtjzvhnghs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.bjfxy.top/gtyuwrkxoy.html

================================================================================
来源：http://hz.jiagoushi.top/gtqslsyoab.html

A. 基础语法与类型
来源：http://hz.cheryme.top/gthnfoerjo.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtktqiazrn.html

[A01] Hello World
来源：http://hz.cheryme.top/gtvogcawak.html

Py:   print("Hello, World!")
来源：http://hz.jinqigfzy.top/gtzyjyjjmr.html

PHP:  echo "Hello, World!";
来源：http://hz.daxiang520.top/gtexrpfmjq.html

JS:   console.log("Hello, World!");
来源：http://hz.gotoacloud.top/gtsuvlwbbm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yueranfly.top/gtugyclhep.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhijiandao.cn/gtjsyfroxk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.haohaochexian.top/gtbsdhifqp.html

Ruby: puts "Hello, World!"
来源：http://hz.sxryk.cn/gtrujyfehm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.feifeiyinyue.top/gttnrthglb.html

[A02] 变量声明与赋值
来源：http://hz.wangdashe.top/gtqvqgjbgv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hfpthk.cn/gtphtfwyao.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shanyushiyangkeji.top/gtslkrless.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.daria6918.cn/gtufetdjni.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.chenjidiqi.icu/gtyamdtctq.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhongyouzk.top/gtbgstswrc.html

Go:   name := "Alex"; age := 20
来源：http://hz.xylfe.cn/gtnomsedjm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yuxming.cn/gtvfenfdno.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jianghu66.top/gtlrcivckj.html

[A03] 常量定义
来源：http://hz.zhongyouzk.top/gtkxxeruxb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xylfe.cn/gtgdlocyjx.html

PHP:  const PI = 3.14159;
来源：http://hz.zycfv.cn/gtvxdlfwgu.html

JS:   const PI = 3.14159;
来源：http://hz.cqqwz.cn/gtllgdnaxn.html

TS:   const PI: number = 3.14159;
来源：http://hz.ybcxt.top/gtjmijrvhe.html

Java: static final double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtcgmmyjrt.html

Go:   const PI = 3.14159
来源：http://hz.yvedp.cn/gtdlzcvveq.html

Ruby: PI = 3.14159
来源：http://hz.sweek.top/gttnkaiwym.html

C#:   const double PI = 3.14159;
来源：http://hz.iojbl.cn/gtayvraeaq.html

[A04] 判断变量类型
来源：http://hz.pengpengdd.cyou/gtsniutjqn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ywan-chungtsiang.top/gtjaioxqww.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yj20258888.top/gtiauumzqu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shzxlz.cn/gtdvwtwwxf.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gtmrduaunj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.feifeiyinyue.top/gtxksfcstc.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jinqigufen.top/gtczeigzja.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.svipenyu.cn/gteeeeyjeg.html

C#:   x.GetType().Name; x is int
来源：http://hz.shangyingyoupin.top/gtjcieiayh.html

[A05] 整数除法与取模
来源：http://hz.feifeiyinyue.top/gtzdfjlbug.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.bjfxy.top/gtkxrxnlzw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.snrcjt.cn/gtntsweacq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gogol.net.cn/gtebxkqsid.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shangyingyoupin.top/gtzwajoixb.html

Java: 7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gtixwubaiu.html

Go:   7 / 2; 7 % 2
来源：http://hz.cqqwz.cn/gtfvaccjrt.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jlsjyb.cn/gtlnxhjgqj.html

C#:   7 / 2; 7 % 2
来源：http://hz.jiagoushi.top/gtjqexxmfu.html

[A06] 字符串转数字
来源：http://hz.kuanghao11.cn/gtdgulegsp.html

Py:   int("42"); float("3.14")
来源：http://hz.gogol.net.cn/gtvgeesyfy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hammf.cn/gtfiinezuq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.svipenyu.cn/gtpwstfzwt.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.pengpengdd.cyou/gtxsvtemtu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.shuidangran.top/gtfiypegly.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jyoumei.cn/gttlrpujqc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.xylfe.cn/gtminzdrwr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.daria6918.cn/gtzkpzpftq.html

[A07] 数字转字符串
来源：http://hz.gaohongyu789.top/gtpksncksg.html

Py:   str(42)
来源：http://hz.zhijiandao.cn/gtfcunhrlk.html

PHP:  (string) 42; strval(42)
来源：http://hz.daxiang520.top/gtldvemvfe.html

JS:   String(42); (42).toString()
来源：http://hz.jinqigfzy.top/gtyobltmhb.html

TS:   String(42)
来源：http://hz.aibaodan.cn/gtarjnpgyg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hongshengwenyu.top/gtycgbpdjs.html

Go:   strconv.Itoa(42)
来源：http://hz.316326.xyz/gtorbkiome.html

Ruby: 42.to_s
来源：http://hz.nanxuanxn.top/gtguisgwjt.html

C#:   42.ToString()
来源：http://hz.yj20258.top/gtpqezgobl.html

[A08] 取整与四舍五入
来源：http://hz.xylfe.cn/gtmzvnmrhb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.dianchejie.cn/gtwkkegaqk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.hysaishi.cn/gtswwzkuat.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jinghuilouyu.cn/gtoueksgwp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.guowangkeji.top/gtrmzmhtkt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.cucudq.cn/gtdoysvuju.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.ehwqpu.com/gtllqhfpex.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.tian-w.cn/gtcimqxjks.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.haohaochexian.top/gtxierqcgp.html

[A09] 绝对值与最大最小值
来源：http://hz.andypj.xyz/gtxvrmuomm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.svipenyu.cn/gtvacnyvgq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zycfv.cn/gtwntylqrp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtkcbbamcd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jiagoushi.top/gtemlnhrnb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.52xcode.cn/gtvkylsfdd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.0kj1m.cn/gtymjolwrx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.xuanzx.com/gtpvcaqkzy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gthojnhgwu.html

[A10] 生成随机数
来源：http://hz.xylfe.cn/gtoycpjdst.html

Py:   import random; random.randint(1, 100)
来源：http://hz.quarkkingdee.top/gteucljjqq.html

PHP:  random_int(1, 100);
来源：http://hz.ehwqpu.com/gtcproiame.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jyoumei.cn/gtiznprsdl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.birdmap.top/gtayqqxxmr.html

Java: new Random().nextInt(100) + 1
来源：http://hz.cashguo.top/gtkbivvanr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.hongshengwenyu.top/gtjqoshxjb.html

Ruby: rand(1..100)
来源：http://hz.pycfn.com/gtoflvyshz.html

C#:   new Random().Next(1, 101)
来源：http://hz.yuanzhike.top/gtnnpnjohg.html

[A11] 条件表达式（三元）
来源：http://hz.nanxinkj.top/gtvfksuxqv.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.iojbl.cn/gtxymbtuwk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.daria6918.cn/gtfbimycyu.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.gaohongyu789.top/gttxjvgxyl.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.cucudq.cn/gtfkddkyfe.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ydjk.org.cn/gtfphnpryy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.yj20258.top/gtplrxrgji.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.xinyue.icu/gtxkknhxvi.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.xuanzx.com/gtvkfyfzcn.html

[A12] 字符串插值 / 格式化
来源：http://hz.jinqigfzy.top/gtagchovab.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.wangshuangyany.cn/gtltpscery.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.shuidangran.top/gtppmumowh.html

JS:   `Hello, ${name}!`
来源：http://hz.fengsongda.top/gtwzylnvkv.html

TS:   `Hello, ${name}!`
来源：http://hz.jinqigufen.top/gtvbnqmajj.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.xuetiantiany.cn/gtoahzzdrl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.gotoacloud.top/gtdqwumjfh.html

Ruby: "Hello, #{name}!"
来源：http://hz.bjfxy.top/gtgzghibnx.html

C#:   $"Hello, {name}!"
来源：http://hz.yj20258888.top/gteqecjxbj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yangfankeji.com/gtveqczhok.html

Py:   "第一行\n第二行"
来源：http://hz.sweek.top/gtjuhofccp.html

PHP:  "第一行\n第二行"
来源：http://hz.316326.xyz/gtqddfsucu.html

JS:   "第一行\n第二行"
来源：http://hz.zhixingplan.top/gtspanisiy.html

TS:   "第一行\n第二行"
来源：http://hz.yueranfly.top/gtgdzbswug.html

Java: "第一行\n第二行"
来源：http://hz.yj202588.top/gtadutgtxf.html

Go:   "第一行\n第二行"
来源：http://hz.ehwqpu.com/gtywohepbu.html

Ruby: "第一行\n第二行"
来源：http://hz.zhaomingkeji.xyz/gtodmitwrh.html

C#:   "第一行\n第二行"
来源：http://hz.yj20258.top/gtkeibzddy.html

[A14] 注释写法
来源：http://hz.9152youxi.cn/gtbxwaymxd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.bjfxy.top/gtxgzuyviw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.xylfe.cn/gtoydbwyol.html

JS:   // 单行；/* 多行 */
来源：http://hz.jinqigufen.top/gtshrjskfc.html

TS:   // 单行；/* 多行 */
来源：http://hz.tanke756.top/gtpdnyhnvw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.0kj1m.cn/gtipkakeur.html

Go:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangtech.top/gtveoitksf.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.redwolf501.top/gttjszfmam.html


<!-- 参考信息 -->