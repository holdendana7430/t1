代发 wailian999

[U79] PHP：静态分析
来源：http://hz.feifeiyinyue.top/gtwrsehuuq.html

composer require --dev phpstan/phpstan
来源：http://hz.ybcxt.top/gtwamlbppu.html

[U80] PHP：代码规范修复
来源：http://hz.pengpengdd.cyou/gtiqzanfnh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yvedp.cn/gtbgykwipx.html

[U81] JS：初始化项目
来源：http://hz.c1oappe.top/gthwnyglxx.html

npm init -y;  npm i express
来源：http://hz.nanxuanxn.top/gtsmptaqvi.html

[U82] JS：package.json 脚本
来源：http://hz.hfpthk.cn/gtoijzddrv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.guannengcc.top/gtumimgore.html

[U83] JS：ES Module 导入导出
来源：http://hz.xziqi.cn/gterxlfkfd.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.guannengcc.top/gtppqkbokp.html

[U84] JS：CommonJS 写法
来源：http://hz.zhongyouzk.top/gtpogeupdy.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cheryme.top/gtdjjzqudz.html

[U85] JS：可选链
来源：http://hz.chenzaomai.com/gtygtnbvit.html

a?.b?.c
来源：http://hz.jqgfzy.top/gtywmbstyg.html

[U86] JS：空值合并
来源：http://hz.cqqwz.cn/gtphpcnemd.html

a ?? b
来源：http://hz.fzhhl.top/gttrmotwic.html

[U87] JS：解构默认值
来源：http://hz.jyoumei.cn/gtvnpcncix.html

const { a = 1, b = 2 } = obj;
来源：http://hz.tian-w.cn/gtwvrjqmzr.html

[U88] JS：对象展开合并
来源：http://hz.bjfxy.top/gtyahcoxba.html

{ ...a, ...b }
来源：http://hz.yangfankeji.com/gtlurlnvlz.html

[U89] JS：数组去重
来源：http://hz.kuanghao11.cn/gtdbaouzse.html

