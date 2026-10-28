代发 wailian999

[U79] PHP：静态分析
来源：http://hz.hysaishi.cn/gtzfdsvbuj.html

composer require --dev phpstan/phpstan
来源：http://hz.shzxlz.cn/gtuxkrekzt.html

[U80] PHP：代码规范修复
来源：http://hz.shangyingyoupin.top/gtylpvauxj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhiwuduotai.top/gtdbscrydb.html

[U81] JS：初始化项目
来源：http://hz.zycfv.cn/gtyxzqpilq.html

npm init -y;  npm i express
来源：http://hz.wangshuangyany.cn/gtnkeudfdb.html

[U82] JS：package.json 脚本
来源：http://hz.yuanzhike.top/gtimedazec.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinghuilouyu.cn/gtccvyqbyc.html

[U83] JS：ES Module 导入导出
来源：http://hz.feifeiyinyue.top/gtsimbndpa.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shangyingyoupin.top/gtarmuapbr.html

[U84] JS：CommonJS 写法
来源：http://hz.ydjk.org.cn/gtsdlqplcs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ehwqpu.com/gtssuprddk.html

[U85] JS：可选链
来源：http://hz.fzhhl.top/gtbleuwfrh.html

a?.b?.c
来源：http://hz.yj20258888.top/gtrystvstc.html

[U86] JS：空值合并
来源：http://hz.xuanzx.com/gtqywoitmh.html

a ?? b
来源：http://hz.haohaochexian.top/gtvcsjmrpv.html

[U87] JS：解构默认值
来源：http://hz.vqdsnc.cn/gtntgvtcmz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hnxiangtu.top/gtypoyrxlm.html

[U88] JS：对象展开合并
来源：http://hz.yj20258888.top/gtkoipinls.html

{ ...a, ...b }
来源：http://hz.daria6918.cn/gtgmhepypq.html

[U89] JS：数组去重
来源：http://hz.ppjwa.cn/gtapvamvpy.html

[...new Set(arr)]
来源：http://hz.iojbl.cn/gtiuyhwvpe.html

[U90] JS：数字数组排序
来源：http://hz.wangdashe.top/gtntqnhjyi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtvhymesbt.html

[U91] JS：对象键值遍历
来源：http://hz.xuanzx.com/gtwgzkkhxm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cqqwz.cn/gtsgcudekc.html

[U92] JS：深拷贝
来源：http://hz.xuetiantiany.cn/gtlofzpnup.html

structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtsbuyfmfk.html

[U93] JS：模板字符串
来源：http://hz.yvedp.cn/gtigkbfzhk.html

`共 ${n} 条`
来源：http://hz.ydjk.org.cn/gtdpnyubey.html

[U94] JS：箭头函数
来源：http://hz.daxiang520.top/gtfcxbdirh.html

const double = x => x * 2;
来源：http://hz.pengpengdd.cyou/gtgziawunz.html

[U95] JS：Promise 包装
来源：http://hz.dianchejie.cn/gtixwckmht.html

new Promise((resolve, reject) => {})
来源：http://hz.pycfn.com/gtuoosthnc.html

[U96] JS：async/await 与异常
来源：http://hz.pengpengdd.cyou/gtqdjrbpxy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtoxcrvzkv.html

[U97] JS：并发请求
来源：http://hz.xingfuxueyuan.xyz/gtpsykpfui.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtnsgifhib.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhixingplan.top/gtspzfhomv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.tanke756.top/gtszqvdyme.html

[U99] JS：事件监听
来源：http://hz.jqgufenzy.top/gtvttefdoe.html

el.addEventListener("click", e => {})
来源：http://hz.bjfxy.top/gtntwqntcr.html

[U100] JS：DOM 查询
来源：http://hz.52xcode.cn/gtvvyaidwg.html

document.querySelector(".item")
来源：http://hz.gotoacloud.top/gtxqmpmyky.html

[U101] JS：classList 操作
来源：http://hz.gotoacloud.top/gtzuczhbwp.html

el.classList.toggle("active")
来源：http://hz.sweek.top/gtpbkrmfoz.html

[U102] JS：本地存储
来源：http://hz.gogol.net.cn/gtllfstque.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinqigufen.top/gtoxsxuubb.html

[U103] JS：定时器
来源：http://hz.xinyue.icu/gteazihiwl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sxryk.cn/gtolkeypnj.html

