代发 wailian999

[U85] JS：可选链
来源：http://hz.shanyushiyangtech.top/gtrcbxvpez.html

a?.b?.c
来源：http://hz.fzhhl.top/gtryseshbf.html

[U86] JS：空值合并
来源：http://hz.jianghu66.top/gtrktrbvyb.html

a ?? b
来源：http://hz.zhongyouzk.top/gtxadlfqpj.html

[U87] JS：解构默认值
来源：http://hz.quarkkingdee.top/gtqghfkzwy.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shzxlz.cn/gtnrhtcatr.html

[U88] JS：对象展开合并
来源：http://hz.snrcjt.cn/gtspxybvnp.html

{ ...a, ...b }
来源：http://hz.svipenyu.cn/gtzrdyncmh.html

[U89] JS：数组去重
来源：http://hz.zycfv.cn/gtxjirrtpf.html

[...new Set(arr)]
来源：http://hz.zhengqikj.top/gtvunmkaps.html

[U90] JS：数字数组排序
来源：http://hz.nanxuanxn.top/gtpbfanxua.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xinyue.icu/gtjolmeyfz.html

[U91] JS：对象键值遍历
来源：http://hz.bjfxy.top/gtxyelgbui.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xingfuxueyuan.xyz/gtivjjvrsk.html

[U92] JS：深拷贝
来源：http://hz.jlsjyb.cn/gtqgerlmbj.html

structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtiswedeyg.html

[U93] JS：模板字符串
来源：http://hz.andypj.xyz/gtmpuuasul.html

`共 ${n} 条`
来源：http://hz.yj202588.top/gtnuojpefb.html

[U94] JS：箭头函数
来源：http://hz.ivvv.top/gtnnniihwp.html

const double = x => x * 2;
来源：http://hz.shuidangran.top/gtrroqdfzv.html

[U95] JS：Promise 包装
来源：http://hz.vqdsnc.cn/gthumqbhov.html

new Promise((resolve, reject) => {})
来源：http://hz.xuetiantiany.cn/gtvaobvjuu.html

[U96] JS：async/await 与异常
来源：http://hz.sufxvd.cn/gtmzddsrej.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtphxsydho.html

[U97] JS：并发请求
来源：http://hz.iojbl.cn/gtyfwgpqtd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtimcgkujh.html

[U98] JS：fetch 带 JSON
来源：http://hz.svipenyu.cn/gtxbahkgaz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.kuanghao11.cn/gtufxyhrvb.html

[U99] JS：事件监听
来源：http://hz.smart0.xyz/gtsryhqmen.html

el.addEventListener("click", e => {})
来源：http://hz.yanxiufei.cn/gttalxigqa.html

[U100] JS：DOM 查询
来源：http://hz.hysaishi.cn/gtpskotvsy.html

document.querySelector(".item")
来源：http://hz.zhongyouzk.top/gtfwuwfeiq.html

[U101] JS：classList 操作
来源：http://hz.shangyingyoupin.top/gtlarlbllz.html

el.classList.toggle("active")
来源：http://hz.yuxming.cn/gtcriuotwv.html

[U102] JS：本地存储
来源：http://hz.fengsongda.top/gtqhmschvy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.havefunace.top/gtyufwmkcx.html

[U103] JS：定时器
来源：http://hz.cheryme.top/gthceinuvh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aibaodan.cn/gtfbujqqst.html

[U104] JS：防抖
来源：http://hz.cqqwz.cn/gtvxrnxeaf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gthlbevpak.html

[U105] JS：节流
来源：http://hz.tanke756.top/gtfcbbcccc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zycfv.cn/gtnoebioiq.html

[U106] JS：日期格式化
来源：http://hz.cucudq.cn/gtdhvwoyos.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hnxiangtu.top/gtpawpooeh.html

[U107] JS：数字千分位
来源：http://hz.sysykeji.top/gteolambmd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tanke756.top/gtjglusyjf.html

[U108] JS：随机整数
来源：http://hz.yj20258.top/gtyjhfffyr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ydjk.org.cn/gtsbeqiisr.html

[U109] JS：数组分组
来源：http://hz.xylfe.cn/gtlmqjvzql.html

Object.groupBy(arr, x => x.type)
来源：http://hz.aizwys.cn/gtjvxujrog.html

[U110] JS：数组分块
来源：http://hz.jqgfzy.top/gtifewfzkw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.aizwys.cn/gtcfqaqskr.html

