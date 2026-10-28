代发 wailian999

[U91] JS：对象键值遍历
来源：http://hz.shanyushiyangkeji.top/gtaywcuoxq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ywan-chungtsiang.top/gtksjsxiwv.html

[U92] JS：深拷贝
来源：http://hz.hfpthk.cn/gtiljuivlj.html

structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gtxetccbaj.html

[U93] JS：模板字符串
来源：http://hz.vqdsnc.cn/gtngrxkrfj.html

`共 ${n} 条`
来源：http://hz.nanxuanxn.top/gtpnfhmwwu.html

[U94] JS：箭头函数
来源：http://hz.nanxuanxn.top/gtddptfung.html

const double = x => x * 2;
来源：http://hz.jinqigfzy.top/gtigxdmulf.html

[U95] JS：Promise 包装
来源：http://hz.hnxiangtu.top/gtbkifhwog.html

new Promise((resolve, reject) => {})
来源：http://hz.jlsjyb.cn/gtzcofotsz.html

[U96] JS：async/await 与异常
来源：http://hz.xinyue.icu/gtahapiadw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtmqczfiag.html

[U97] JS：并发请求
来源：http://hz.nwbrower.top/gtmzdtvsub.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtqojexhrx.html

[U98] JS：fetch 带 JSON
来源：http://hz.wangshuangyany.cn/gtkyetlsgb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shanyushiyangtech.top/gtcxunjgqs.html

[U99] JS：事件监听
来源：http://hz.hongshengwenyu.top/gtxuotjdml.html

el.addEventListener("click", e => {})
来源：http://hz.ivvv.top/gtfthhuwou.html

[U100] JS：DOM 查询
来源：http://hz.bjfxy.top/gtyzpwvimj.html

document.querySelector(".item")
来源：http://hz.xuanzx.com/gtlrgebevn.html

[U101] JS：classList 操作
来源：http://hz.aizwys.cn/gtjmbxppxt.html

el.classList.toggle("active")
来源：http://hz.shanyushiyangtech.top/gtoadlfidl.html

[U102] JS：本地存储
来源：http://hz.svipenyu.cn/gtbixfrsbz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.dianchejie.cn/gtanxdfmge.html

[U103] JS：定时器
来源：http://hz.zhiwuduotai.top/gtemvmhrgi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hammf.cn/gtvjaztzsz.html

[U104] JS：防抖
来源：http://hz.cheryme.top/gtvphsyhlj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtcxkppxlf.html

[U105] JS：节流
来源：http://hz.hysaishi.cn/gtqrpxuerw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhixingplan.top/gtbhimyuiq.html

[U106] JS：日期格式化
来源：http://hz.yj20258.top/gtzujplnla.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tian-w.cn/gttmccnjtj.html

[U107] JS：数字千分位
来源：http://hz.zhoulong.xyz/gtwwtcfnzc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.sxryk.cn/gtpizyljvm.html

[U108] JS：随机整数
来源：http://hz.ybcxt.top/gtmeeictve.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hammf.cn/gtbqexqvna.html

[U109] JS：数组分组
来源：http://hz.nwbrower.top/gtjpgcxkyt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.smart0.xyz/gtqqwtxyxd.html

[U110] JS：数组分块
来源：http://hz.0kj1m.cn/gtdehbbigo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ydjk.org.cn/gtfvqqlhem.html

[U111] JS：对象转 Map
来源：http://hz.aibaodan.cn/gtsnmvpjiz.html

new Map(Object.entries(obj))
来源：http://hz.nwbrower.top/gtlwbjmujv.html

[U112] JS：字符串补位
来源：http://hz.dianchejie.cn/gtdlpuicyb.html

"7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtyfdojfsl.html

[U113] JS：正则替换全部
来源：http://hz.chenlongwang.top/gtbwovoaon.html

s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtzblzpagd.html

[U114] JS：JSON 深比较
来源：http://hz.ppjwa.cn/gtreycxbmp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gogol.net.cn/gtvxdjbstd.html

[U115] JS：生成 UUID
来源：http://hz.cdnleiting.top/gthunmwetj.html

crypto.randomUUID()
来源：http://hz.sweek.top/gtafkpthvf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ppjwa.cn/gtnfsncymu.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xziqi.cn/gtbiyjpnrn.html

[U117] JS：单元测试
来源：http://hz.sysykeji.top/gtdlbaqxpp.html