[U104] JS：防抖
来源：http://hz.pycfn.com/gtakpztzlh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtrdvtppss.html

[U105] JS：节流
来源：http://hz.0kj1m.cn/gtmkpkfcwt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.tanke756.top/gtjkuotxgi.html

[U106] JS：日期格式化
来源：http://hz.tanke756.top/gtljxzuwbn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.chenlongwang.top/gtprnzgtbn.html

[U107] JS：数字千分位
来源：http://hz.yj20258888.top/gtvddkkgmh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinqigfzy.top/gtbjtxfcjc.html

[U108] JS：随机整数
来源：http://hz.pengpengdd.cyou/gtjfiwflwc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hnxiangtu.top/gtifkpzmvv.html

[U109] JS：数组分组
来源：http://hz.sysykeji.top/gtlclqdfuv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtjsseldxe.html

[U110] JS：数组分块
来源：http://hz.iojbl.cn/gtpyabxcvm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zycfv.cn/gtawgdhvcy.html

[U111] JS：对象转 Map
来源：http://hz.hnqzz.top/gtejcwkxlx.html

new Map(Object.entries(obj))
来源：http://hz.ydjk.org.cn/gtxdrreiji.html

[U112] JS：字符串补位
来源：http://hz.andypj.xyz/gttlcuidyc.html

"7".padStart(3, "0")
来源：http://hz.birdmap.top/gtmvrqkuwe.html

[U113] JS：正则替换全部
来源：http://hz.daxiang520.top/gtsydmfjwo.html

s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtfwfveyrz.html

[U114] JS：JSON 深比较
来源：http://hz.jianghu66.top/gtbcicrbcr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinghuilouyu.cn/gteaqvrewm.html

[U115] JS：生成 UUID
来源：http://hz.feifeiyinyue.top/gtzeodnkly.html

crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtlbraggjl.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hnqzz.top/gtxonlqhxj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shzxlz.cn/gtlpjantgq.html

[U117] JS：单元测试
来源：http://hz.shangyingyoupin.top/gtjetxstjz.html

npm i -D vitest;  npx vitest
来源：http://hz.chenzaomai.com/gtigvbdihz.html

[U118] JS：开发服务器
来源：http://hz.yongpay.top/gtsiqdtyxq.html

npm i -D vite;  npx vite
来源：http://hz.ybcxt.top/gteypdmqmt.html

[U119] JS：生产构建
来源：http://hz.hywenlv.cn/gtbvvqsifk.html

npx vite build
来源：http://hz.ivvv.top/gtniestbrj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ywan-chungtsiang.top/gtlwsjihht.html

import.meta.env.VITE_API_URL
来源：http://hz.jqgufenzy.top/gtukborrcz.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtjuzgrumc.html

统计汇总
来源：http://hz.snrcjt.cn/gtqxguiyge.html

================================================================================
来源：http://hz.gogol.net.cn/gtxilnbxct.html

按语言统计（条）：
来源：http://hz.zycfv.cn/gtwvmdymqg.html

Python ......... 252
来源：http://hz.tian-w.cn/gtqpqjxkuy.html

PHP ............ 252
来源：http://hz.shanyushiyangtech.top/gtinxwownd.html

JavaScript ..... 252
来源：http://hz.chenzaomai.com/gtvbjncwpp.html

TypeScript ..... 212
来源：http://hz.yonumen.top/gtohzunkhw.html

Java ........... 212
来源：http://hz.fzhhl.top/gtcihgrilo.html

Go ............. 212
来源：http://hz.wangshuangyany.cn/gtrbvddgow.html

Ruby ........... 212
来源：http://hz.hammf.cn/gtnxtuoglc.html

C# ............. 212
来源：http://hz.guowangkeji.top/gthmlzsljr.html

C .............. 30
来源：http://hz.jlsjyb.cn/gtpymnipts.html

C++ ............ 30
来源：http://hz.ydjk.org.cn/gtjdunxkgt.html

SQL ............ 90
来源：http://hz.ehwqpu.com/gtspoyacza.html

Bash ........... 80
来源：http://hz.yongpay.top/gttecupwob.html

Kotlin ......... 15
来源：http://hz.dashuyun.cn/gtauycfzox.html