[U111] JS：对象转 Map
来源：http://hz.jinqigfzy.top/gtxttxvzzu.html

new Map(Object.entries(obj))
来源：http://hz.redwolf501.top/gtzxnwibnl.html

[U112] JS：字符串补位
来源：http://hz.dashuyun.cn/gtnjhufaad.html

"7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtjcffxmvl.html

[U113] JS：正则替换全部
来源：http://hz.sufxvd.cn/gtmlungotx.html

s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtpcuwuhzc.html

[U114] JS：JSON 深比较
来源：http://hz.hammf.cn/gtreqtqdjd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangtech.top/gtplkkejdc.html

[U115] JS：生成 UUID
来源：http://hz.yueranfly.top/gtvdtgfnrw.html

crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtgdqokhne.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.nanxinkj.top/gtnibdwqsm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.316326.xyz/gthrywqsaq.html

[U117] JS：单元测试
来源：http://hz.iojbl.cn/gtpsapndqk.html

npm i -D vitest;  npx vitest
来源：http://hz.gzhubu.top/gtwvuenqgw.html

[U118] JS：开发服务器
来源：http://hz.zycfv.cn/gtusnronub.html

npm i -D vite;  npx vite
来源：http://hz.snrcjt.cn/gtnggecmql.html

[U119] JS：生产构建
来源：http://hz.quarkkingdee.top/gtdbbydfgj.html

npx vite build
来源：http://hz.daxiang520.top/gtlxqxmsci.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinghuilouyu.cn/gtwcfvouly.html

import.meta.env.VITE_API_URL
来源：http://hz.chenjidiqi.icu/gtxbpeuwrs.html

================================================================================
来源：http://hz.aizwys.cn/gttyaojyqu.html

统计汇总
来源：http://hz.vqdsnc.cn/gthcdkabvk.html

================================================================================
来源：http://hz.hnqzz.top/gtbmirdqzc.html

按语言统计（条）：
来源：http://hz.sweek.top/gtxzmxdnkq.html

Python ......... 252
来源：http://hz.jqgfzy.top/gtgrygznwk.html

PHP ............ 252
来源：http://hz.cqqwz.cn/gtgecrfczt.html

JavaScript ..... 252
来源：http://hz.hfpthk.cn/gtogkhzzms.html

TypeScript ..... 212
来源：http://hz.ywan-chungtsiang.top/gtjgjfdaeq.html

Java ........... 212
来源：http://hz.52xcode.cn/gtcbttuezc.html

Go ............. 212
来源：http://hz.sweek.top/gtkdqngcww.html

Ruby ........... 212
来源：http://hz.redwolf501.top/gtdtlhufuc.html

C# ............. 212
来源：http://hz.zhixingplan.top/gtzbaxyrwu.html

C .............. 30
来源：http://hz.yonumen.top/gtvsmsuucy.html

C++ ............ 30
来源：http://hz.yanxiufei.cn/gtgmggntbm.html

SQL ............ 90
来源：http://hz.bjfxy.top/gtttxmfvcl.html

Bash ........... 80
来源：http://hz.shangyingyoupin.top/gtfzoiblhv.html

Kotlin ......... 15
来源：http://hz.ppjwa.cn/gtkbnytkie.html

Swift .......... 15
来源：http://hz.yj20258888.top/gtrbtqhqhd.html

Lua ............ 10
来源：http://hz.yueranfly.top/gtkwpynevi.html

Perl ........... 10
来源：http://hz.meibo888.top/gthjatmbcp.html

Scala .......... 10
来源：http://hz.daxiang520.top/gtahpdxrpp.html

------------------------------------
来源：http://hz.tianlin.xyz/gthcjukcsn.html

合计 ........... 2106 条
来源：http://hz.smart0.xyz/gtbxglxwvx.html

按章节统计：
来源：http://hz.316326.xyz/gtjgohdjme.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yvedp.cn/gtbxfnmjjh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yonumen.top/gtxspkaipn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenjidiqi.icu/gtoukfxvci.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.dashuyun.cn/gtsupsjurw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xingfuxueyuan.xyz/gtmqxjbvnn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yuanzhike.top/gtgynjvdzr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtpuuvvwrq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtqfebaunf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gttbsuvhhr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yueranfly.top/gtdpnszajz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtjrkatjot.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtagnvhkil.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtyvzritmw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jianghu66.top/gtdnyrouqj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.dianchejie.cn/gtjmowhkdq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtlaikmpdg.html