npm i -D vitest;  npx vitest
来源：http://hz.xingfuxueyuan.xyz/gtkbiqsqys.html

[U118] JS：开发服务器
来源：http://hz.wangshuangyany.cn/gtxfhyadyt.html

npm i -D vite;  npx vite
来源：http://hz.52xcode.cn/gtlcrmkvdi.html

[U119] JS：生产构建
来源：http://hz.zhiwuduotai.top/gtprcpukam.html

npx vite build
来源：http://hz.redwolf501.top/gtkkothpsb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xziqi.cn/gtyybvzbmt.html

import.meta.env.VITE_API_URL
来源：http://hz.cdnleiting.top/gtyuqkgkef.html

================================================================================
来源：http://hz.yj20258.top/gtinvakrml.html

统计汇总
来源：http://hz.ydzc1.top/gttmiqrrfb.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtgrqiupvj.html

按语言统计（条）：
来源：http://hz.vqdsnc.cn/gtkfczqfsn.html

Python ......... 252
来源：http://hz.daxiang520.top/gtcethrook.html

PHP ............ 252
来源：http://hz.9152youxi.cn/gtrkfdonzy.html

JavaScript ..... 252
来源：http://hz.fengsongda.top/gtpzmoanjg.html

TypeScript ..... 212
来源：http://hz.jinghuilouyu.cn/gtodfcukni.html

Java ........... 212
来源：http://hz.gotoacloud.top/gtrbgkauor.html

Go ............. 212
来源：http://hz.cdnleiting.top/gtvodwzzpx.html

Ruby ........... 212
来源：http://hz.andypj.xyz/gtdjvqjjaz.html

C# ............. 212
来源：http://hz.hywenlv.cn/gtczwjxgsi.html

C .............. 30
来源：http://hz.sysykeji.top/gtywyyhebu.html

C++ ............ 30
来源：http://hz.zhoulong.xyz/gtmiwlbwmf.html

SQL ............ 90
来源：http://hz.dianchejie.cn/gtzwsxiutd.html

Bash ........... 80
来源：http://hz.ivvv.top/gtjbtjrswm.html

Kotlin ......... 15
来源：http://hz.cdnleiting.top/gttuncobqi.html

Swift .......... 15
来源：http://hz.hammf.cn/gtvntkxbzd.html

Lua ............ 10
来源：http://hz.jinqigfzy.top/gtrjwtlnbd.html

Perl ........... 10
来源：http://hz.tanke756.top/gthzctcard.html

Scala .......... 10
来源：http://hz.wangshuangyany.cn/gtrglytows.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtvywwzrul.html

合计 ........... 2106 条
来源：http://hz.xylfe.cn/gtdlxdtcpq.html

按章节统计：
来源：http://hz.yuxming.cn/gtpzydxrzy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinghuilouyu.cn/gtizglncjc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gtojphgxit.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenjidiqi.icu/gtshmkexfr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pycfn.com/gtdhwbnbgm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.bjfxy.top/gtxxlorupa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ybcxt.top/gtrupgtpes.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinyuanbaomall.cn/gtvpoenjjv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.c1oappe.top/gtfstvupqz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtqkphsqyi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.feifeiyinyue.top/gtopjlrkjb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtqhxtwunv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtfpvkdtay.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtqbgbpzjc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cdnleiting.top/gtzicelywh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hnxiangtu.top/gtwrpmrsdm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtbdreevli.html

Q SQL 专题                              90
来源：http://hz.zycfv.cn/gtfhmcjbwp.html

R Bash 专题                             80
来源：http://hz.yj202588.top/gtasvdkkhd.html

S C / C++ 专题                          60
来源：http://hz.aibaodan.cn/gtbuezqwxp.html

T 其他语言补充                          60
来源：http://hz.fengsongda.top/gtrfsgbrpe.html

U 高频实用片段                         120
来源：http://hz.ehwqpu.com/gtbfnsirrl.html

------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtasntrxmb.html

合计                                  2106 条
来源：http://hz.yj20258888.top/gtjzfscgzq.html

--------------------------------------------------------------------------------
来源：http://hz.ivvv.top/gtuwtdiyji.html

使用提醒
来源：http://hz.jlsjyb.cn/gtxlheljzm.html