Swift .......... 15
来源：http://hz.xingfuxueyuan.xyz/gtghgctubx.html

Lua ............ 10
来源：http://hz.yuanzhike.top/gtvquljzis.html

Perl ........... 10
来源：http://hz.cucudq.cn/gtviwhrevp.html

Scala .......... 10
来源：http://hz.jianghu66.top/gtndceqvhf.html

------------------------------------
来源：http://hz.hammf.cn/gtzzszexxa.html

合计 ........... 2106 条
来源：http://hz.shzxlz.cn/gtcarkzwuf.html

按章节统计：
来源：http://hz.xinyue.icu/gtnkxymquc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jlsjyb.cn/gtyrugjskn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gttxweivhc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.mhx1999.top/gttetzfxhw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cheryme.top/gtbebwkafe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zdqjudy.top/gtmnnlmfnz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhoulong.xyz/gtoxdzwlzi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gtsrcxruyy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sufxvd.cn/gtolnsapck.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtkqypqjeu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.birdmap.top/gtgopzyzec.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtudeqpjhv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hammf.cn/gtqrnulctg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtmmwgbpdp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.feifeiyinyue.top/gtjvzqfyuo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jlsjyb.cn/gtzbvgkddm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtxdwxmrvt.html

Q SQL 专题                              90
来源：http://hz.aibaodan.cn/gtvydkirtb.html

R Bash 专题                             80
来源：http://hz.jianghu66.top/gtyiujstmj.html

S C / C++ 专题                          60
来源：http://hz.jqgufenzy.top/gttkutigwi.html

T 其他语言补充                          60
来源：http://hz.gotoacloud.top/gtuaucgdye.html

U 高频实用片段                         120
来源：http://hz.gzhubu.top/gtednzrrny.html

------------------------------------
来源：http://hz.jqgfzy.top/gtxrmxtihz.html

合计                                  2106 条
来源：http://hz.nanxinkj.top/gtejxpbsty.html

--------------------------------------------------------------------------------
来源：http://hz.ivvv.top/gtqpahdgnc.html

使用提醒
来源：http://hz.zhengqikj.top/gtdwhuowvy.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gtdvmzznjy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jianghu66.top/gtctfymtgp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.c1oappe.top/gtyjkeputk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jinyuanbaomall.cn/gtcleqtzlt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.smart0.xyz/gtuodzdhwx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xuanzx.com/gtwywsguxg.html

—— 文件结束 ——
来源：http://hz.ivvv.top/gtmdcrewab.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwymnhyku.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj202588.top/gtmenayned.html

Common Programming Examples Cheat Book
来源：http://hz.shanyushiyangkeji.top/gtgepvxtzy.html

================================================================================
来源：http://hz.hnxiangtu.top/gtfvxdjsom.html

【收录内容】
来源：http://hz.yj202588.top/gtjwngqynp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cucudq.cn/gterseyruf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ywan-chungtsiang.top/gtfkwtndjs.html

SQL · Bash · C · C++
来源：http://hz.sufxvd.cn/gtwczadpcw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yuxming.cn/gtcygptdkn.html

【使用说明】
来源：http://hz.gogol.net.cn/gtvqqfivdr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.andypj.xyz/gtbxcpcefz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.tianlin.xyz/gttfpxorqt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.9152youxi.cn/gtouasgmyc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhoulong.xyz/gtugwcande.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.daxiang520.top/gtlajheccd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.redwolf501.top/gtlnvyzpfc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.redwolf501.top/gtnqrdnhgm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.52xcode.cn/gtqcjvtqvh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ivvv.top/gtphbhxbqg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xziqi.cn/gthycrlxha.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yuxming.cn/gtbnuhasqv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xingfuxueyuan.xyz/gtshhkggwb.html

【文件统计】
来源：http://hz.yj202588.top/gtbngljlxz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yuxming.cn/gtrwexuxjj.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtsrkdiqdt.html

目  录
来源：http://hz.xingfuxueyuan.xyz/gtbujzgmcm.html