Q SQL 专题                              90
来源：http://hz.shuidangran.top/gtobchsufm.html

R Bash 专题                             80
来源：http://hz.yangfankeji.com/gtctvpcvez.html

S C / C++ 专题                          60
来源：http://hz.zhijiandao.cn/gtrpxmbmoi.html

T 其他语言补充                          60
来源：http://hz.yanxiufei.cn/gtxrhjdivh.html

U 高频实用片段                         120
来源：http://hz.andypj.xyz/gtoidmtxzu.html

------------------------------------
来源：http://hz.0kj1m.cn/gtiqsvbykn.html

合计                                  2106 条
来源：http://hz.cashguo.top/gtntfcejrk.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gtwjlsokma.html

使用提醒
来源：http://hz.cashguo.top/gtbelecgkc.html

--------------------------------------------------------------------------------
来源：http://hz.sysykeji.top/gteicypcqy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.quarkkingdee.top/gtqhidhqgx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yongpay.top/gtmhnahnmt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj20258888.top/gtmvpaltvc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.nwbrower.top/gtonagphuz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.wangdashe.top/gtszdpuwyh.html

—— 文件结束 ——
来源：http://hz.daria6918.cn/gtawfysxye.html

================================================================================
来源：http://hz.bjfxy.top/gtkbofizcv.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.wangshuangyany.cn/gtqmzjapqc.html

Common Programming Examples Cheat Book
来源：http://hz.chenlongwang.top/gtjptpgduu.html

================================================================================
来源：http://hz.haohaochexian.top/gticxjabdx.html

【收录内容】
来源：http://hz.pengpengdd.cyou/gtghmbeqmv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gogol.net.cn/gtvafhebpb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jinqigfzy.top/gthjszfcup.html

SQL · Bash · C · C++
来源：http://hz.zhengqikj.top/gtjvuupgaj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.nanxuanxn.top/gtdsrrnrxj.html

【使用说明】
来源：http://hz.kuanghao11.cn/gtzjguttll.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.quarkkingdee.top/gtftgnrhix.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ppjwa.cn/gtcvxkcgys.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhaomingkeji.xyz/gttncjhhoe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ydzc1.top/gtaccawryq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhongyouzk.top/gtvdbagioo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zycfv.cn/gtxkwyeqgw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yvedp.cn/gttzzuzfdk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.chenlongwang.top/gtukqgseya.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhiwuduotai.top/gtwsbqkewp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ybcxt.top/gtwfiwwikv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hnqzz.top/gtqetdyqge.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xylfe.cn/gtzzfiyclz.html

【文件统计】
来源：http://hz.hywenlv.cn/gtvuiygyth.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cqqwz.cn/gttvhqjqch.html

--------------------------------------------------------------------------------
来源：http://hz.meibo888.top/gtuyhtiyrs.html

目  录
来源：http://hz.zycfv.cn/gtvetjmpzs.html

--------------------------------------------------------------------------------
来源：http://hz.jqgufenzy.top/gtkdhitbfz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.bjfxy.top/gtxywdxwbi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ivvv.top/gtwzzenont.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jinghuilouyu.cn/gtxtmvbtcy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sysykeji.top/gtrxgnezpf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shanyushiyangtech.top/gtngemfniv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.shanyushiyangkeji.top/gtpkhvvhbq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.chenlongwang.top/gthruqhswo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.birdmap.top/gtigukyepa.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtsiyhyyuh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.dianchejie.cn/gtleznewyp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.nanxuanxn.top/gtrofkgpee.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.sysykeji.top/gtqcydnirw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtjzzvbzeo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hysaishi.cn/gtlwmtkgeb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jiagoushi.top/gtkxyvazwq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gtaaentswx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yuanzhike.top/gteofzekiy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.haohaochexian.top/gtcyjaegcw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinyuanbaomall.cn/gtkbubshvl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daria6918.cn/gtvpzneggv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigufen.top/gthmezwaut.html

================================================================================
来源：http://hz.zdqjudy.top/gtlfrvgrem.html

A. 基础语法与类型
来源：http://hz.jlsjyb.cn/gtplrueyfv.html

================================================================================
来源：http://hz.gaohongyu789.top/gtxefwzlpy.html

[A01] Hello World
来源：http://hz.ywan-chungtsiang.top/gtoqljitep.html

Py:   print("Hello, World!")
来源：http://hz.cashguo.top/gtkgpfchwt.html