--------------------------------------------------------------------------------
来源：http://hz.hnqzz.top/gtbglskwph.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sufxvd.cn/gtkrkbiedn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hywenlv.cn/gtddozwodk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ydjk.org.cn/gtfrwseuyf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.birdmap.top/gtgzhquntr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhoulong.xyz/gtbirgqhdk.html

—— 文件结束 ——
来源：http://hz.gogol.net.cn/gtqhpbgpcd.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtdxhkxvjh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj20258.top/gtibjrutjd.html

Common Programming Examples Cheat Book
来源：http://hz.jianghu66.top/gterrqodok.html

================================================================================
来源：http://hz.yangfankeji.com/gtktriidts.html

【收录内容】
来源：http://hz.yongpay.top/gtiodzecvm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.chenzaomai.com/gtrezdhqcs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ppjwa.cn/gtuwrvlnig.html

SQL · Bash · C · C++
来源：http://hz.zhongyouzk.top/gtnqrsilgr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yvedp.cn/gtpwnryawp.html

【使用说明】
来源：http://hz.yuxming.cn/gtbpoilsxc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.sysykeji.top/gtnnmcwfgh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.chenlongwang.top/gtvyiutzzl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yvedp.cn/gtoxpifuxs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jinqigufen.top/gtlxgalvdu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.guowangkeji.top/gtzajycjgn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhijiandao.cn/gtbntluuaa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.birdmap.top/gtismdpalk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jiagoushi.top/gtxqmrqbri.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jlsjyb.cn/gtbwonljbb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.hammf.cn/gtacxeddzb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hongshengwenyu.top/gtmpxvkaft.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.snrcjt.cn/gtujwtljxl.html

【文件统计】
来源：http://hz.zhixingplan.top/gtfdxqijrt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ppjwa.cn/gthuajlcfw.html

--------------------------------------------------------------------------------
来源：http://hz.zhiwuduotai.top/gtbqidtams.html

目  录
来源：http://hz.yvedp.cn/gtkqspfmmm.html

--------------------------------------------------------------------------------
来源：http://hz.zhijiandao.cn/gthhuzxvhq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zdqjudy.top/gtxcbbtvvl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.meibo888.top/gtlndxamvn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yanxiufei.cn/gtvpftewap.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.wangshuangyany.cn/gtpbodxalh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhengqikj.top/gtdzqheisb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yuanzhike.top/gttjtxwzca.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shangyingyoupin.top/gtfbhblmrl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.meibo888.top/gtafciwdxr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtuvzzytcl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ehwqpu.com/gtmshsbgbw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtjtuifkur.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jinghuilouyu.cn/gtgvhvxdvo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtswhyralf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.gotoacloud.top/gtoemzsker.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yonumen.top/gtrmdnnhlv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtvhdegefe.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.fzhhl.top/gtkswodbfn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.iojbl.cn/gtporwutkh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cqqwz.cn/gtxvxvgzyz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sysykeji.top/gtgnrmimwx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yvedp.cn/gtdsmxybwt.html

================================================================================
来源：http://hz.mhx1999.top/gtsyapfepu.html

A. 基础语法与类型
来源：http://hz.hywenlv.cn/gtomiofelk.html

================================================================================
来源：http://hz.jianghu66.top/gtwqjgdplu.html

[A01] Hello World
来源：http://hz.yonumen.top/gtzutktgyj.html

Py:   print("Hello, World!")
来源：http://hz.shzxlz.cn/gthmkinnsf.html

PHP:  echo "Hello, World!";
来源：http://hz.xuanzx.com/gtfwyxhuxg.html

JS:   console.log("Hello, World!");
来源：http://hz.xinyue.icu/gtrehsxghi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.dashuyun.cn/gtcdwviawq.html

Java: System.out.println("Hello, World!");
来源：http://hz.bjfxy.top/gttrpnxptg.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.chenjidiqi.icu/gtrxnlxejn.html

Ruby: puts "Hello, World!"
来源：http://hz.svipenyu.cn/gtemijpwwz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhoulong.xyz/gtaqnfrooc.html

[A02] 变量声明与赋值
来源：http://hz.tanke756.top/gtqckxrprm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.pengpengdd.cyou/gtfyinxvkp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zycfv.cn/gtnwbzaxwn.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ivvv.top/gtdzpuwsbg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hysaishi.cn/gtojaaxiyb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.cdnleiting.top/gtfxaqhmwf.html