[...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtpkbyuzui.html

[U90] JS：数字数组排序
来源：http://hz.gogol.net.cn/gtdqwpnroq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtegubyvde.html

[U91] JS：对象键值遍历
来源：http://hz.hnxiangtu.top/gtsjgshdbp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.kuanghao11.cn/gtkukdwekw.html

[U92] JS：深拷贝
来源：http://hz.shuidangran.top/gtrxelpxsd.html

structuredClone(obj)
来源：http://hz.xylfe.cn/gtlhxywvms.html

[U93] JS：模板字符串
来源：http://hz.jlsjyb.cn/gtbsamowxg.html

`共 ${n} 条`
来源：http://hz.wangshuangyany.cn/gtmgcpepja.html

[U94] JS：箭头函数
来源：http://hz.jinqigufen.top/gttzemeqqm.html

const double = x => x * 2;
来源：http://hz.zdqjudy.top/gtgynmzwor.html

[U95] JS：Promise 包装
来源：http://hz.andypj.xyz/gttaxfxrqb.html

new Promise((resolve, reject) => {})
来源：http://hz.fengsongda.top/gtpcoshaus.html

[U96] JS：async/await 与异常
来源：http://hz.hnqzz.top/gtnthnodle.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ivvv.top/gtcdzduqfq.html

[U97] JS：并发请求
来源：http://hz.hongshengwenyu.top/gtmhmncljz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtigjzkqrr.html

[U98] JS：fetch 带 JSON
来源：http://hz.hnxiangtu.top/gtxbidcjfg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj202588.top/gtlaxjbgmt.html

[U99] JS：事件监听
来源：http://hz.xingfuxueyuan.xyz/gtijsvtpcv.html

el.addEventListener("click", e => {})
来源：http://hz.hfpthk.cn/gtwjneyjbt.html

[U100] JS：DOM 查询
来源：http://hz.feifeiyinyue.top/gtkskpmcvy.html

document.querySelector(".item")
来源：http://hz.jinqigufen.top/gtmymulfjc.html

[U101] JS：classList 操作
来源：http://hz.vqdsnc.cn/gtzrosexnh.html

el.classList.toggle("active")
来源：http://hz.cqqwz.cn/gtuactpvqy.html

[U102] JS：本地存储
来源：http://hz.ywan-chungtsiang.top/gthumbldur.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.guowangkeji.top/gtmchqztpj.html

[U103] JS：定时器
来源：http://hz.hnqzz.top/gtmdakevru.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinyuanbaomall.cn/gtnicsmkjw.html

[U104] JS：防抖
来源：http://hz.tianlin.xyz/gtfwrctzvt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtdlpnilxg.html

[U105] JS：节流
来源：http://hz.gogol.net.cn/gtjfgylimt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuxming.cn/gtpvtjxmif.html

[U106] JS：日期格式化
来源：http://hz.zhongyouzk.top/gthridiweq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sysykeji.top/gtcxvvtzwg.html

[U107] JS：数字千分位
来源：http://hz.guowangkeji.top/gtkmkqhalf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shzxlz.cn/gtmvybqiob.html

[U108] JS：随机整数
来源：http://hz.zhoulong.xyz/gtgtudbxcv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj20258.top/gtjdjwsqca.html

[U109] JS：数组分组
来源：http://hz.shangyingyoupin.top/gtftgahjmy.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hammf.cn/gtudxzovdb.html

[U110] JS：数组分块
来源：http://hz.gogol.net.cn/gtifssuuqy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinqigufen.top/gtmkjxlscd.html

[U111] JS：对象转 Map
来源：http://hz.jinyuanbaomall.cn/gtcnubnckq.html

new Map(Object.entries(obj))
来源：http://hz.iojbl.cn/gtvnvvnjad.html

[U112] JS：字符串补位
来源：http://hz.ivvv.top/gtanmyzxvk.html

"7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gthhbeckle.html

[U113] JS：正则替换全部
来源：http://hz.xuanzx.com/gtzmkmoist.html

s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtjpkfmhva.html

[U114] JS：JSON 深比较
来源：http://hz.xuanzx.com/gtklucveln.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtviyacnln.html

[U115] JS：生成 UUID
来源：http://hz.cdnleiting.top/gtfifbznak.html

crypto.randomUUID()
来源：http://hz.yj20258.top/gtkwkjyezd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guowangkeji.top/gtwqwqkvlb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.wangshuangyany.cn/gtwsiqyvwj.html

[U117] JS：单元测试
来源：http://hz.cqqwz.cn/gtfsbqmifi.html

npm i -D vitest;  npx vitest
来源：http://hz.yangfankeji.com/gtvbgpzkhu.html

[U118] JS：开发服务器
来源：http://hz.svipenyu.cn/gtmzhasqbg.html

npm i -D vite;  npx vite
来源：http://hz.hongshengwenyu.top/gtwjrsxnne.html

[U119] JS：生产构建
来源：http://hz.zhaomingkeji.xyz/gtyhhjxvxz.html

npx vite build
来源：http://hz.jlsjyb.cn/gtjoguiepo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yangfankeji.com/gtvkctqsdw.html

import.meta.env.VITE_API_URL
来源：http://hz.jlsjyb.cn/gtbnikfqho.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmstzxjfz.html

统计汇总
来源：http://hz.birdmap.top/gtvhqdlrtt.html

================================================================================
来源：http://hz.jqgfzy.top/gtuzduqalb.html

按语言统计（条）：
来源：http://hz.sysykeji.top/gtqudpyblm.html

Python ......... 252
来源：http://hz.bjfxy.top/gtuviuumos.html

PHP ............ 252
来源：http://hz.quarkkingdee.top/gturseggyo.html

JavaScript ..... 252
来源：http://hz.nanxinkj.top/gtmhfqoyiv.html

TypeScript ..... 212
来源：http://hz.guannengcc.top/gtuualoqbw.html

Java ........... 212
来源：http://hz.yvedp.cn/gtdaenvist.html

Go ............. 212
来源：http://hz.cqqwz.cn/gthbbwcmca.html

Ruby ........... 212
来源：http://hz.52xcode.cn/gtqjetnmzg.html

C# ............. 212
来源：http://hz.shangyingyoupin.top/gttlyjojol.html

C .............. 30
来源：http://hz.hnqzz.top/gtxddvvfoe.html

C++ ............ 30
来源：http://hz.ydzc1.top/gtgkfjhpgk.html

SQL ............ 90
来源：http://hz.xuanzx.com/gtajtsasst.html

Bash ........... 80
来源：http://hz.yueranfly.top/gtpvlqyxlc.html

Kotlin ......... 15
来源：http://hz.ivvv.top/gtorkfwndd.html

Swift .......... 15
来源：http://hz.xylfe.cn/gtwqhjoieg.html

Lua ............ 10
来源：http://hz.zdqjudy.top/gtpkrnwlis.html

Perl ........... 10
来源：http://hz.tanke756.top/gtffkgxdwy.html

Scala .......... 10
来源：http://hz.gogol.net.cn/gtvcoaeetw.html

------------------------------------
来源：http://hz.zhixingplan.top/gtesmyqbma.html

合计 ........... 2106 条
来源：http://hz.sxryk.cn/gtwpphdsyy.html

按章节统计：
来源：http://hz.iojbl.cn/gtnvhxpyry.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yonumen.top/gtqavaxqyh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yuanzhike.top/gtbdwhujpi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zycfv.cn/gtqbzkgfca.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.52xcode.cn/gtnunnmehk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenlongwang.top/gtzzfwuewt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtvgjpbgtm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gtibemmyxv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj202588.top/gtykdrmltl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtvgmvphpy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hywenlv.cn/gtvhwczgju.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtwgmsdxtd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gterktgvue.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtinjxopfi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ydjk.org.cn/gtcckddujn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.52xcode.cn/gtzzwmwljw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtzqjxejoj.html

Q SQL 专题                              90
来源：http://hz.xylfe.cn/gtbctahxpv.html

R Bash 专题                             80
来源：http://hz.sweek.top/gtrtsafyzk.html

S C / C++ 专题                          60
来源：http://hz.yangfankeji.com/gtjgameixc.html

T 其他语言补充                          60
来源：http://hz.aibaodan.cn/gtijocxiyl.html

U 高频实用片段                         120
来源：http://hz.dianchejie.cn/gtqithbdug.html

------------------------------------
来源：http://hz.yongpay.top/gtraoqtgqq.html

合计                                  2106 条
来源：http://hz.yanxiufei.cn/gtpjgtnehv.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtrralicky.html

使用提醒
来源：http://hz.chenlongwang.top/gtslozvoru.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gtenedxzzy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.gaohongyu789.top/gtberljmso.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yonumen.top/gtvsnnoumq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.andypj.xyz/gtdbocnlfa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.shzxlz.cn/gtzzwfjtlk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.haohaochexian.top/gtpjkthnli.html

—— 文件结束 ——
来源：http://hz.ydjk.org.cn/gtilowpihr.html

================================================================================
来源：http://hz.9152youxi.cn/gtcyxhskui.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.gogol.net.cn/gtozawkzuh.html

Common Programming Examples Cheat Book
来源：http://hz.fengsongda.top/gttmgcdlig.html

================================================================================
来源：http://hz.shuidangran.top/gtkckamzrj.html

【收录内容】
来源：http://hz.redwolf501.top/gtkxgefwqt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.guannengcc.top/gtmujmstyc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhaomingkeji.xyz/gtkqgerwwp.html

SQL · Bash · C · C++
来源：http://hz.ybcxt.top/gtsiapvmjf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinghuilouyu.cn/gtgvscrrnd.html

【使用说明】
来源：http://hz.gaohongyu789.top/gtnhppbote.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.daxiang520.top/gtoqznhgal.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhiwuduotai.top/gtighgehnb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ivvv.top/gtifkcusmd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xuetiantiany.cn/gtvsewbxlg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hnqzz.top/gtomejvueu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gogol.net.cn/gtpxwkjmov.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jlsjyb.cn/gtoyoypslr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ybcxt.top/gtmukeyuyo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hfpthk.cn/gtdlknfjhj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.guowangkeji.top/gtblhznejj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhaomingkeji.xyz/gthgldthof.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yongpay.top/gtujzthugk.html

【文件统计】
来源：http://hz.jiagoushi.top/gtomtwzhkk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.daria6918.cn/gtegncwlxe.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gtrwbbwnxc.html

目  录
来源：http://hz.cqqwz.cn/gtsujvreqv.html

--------------------------------------------------------------------------------
来源：http://hz.wangshuangyany.cn/gteoahorub.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.c1oappe.top/gtqmgsfmlj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhiwuduotai.top/gtxorditdd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.havefunace.top/gtjuiwkjhd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ywan-chungtsiang.top/gtbcjwvajd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.gotoacloud.top/gtrddniqgk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.havefunace.top/gtdfjtswkb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cdnleiting.top/gtbpiqeuoa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cashguo.top/gtphpryvsn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtbnvvxpew.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.0kj1m.cn/gtjxrjhizl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtzhktnbcq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtphaqkdbe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtzufriadi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.tian-w.cn/gtkhfhxgfl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj20258.top/gthzojevcf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtvcjtyrwl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.mhx1999.top/gtivgnzfjn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.dianchejie.cn/gtpuqvlvbf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ybcxt.top/gthqrahboc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gtzafmqvbx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.dashuyun.cn/gthxlaeinp.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtrrftncbi.html

A. 基础语法与类型
来源：http://hz.kuanghao11.cn/gtyhldxvlb.html

================================================================================
来源：http://hz.havefunace.top/gtsaxdwesg.html

[A01] Hello World
来源：http://hz.birdmap.top/gtqrhduiwm.html

Py:   print("Hello, World!")
来源：http://hz.guowangkeji.top/gtwomphhcg.html

PHP:  echo "Hello, World!";
来源：http://hz.daria6918.cn/gtituocehg.html

JS:   console.log("Hello, World!");
来源：http://hz.yuxming.cn/gtdkcepsuu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhijiandao.cn/gtpszisgcf.html

Java: System.out.println("Hello, World!");
来源：http://hz.mhx1999.top/gtarcfytfa.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.gogol.net.cn/gtogqohcjs.html

Ruby: puts "Hello, World!"
来源：http://hz.ybcxt.top/gtisbcvwoq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hysaishi.cn/gtnydmvmcy.html

[A02] 变量声明与赋值
来源：http://hz.jianghu66.top/gtwttkqtjy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhixingplan.top/gtsiteailj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shanyushiyangkeji.top/gtywbnashs.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.cdnleiting.top/gtfnhiorcj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yongpay.top/gtrczjpldx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.gzhubu.top/gtvelopium.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhiwuduotai.top/gtdmgemfme.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinghuilouyu.cn/gtlefogpvu.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.fzhhl.top/gthfslwcey.html

[A03] 常量定义
来源：http://hz.zdqjudy.top/gtrymqexxb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ivvv.top/gtzukhvyxl.html

PHP:  const PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtoplljrmp.html

JS:   const PI = 3.14159;
来源：http://hz.0kj1m.cn/gtcohaisus.html

TS:   const PI: number = 3.14159;
来源：http://hz.jiagoushi.top/gtndcpcotj.html

Java: static final double PI = 3.14159;
来源：http://hz.redwolf501.top/gtmmjydznn.html

Go:   const PI = 3.14159
来源：http://hz.yj202588.top/gthxoijtna.html

Ruby: PI = 3.14159
来源：http://hz.cashguo.top/gtyxpsjoxj.html

C#:   const double PI = 3.14159;
来源：http://hz.redwolf501.top/gthoygesao.html

[A04] 判断变量类型
来源：http://hz.aizwys.cn/gtaiwomxue.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yongpay.top/gtyjgykdni.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.aibaodan.cn/gtenskuwxk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.pycfn.com/gtqoswuidu.html

TS:   typeof x; x instanceof Date
来源：http://hz.yvedp.cn/gtqofrsznz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.chenlongwang.top/gtzgczyhyz.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.tian-w.cn/gtcavbjrif.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xziqi.cn/gtgwlfmbiu.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhaomingkeji.xyz/gtqypwwttg.html

[A05] 整数除法与取模
来源：http://hz.52xcode.cn/gtmtyhbcie.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.chenjidiqi.icu/gtaszqyotu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jinqigufen.top/gtdutwocvv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhoulong.xyz/gtoxqqpwbx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pycfn.com/gtsioofgin.html

Java: 7 / 2; 7 % 2
来源：http://hz.zhijiandao.cn/gtanhglsxs.html

Go:   7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtnxamefof.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ehwqpu.com/gthywobwiw.html

C#:   7 / 2; 7 % 2
来源：http://hz.tanke756.top/gthhcnrsds.html

[A06] 字符串转数字
来源：http://hz.shzxlz.cn/gtiaptzact.html

Py:   int("42"); float("3.14")
来源：http://hz.jyoumei.cn/gtvwbzuedw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yangfankeji.com/gtiutmgbpw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jlsjyb.cn/gtactmxnbb.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.birdmap.top/gtljkzipgb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.feifeiyinyue.top/gttojxmnqa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.feifeiyinyue.top/gtvddonwai.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jinqigufen.top/gtezovvzab.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xylfe.cn/gtytzmelbw.html

[A07] 数字转字符串
来源：http://hz.wangshuangyany.cn/gtukgtllle.html

Py:   str(42)
来源：http://hz.9152youxi.cn/gtbtcsjlou.html

PHP:  (string) 42; strval(42)
来源：http://hz.mhx1999.top/gtflbpgdjs.html

JS:   String(42); (42).toString()
来源：http://hz.vqdsnc.cn/gtubtppirt.html

TS:   String(42)
来源：http://hz.shanyushiyangtech.top/gtordrmkdj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xuanzx.com/gtvcsdgiwp.html

Go:   strconv.Itoa(42)
来源：http://hz.hywenlv.cn/gtyvteltmg.html

Ruby: 42.to_s
来源：http://hz.havefunace.top/gtypxpigzn.html

C#:   42.ToString()
来源：http://hz.yonumen.top/gtrqqanyxc.html

[A08] 取整与四舍五入
来源：http://hz.tianlin.xyz/gtaydskoru.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.hongshengwenyu.top/gtewycjbch.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yuxming.cn/gtityytvzz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.quarkkingdee.top/gtmzyxvqpi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.haohaochexian.top/gtxpypdwaf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.gogol.net.cn/gtkxojeknj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.tanke756.top/gtdqnvbwzv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.xuanzx.com/gtjfuipmmm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.tianlin.xyz/gtmefwdoqc.html

[A09] 绝对值与最大最小值
来源：http://hz.andypj.xyz/gtbbyliden.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.chenzaomai.com/gtqiebfqwp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.fengsongda.top/gtiwqodlrx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.pycfn.com/gtcbfkzbfi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.chenlongwang.top/gtqfcrezom.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.feifeiyinyue.top/gtkxwonfnz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.vqdsnc.cn/gtrrxymgbg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.chenzaomai.com/gtxudtpphs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yj20258888.top/gtmgszgysb.html

[A10] 生成随机数
来源：http://hz.yj202588.top/gthbuftlze.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hnxiangtu.top/gthutjjxkb.html

PHP:  random_int(1, 100);
来源：http://hz.jqgfzy.top/gtfvsvwseq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hysaishi.cn/gtcowiexwv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yuanzhike.top/gtuedzsray.html

Java: new Random().nextInt(100) + 1
来源：http://hz.nanxinkj.top/gtcadmacwx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.aibaodan.cn/gttaszpajq.html

Ruby: rand(1..100)
来源：http://hz.haohaochexian.top/gtmnxoyeiz.html

C#:   new Random().Next(1, 101)
来源：http://hz.aibaodan.cn/gtvxyxexsk.html

[A11] 条件表达式（三元）
来源：http://hz.zhengqikj.top/gtnaknbmug.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.wangshuangyany.cn/gthhdsxkty.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jqgufenzy.top/gtsturjrlq.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.hysaishi.cn/gtnaodjrni.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhongyouzk.top/gtpctojsoj.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.c1oappe.top/gtwrnueewm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.zhiwuduotai.top/gtlirezxqz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.9152youxi.cn/gtgrhuzzdx.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.316326.xyz/gtebzoqxqc.html

[A12] 字符串插值 / 格式化
来源：http://hz.xinyue.icu/gthnmoqamt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.xuanzx.com/gtjrbquzbg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.pycfn.com/gtbaykgsfi.html

JS:   `Hello, ${name}!`
来源：http://hz.cucudq.cn/gtmzqneslo.html

TS:   `Hello, ${name}!`
来源：http://hz.ybcxt.top/gtgeepzjfm.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jinghuilouyu.cn/gthjvkbmrc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.shangyingyoupin.top/gthoyvdjtw.html

Ruby: "Hello, #{name}!"
来源：http://hz.daxiang520.top/gttjknkrdt.html

C#:   $"Hello, {name}!"
来源：http://hz.mhx1999.top/gtyenojbdo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.chenzaomai.com/gthpmyicdp.html


<!-- 参考信息 -->