PHP:  echo "Hello, World!";
来源：http://hz.guowangkeji.top/gtmdsckpho.html

JS:   console.log("Hello, World!");
来源：http://hz.hnqzz.top/gtfqfksjyr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yanxiufei.cn/gtptorulvt.html

Java: System.out.println("Hello, World!");
来源：http://hz.bjfxy.top/gtcftejezy.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinghuilouyu.cn/gtnqiymhud.html

Ruby: puts "Hello, World!"
来源：http://hz.xylfe.cn/gtdksnvkxe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.feifeiyinyue.top/gtoucxeqbj.html

[A02] 变量声明与赋值
来源：http://hz.gaohongyu789.top/gtgomylhgl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shzxlz.cn/gtlbvkqxls.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.pengpengdd.cyou/gtztxjbsrd.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.kuanghao11.cn/gtfjezgdcc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hnqzz.top/gtvasphwwl.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hnxiangtu.top/gtbelsgmuc.html

Go:   name := "Alex"; age := 20
来源：http://hz.xuanzx.com/gtnctdddvn.html

Ruby: name = "Alex"; age = 20
来源：http://hz.pengpengdd.cyou/gtynxeqhsa.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yonumen.top/gtbbqupack.html

[A03] 常量定义
来源：http://hz.yangfankeji.com/gtoibabnpn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yuxming.cn/gtedkesofx.html

PHP:  const PI = 3.14159;
来源：http://hz.chenlongwang.top/gtixcbeoud.html

JS:   const PI = 3.14159;
来源：http://hz.yonumen.top/gttiawcrbt.html

TS:   const PI: number = 3.14159;
来源：http://hz.9152youxi.cn/gtztcaqlrr.html

Java: static final double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtuhtpzlmv.html

Go:   const PI = 3.14159
来源：http://hz.ydjk.org.cn/gtrjarfchp.html

Ruby: PI = 3.14159
来源：http://hz.pycfn.com/gtxllanlxu.html

C#:   const double PI = 3.14159;
来源：http://hz.smart0.xyz/gtrchtckgq.html

[A04] 判断变量类型
来源：http://hz.fengsongda.top/gtavpndfje.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.wangdashe.top/gtyccxiczd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhixingplan.top/gtqkkkjajg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yongpay.top/gtsduehjfm.html

TS:   typeof x; x instanceof Date
来源：http://hz.shzxlz.cn/gtrpeayzcc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hnqzz.top/gtblwqezeb.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.52xcode.cn/gtdeiytitg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shzxlz.cn/gtpjcuxklc.html

C#:   x.GetType().Name; x is int
来源：http://hz.svipenyu.cn/gtpzbpdjpe.html

[A05] 整数除法与取模
来源：http://hz.jianghu66.top/gtqpemoefv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.aibaodan.cn/gtmxusshpi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hnxiangtu.top/gtelpxzrxv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cashguo.top/gtduoucsaq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.birdmap.top/gtvxnnzqbs.html

Java: 7 / 2; 7 % 2
来源：http://hz.yj20258888.top/gtsrwkodag.html

Go:   7 / 2; 7 % 2
来源：http://hz.yj202588.top/gtkavotpdj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ppjwa.cn/gtfybfwpss.html

C#:   7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gtbpttksta.html

[A06] 字符串转数字
来源：http://hz.chenzaomai.com/gtbwsdwbna.html

Py:   int("42"); float("3.14")
来源：http://hz.hammf.cn/gtjrbairws.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.shanyushiyangtech.top/gtrlautcnt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cucudq.cn/gtkuhnzqgi.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.0kj1m.cn/gtmhyoojsc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.quarkkingdee.top/gtlqvqqtfl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ivvv.top/gtdupwisjh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.hammf.cn/gtxwlgwiee.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xinyue.icu/gtdzobifpg.html

[A07] 数字转字符串
来源：http://hz.jinqigfzy.top/gtwcmgvqvb.html

Py:   str(42)
来源：http://hz.yj20258.top/gtntoxfimo.html

PHP:  (string) 42; strval(42)
来源：http://hz.xylfe.cn/gtgrwbzcry.html

JS:   String(42); (42).toString()
来源：http://hz.cashguo.top/gttledzkpg.html

TS:   String(42)
来源：http://hz.smart0.xyz/gttkrvbrcz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.guannengcc.top/gthhijwyyy.html

Go:   strconv.Itoa(42)
来源：http://hz.cdnleiting.top/gtmawooaxz.html