Go:   name := "Alex"; age := 20
来源：http://hz.xinyue.icu/gtlupymvtm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.52xcode.cn/gtpshcpamw.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gogol.net.cn/gtmjabqeic.html

[A03] 常量定义
来源：http://hz.xuetiantiany.cn/gtgrnnhkwz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.aibaodan.cn/gtyapetkxl.html

PHP:  const PI = 3.14159;
来源：http://hz.tian-w.cn/gttoqzfnwo.html

JS:   const PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtrnomvquo.html

TS:   const PI: number = 3.14159;
来源：http://hz.sysykeji.top/gthvmtgmec.html

Java: static final double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtstwbzmze.html

Go:   const PI = 3.14159
来源：http://hz.sxryk.cn/gtseianclk.html

Ruby: PI = 3.14159
来源：http://hz.jlsjyb.cn/gtaumfganz.html

C#:   const double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtiimsbpuj.html

[A04] 判断变量类型
来源：http://hz.ywan-chungtsiang.top/gtwqmsowdd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.sxryk.cn/gtjkneybba.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jinqigfzy.top/gtatjbpikg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ehwqpu.com/gtyqdbcskr.html

TS:   typeof x; x instanceof Date
来源：http://hz.fzhhl.top/gtfdvyznyz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yangfankeji.com/gtipfwusxp.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.smart0.xyz/gtyvyzzpxu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.cqqwz.cn/gtllloncfw.html

C#:   x.GetType().Name; x is int
来源：http://hz.xylfe.cn/gtemngnktn.html

[A05] 整数除法与取模
来源：http://hz.jianghu66.top/gttopywuis.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hongshengwenyu.top/gtyhyicyye.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jqgfzy.top/gtyguaatxa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.fzhhl.top/gtpbqlteeb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.feifeiyinyue.top/gtslpoauyu.html

Java: 7 / 2; 7 % 2
来源：http://hz.zhengqikj.top/gtlucueeae.html

Go:   7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtownsabww.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.snrcjt.cn/gtxcplsapp.html

C#:   7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtltlijady.html

[A06] 字符串转数字
来源：http://hz.jiagoushi.top/gtbbtrlehe.html

Py:   int("42"); float("3.14")
来源：http://hz.guowangkeji.top/gtvvpjshxl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.gzhubu.top/gteulsxlvw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jianghu66.top/gtabyxkmxm.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.52xcode.cn/gtdnideluq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.dianchejie.cn/gtxrudkfud.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.havefunace.top/gtcqhlnnhe.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yongpay.top/gtlcszfksq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.pycfn.com/gttwtxstxy.html

[A07] 数字转字符串
来源：http://hz.aizwys.cn/gtlngfgsjs.html

Py:   str(42)
来源：http://hz.wangdashe.top/gtttagpuaw.html

PHP:  (string) 42; strval(42)
来源：http://hz.ydjk.org.cn/gtcmkzhotu.html

JS:   String(42); (42).toString()
来源：http://hz.mhx1999.top/gtjrigwzgd.html

TS:   String(42)
来源：http://hz.xylfe.cn/gteajnfgms.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.nanxinkj.top/gtgcklmjxt.html

Go:   strconv.Itoa(42)
来源：http://hz.ivvv.top/gtioqqimvv.html

Ruby: 42.to_s
来源：http://hz.aizwys.cn/gtscwbgoiq.html

C#:   42.ToString()
来源：http://hz.sweek.top/gtfmjtfryo.html

[A08] 取整与四舍五入
来源：http://hz.iojbl.cn/gtfsqzoxpn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.chenjidiqi.icu/gteeswpusg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.ybcxt.top/gtfmhtkabl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zycfv.cn/gtjmlyewsg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zhengqikj.top/gtkpzrshto.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yonumen.top/gtmdszrwcf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zycfv.cn/gtbxyclovz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yanxiufei.cn/gtwiwrkitx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hfpthk.cn/gtswuqponk.html

[A09] 绝对值与最大最小值
来源：http://hz.shanyushiyangtech.top/gtbghenuay.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.smart0.xyz/gtlquggftr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.wangdashe.top/gtlyfnqlhn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hongshengwenyu.top/gtuiffdeyl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yanxiufei.cn/gtstgtndhd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.nanxuanxn.top/gtxpdynqwo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.c1oappe.top/gtchsdftbu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.vqdsnc.cn/gtxaewevbx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hnqzz.top/gtjgxpksjx.html