--------------------------------------------------------------------------------
来源：http://hz.nanxuanxn.top/gtfmvnrney.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xinyue.icu/gtscqupyyx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yuanzhike.top/gtrdsqriwb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.iojbl.cn/gtmvlbbnun.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ivvv.top/gtgzlgtiuf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nanxuanxn.top/gtjrydaxly.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xinyue.icu/gtpxvbouil.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhijiandao.cn/gtvvqleehl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yueranfly.top/gtwdudtysg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gthqaqidjm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gttmpmicvp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yanxiufei.cn/gtglhubyfq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtydqfpiuk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xylfe.cn/gthftvbrss.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zdqjudy.top/gtwxjtbprf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jinghuilouyu.cn/gtpavxgwbw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtmvjkclda.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.snrcjt.cn/gtuhswfqpn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinqigfzy.top/gtfasltiby.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhixingplan.top/gtrjwvtoap.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yongpay.top/gtdsrumenp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gtnwgoccfo.html

================================================================================
来源：http://hz.guowangkeji.top/gtldfjknnv.html

A. 基础语法与类型
来源：http://hz.xziqi.cn/gtoayjmyxm.html

================================================================================
来源：http://hz.hnxiangtu.top/gtczximpkm.html

[A01] Hello World
来源：http://hz.xinyue.icu/gtcqflhoca.html

Py:   print("Hello, World!")
来源：http://hz.hnxiangtu.top/gtmujkldhu.html

PHP:  echo "Hello, World!";
来源：http://hz.tanke756.top/gthlxswpxe.html

JS:   console.log("Hello, World!");
来源：http://hz.dashuyun.cn/gtauhbsbak.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.sweek.top/gtcubrnfxg.html

Java: System.out.println("Hello, World!");
来源：http://hz.wangdashe.top/gtgzrciprl.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cheryme.top/gtiysyzxgy.html

Ruby: puts "Hello, World!"
来源：http://hz.jyoumei.cn/gtfjsmlieo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ppjwa.cn/gthcpemhkk.html

[A02] 变量声明与赋值
来源：http://hz.zhijiandao.cn/gttxuiegec.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hnqzz.top/gtkhercgcn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.gaohongyu789.top/gtdbauleil.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.xziqi.cn/gtcuffzdfu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jianghu66.top/gtqohxwyfx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xingfuxueyuan.xyz/gtlcswawix.html

Go:   name := "Alex"; age := 20
来源：http://hz.jlsjyb.cn/gtxkjjcqhp.html

Ruby: name = "Alex"; age = 20
来源：http://hz.tianlin.xyz/gtzpsvebyj.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhiwuduotai.top/gtwbfxsnvd.html

[A03] 常量定义
来源：http://hz.tianlin.xyz/gtduvbxksc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sxryk.cn/gtqnxshvgq.html

PHP:  const PI = 3.14159;
来源：http://hz.daxiang520.top/gtunildntg.html

JS:   const PI = 3.14159;
来源：http://hz.yangfankeji.com/gtptbclzvy.html

TS:   const PI: number = 3.14159;
来源：http://hz.316326.xyz/gteldorvjl.html

Java: static final double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtctswysbw.html

Go:   const PI = 3.14159
来源：http://hz.hammf.cn/gtesmgkuai.html

Ruby: PI = 3.14159
来源：http://hz.wangdashe.top/gtnwfyndpp.html

C#:   const double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtnvadllmu.html

[A04] 判断变量类型
来源：http://hz.hnqzz.top/gtocozjahw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhijiandao.cn/gtwzizjwtp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shangyingyoupin.top/gtohxekpsi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.tianlin.xyz/gtffpztzgr.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhongyouzk.top/gtcrajhfsj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yueranfly.top/gtrjcrtowt.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yuanzhike.top/gticjtixpi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yuxming.cn/gtxqzgyoci.html

C#:   x.GetType().Name; x is int
来源：http://hz.xziqi.cn/gtpllfocdu.html

[A05] 整数除法与取模
来源：http://hz.hywenlv.cn/gtwfokghgz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.wangshuangyany.cn/gtpagszvvn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.meibo888.top/gtxbpxewci.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yueranfly.top/gtzdybatkp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenlongwang.top/gtufprmusq.html

Java: 7 / 2; 7 % 2
来源：http://hz.9152youxi.cn/gtymlbfckv.html

Go:   7 / 2; 7 % 2
来源：http://hz.hongshengwenyu.top/gtczlgepqt.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtyjpedfqc.html

C#:   7 / 2; 7 % 2
来源：http://hz.feifeiyinyue.top/gthyjbxquo.html

[A06] 字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtwfwemtzf.html