Ruby: 42.to_s
来源：http://hz.9152youxi.cn/gthwymptmx.html

C#:   42.ToString()
来源：http://hz.feifeiyinyue.top/gtyvnzckxt.html

[A08] 取整与四舍五入
来源：http://hz.yj20258.top/gtewkbguud.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.bjfxy.top/gtjvztskib.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yj202588.top/gtbwxjvbgf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.cucudq.cn/gtejxubjop.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.hysaishi.cn/gtdccndwde.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.mhx1999.top/gtxgueqxkf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.svipenyu.cn/gtqllrlbas.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jinqigfzy.top/gtkupyqzks.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.xylfe.cn/gthbfdjxdr.html

[A09] 绝对值与最大最小值
来源：http://hz.aibaodan.cn/gtoetdaxvx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.mhx1999.top/gtvbvcnufb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtoeeqznmv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hfpthk.cn/gtgczjcfwa.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.chenjidiqi.icu/gtdfovwejx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtmihmqrco.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jiagoushi.top/gtjjcrfgcm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.zhongyouzk.top/gtjibohlnd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.gogol.net.cn/gtrvnzysex.html

[A10] 生成随机数
来源：http://hz.yuxming.cn/gtijmwlhgj.html

Py:   import random; random.randint(1, 100)
来源：http://hz.kuanghao11.cn/gtqlvhfjng.html

PHP:  random_int(1, 100);
来源：http://hz.wangdashe.top/gtfdehxadx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.mhx1999.top/gtkrrqggvt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.fzhhl.top/gtxykibfsk.html

Java: new Random().nextInt(100) + 1
来源：http://hz.smart0.xyz/gteedybort.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.hfpthk.cn/gtfoaylvsw.html

Ruby: rand(1..100)
来源：http://hz.xziqi.cn/gtrxdducln.html

C#:   new Random().Next(1, 101)
来源：http://hz.sysykeji.top/gtojgeqnkm.html

[A11] 条件表达式（三元）
来源：http://hz.hnxiangtu.top/gtbkmvknry.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.xziqi.cn/gtquzybffw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.xinyue.icu/gtoldcwgmh.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.316326.xyz/gtibhhpgat.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.ywan-chungtsiang.top/gtxxsglgsh.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.bjfxy.top/gtzifoinyp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.sysykeji.top/gtbjdsqkka.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.tianlin.xyz/gtzvsuzpvt.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.shuidangran.top/gtimttwgfp.html

[A12] 字符串插值 / 格式化
来源：http://hz.redwolf501.top/gtwmavdqkc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.shangyingyoupin.top/gtncazqjyd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.xziqi.cn/gtzdzkpufr.html

JS:   `Hello, ${name}!`
来源：http://hz.sufxvd.cn/gtodxcypvz.html

TS:   `Hello, ${name}!`
来源：http://hz.cheryme.top/gtabuxanov.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.52xcode.cn/gttcwfgtsa.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.hywenlv.cn/gtytgqeoum.html

Ruby: "Hello, #{name}!"
来源：http://hz.sxryk.cn/gttzaluylf.html

C#:   $"Hello, {name}!"
来源：http://hz.snrcjt.cn/gtvhnpiqmm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jiagoushi.top/gtyoecamzn.html

Py:   "第一行\n第二行"
来源：http://hz.aizwys.cn/gtuzovrkmm.html

PHP:  "第一行\n第二行"
来源：http://hz.yuanzhike.top/gtoyagjeue.html

JS:   "第一行\n第二行"
来源：http://hz.shanyushiyangtech.top/gtykeffxfo.html

TS:   "第一行\n第二行"
来源：http://hz.yueranfly.top/gtejfzcwgj.html

Java: "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtsqmtilvb.html

Go:   "第一行\n第二行"
来源：http://hz.c1oappe.top/gtpkeaiwcd.html

Ruby: "第一行\n第二行"
来源：http://hz.hywenlv.cn/gtsssrlsiu.html

C#:   "第一行\n第二行"
来源：http://hz.zycfv.cn/gtpwcbrfzi.html

[A14] 注释写法
来源：http://hz.birdmap.top/gttxcuahxz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.havefunace.top/gtvambzkpt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.52xcode.cn/gtvwhktcbe.html

JS:   // 单行；/* 多行 */
来源：http://hz.feifeiyinyue.top/gtnorlxxuk.html


<!-- 参考信息 -->