[A10] 生成随机数
来源：http://hz.yj20258.top/gtaknzwpep.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zhiwuduotai.top/gtrnatgoyn.html

PHP:  random_int(1, 100);
来源：http://hz.ydzc1.top/gtbdqwwhpg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yongpay.top/gtncarkwsc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.dianchejie.cn/gtsfnjupkz.html

Java: new Random().nextInt(100) + 1
来源：http://hz.gogol.net.cn/gtjvphpfbl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.sysykeji.top/gtlpqqerul.html

Ruby: rand(1..100)
来源：http://hz.cqqwz.cn/gtjhmeebik.html

C#:   new Random().Next(1, 101)
来源：http://hz.9152youxi.cn/gtmfpzihrw.html

[A11] 条件表达式（三元）
来源：http://hz.haohaochexian.top/gtmsjurwns.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.shzxlz.cn/gtasrbufvk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yanxiufei.cn/gtllpkawoa.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.sysykeji.top/gtccwrfmwy.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.cashguo.top/gtaqyazdcf.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ppjwa.cn/gtppbzwosn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.gzhubu.top/gtoozywibd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.yj20258888.top/gtqeirgmuw.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.cashguo.top/gtkmtwbung.html

[A12] 字符串插值 / 格式化
来源：http://hz.gaohongyu789.top/gtqzudqtup.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.shangyingyoupin.top/gtkedfmhcl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.iojbl.cn/gthrbbvwns.html

JS:   `Hello, ${name}!`
来源：http://hz.birdmap.top/gtoqmpvtsm.html

TS:   `Hello, ${name}!`
来源：http://hz.jqgfzy.top/gtjlqwlpbs.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.xingfuxueyuan.xyz/gtrltwvpqe.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.daxiang520.top/gtnubgoirz.html

Ruby: "Hello, #{name}!"
来源：http://hz.zhixingplan.top/gtldmkqguo.html

C#:   $"Hello, {name}!"
来源：http://hz.zdqjudy.top/gtlecnecty.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yanxiufei.cn/gtemseoeav.html

Py:   "第一行\n第二行"
来源：http://hz.xuetiantiany.cn/gtdjqoyfvq.html

PHP:  "第一行\n第二行"
来源：http://hz.tian-w.cn/gtnotoagsy.html

JS:   "第一行\n第二行"
来源：http://hz.smart0.xyz/gtkhsprgoc.html

TS:   "第一行\n第二行"
来源：http://hz.pycfn.com/gtspzwjtet.html

Java: "第一行\n第二行"
来源：http://hz.gaohongyu789.top/gthetdfyfq.html

Go:   "第一行\n第二行"
来源：http://hz.haohaochexian.top/gtwqcizkfi.html

Ruby: "第一行\n第二行"
来源：http://hz.52xcode.cn/gtqdmufmye.html

C#:   "第一行\n第二行"
来源：http://hz.daxiang520.top/gtajsxejdv.html

[A14] 注释写法
来源：http://hz.jqgufenzy.top/gttfzxxbch.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.cashguo.top/gteniaemuc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.tian-w.cn/gtfcnjpmwd.html

JS:   // 单行；/* 多行 */
来源：http://hz.havefunace.top/gtslptgdhs.html

TS:   // 单行；/* 多行 */
来源：http://hz.zhongyouzk.top/gtlpryfzau.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.dianchejie.cn/gtdrwkvcjl.html

Go:   // 单行；/* 多行 */
来源：http://hz.aizwys.cn/gtqjzbovbd.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.meibo888.top/gtmamzgnew.html

C#:   // 单行；/* 多行 */
来源：http://hz.yj202588.top/gtxcudbcce.html

[A15] 空值判断与默认值
来源：http://hz.snrcjt.cn/gtvemlfghf.html

Py:   value = data or "默认值"
来源：http://hz.nanxinkj.top/gtcsohipqq.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.nwbrower.top/gtiwjqhqhh.html

JS:   const value = data ?? "默认值";
来源：http://hz.hnqzz.top/gtqfsflzqa.html

TS:   const value = data ?? "默认值";
来源：http://hz.zhijiandao.cn/gtdlxqdhwq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.pengpengdd.cyou/gthxebeivp.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.jinyuanbaomall.cn/gtnehhqggc.html


<!-- 参考信息 -->