Py:   int("42"); float("3.14")
来源：http://hz.9152youxi.cn/gthmekpwlu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhixingplan.top/gtndinztga.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cashguo.top/gteqjbiooh.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.daxiang520.top/gtbpzssipt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ehwqpu.com/gtvglnjvoa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ybcxt.top/gtwtawpwol.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yonumen.top/gtsvbyhoun.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.gzhubu.top/gtsxrvvmqj.html

[A07] 数字转字符串
来源：http://hz.jinqigufen.top/gtzelfbemn.html

Py:   str(42)
来源：http://hz.havefunace.top/gtfdqwbuev.html

PHP:  (string) 42; strval(42)
来源：http://hz.meibo888.top/gtdscqyetv.html

JS:   String(42); (42).toString()
来源：http://hz.shanyushiyangkeji.top/gtxyxxppye.html

TS:   String(42)
来源：http://hz.jlsjyb.cn/gtmdiiyuzq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.pycfn.com/gtprkboist.html

Go:   strconv.Itoa(42)
来源：http://hz.52xcode.cn/gttjouedcf.html

Ruby: 42.to_s
来源：http://hz.aibaodan.cn/gthrczqucv.html

C#:   42.ToString()
来源：http://hz.mhx1999.top/gthzejokuz.html

[A08] 取整与四舍五入
来源：http://hz.cucudq.cn/gtzmxdttsw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yuxming.cn/gtelpmyzcn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.ybcxt.top/gtzkspyahs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jqgufenzy.top/gthbryiygh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yueranfly.top/gtjpfhbryt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.quarkkingdee.top/gtgsxweuim.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.xziqi.cn/gtakcfcefp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yonumen.top/gtkwqpbpqf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yanxiufei.cn/gtjmcvtmse.html

[A09] 绝对值与最大最小值
来源：http://hz.xuanzx.com/gtvgvlgevx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ybcxt.top/gthbfjogwd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.dianchejie.cn/gthntydmbt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xuanzx.com/gtlhkwyjby.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.nwbrower.top/gtntcbfixu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinghuilouyu.cn/gtjjodspmw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.hnxiangtu.top/gtrhaibtrf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.chenzaomai.com/gtszinqpug.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ehwqpu.com/gtpcebjehw.html

[A10] 生成随机数
来源：http://hz.ivvv.top/gtdxozlvxh.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ybcxt.top/gtimcexzit.html

PHP:  random_int(1, 100);
来源：http://hz.zhixingplan.top/gtzlwkjcfv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.meibo888.top/gtbowortot.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shanyushiyangtech.top/gttkrlofvi.html

Java: new Random().nextInt(100) + 1
来源：http://hz.ehwqpu.com/gtjphlcswk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.shuidangran.top/gtpufjykhn.html

Ruby: rand(1..100)
来源：http://hz.jiagoushi.top/gtumbssncn.html

C#:   new Random().Next(1, 101)
来源：http://hz.iojbl.cn/gtkqslbcmw.html

[A11] 条件表达式（三元）
来源：http://hz.cqqwz.cn/gtuqnxvnjh.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jlsjyb.cn/gtfqhuagxq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.hysaishi.cn/gtpavpxogw.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.feifeiyinyue.top/gtksjktuhw.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.cheryme.top/gtvslmkpal.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.shangyingyoupin.top/gtdokdydtj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.zhengqikj.top/gtwmibcrnf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.ppjwa.cn/gtunyivxgb.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.tian-w.cn/gtpxmksiec.html

[A12] 字符串插值 / 格式化
来源：http://hz.jqgufenzy.top/gtanbwmlhz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.zhongyouzk.top/gtyetnmnvi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.jinghuilouyu.cn/gtviqhhlod.html

JS:   `Hello, ${name}!`
来源：http://hz.ydjk.org.cn/gtwdatshxa.html

TS:   `Hello, ${name}!`
来源：http://hz.havefunace.top/gthovvcbhd.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.gogol.net.cn/gttjbmtudo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jinghuilouyu.cn/gtmwaigegr.html

Ruby: "Hello, #{name}!"
来源：http://hz.tian-w.cn/gtqwuurske.html

C#:   $"Hello, {name}!"
来源：http://hz.ppjwa.cn/gtlsmgrwnu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.sysykeji.top/gtvkzbugck.html


<!-- 参考信息 -->