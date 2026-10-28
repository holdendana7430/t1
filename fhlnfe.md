代发 wailian999

[U79] PHP：静态分析
来源：http://hz.xinyue.icu/gttkjjjvam.html

composer require --dev phpstan/phpstan
来源：http://hz.hnqzz.top/gtdzaloqdp.html

[U80] PHP：代码规范修复
来源：http://hz.0kj1m.cn/gtlchggkqx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zycfv.cn/gtuspyogeh.html

[U81] JS：初始化项目
来源：http://hz.xylfe.cn/gtceamtvla.html

npm init -y;  npm i express
来源：http://hz.chenlongwang.top/gtpjtulcgw.html

[U82] JS：package.json 脚本
来源：http://hz.yj20258888.top/gtmwqbkypq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhongyouzk.top/gtikuotoau.html

[U83] JS：ES Module 导入导出
来源：http://hz.wangshuangyany.cn/gtrugapglq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.52xcode.cn/gtiyzptmjs.html

[U84] JS：CommonJS 写法
来源：http://hz.smart0.xyz/gtfjpdzrcc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.shzxlz.cn/gtgsyslzqa.html

[U85] JS：可选链
来源：http://hz.ivvv.top/gtuiomuohd.html

a?.b?.c
来源：http://hz.jinghuilouyu.cn/gtpfuuvfhu.html

[U86] JS：空值合并
来源：http://hz.ywan-chungtsiang.top/gtncsnbasm.html

a ?? b
来源：http://hz.svipenyu.cn/gttztygmpj.html

[U87] JS：解构默认值
来源：http://hz.hywenlv.cn/gtrytjhefg.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sufxvd.cn/gtmkmkbsuu.html

[U88] JS：对象展开合并
来源：http://hz.jinghuilouyu.cn/gtppgdocco.html

{ ...a, ...b }
来源：http://hz.zdqjudy.top/gthpahbujt.html

[U89] JS：数组去重
来源：http://hz.sweek.top/gthnzlfdal.html

[...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtwtcvsxrf.html

[U90] JS：数字数组排序
来源：http://hz.yanxiufei.cn/gtnzncqrfq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtdkuyrict.html

[U91] JS：对象键值遍历
来源：http://hz.dashuyun.cn/gtgltzkpkc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.redwolf501.top/gtuzayxtjw.html

[U92] JS：深拷贝
来源：http://hz.aizwys.cn/gtzmzkudbl.html

structuredClone(obj)
来源：http://hz.chenlongwang.top/gtfbhlzvjc.html

[U93] JS：模板字符串
来源：http://hz.shzxlz.cn/gttlsbhcha.html

`共 ${n} 条`
来源：http://hz.jinyuanbaomall.cn/gtcwsstvao.html

[U94] JS：箭头函数
来源：http://hz.yanxiufei.cn/gtwhevzboz.html

const double = x => x * 2;
来源：http://hz.jlsjyb.cn/gtadeieptq.html

[U95] JS：Promise 包装
来源：http://hz.gzhubu.top/gtwtibbrva.html

new Promise((resolve, reject) => {})
来源：http://hz.gotoacloud.top/gtfstscula.html

[U96] JS：async/await 与异常
来源：http://hz.chenzaomai.com/gtgtpdvybp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtsxjwecsc.html

[U97] JS：并发请求
来源：http://hz.daria6918.cn/gttwplanbf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtbrpnlzge.html

[U98] JS：fetch 带 JSON
来源：http://hz.gzhubu.top/gtkwqkcwwq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ehwqpu.com/gtaspfvufc.html

[U99] JS：事件监听
来源：http://hz.mhx1999.top/gtxdplktph.html

el.addEventListener("click", e => {})
来源：http://hz.tian-w.cn/gtwgkmhwjl.html

[U100] JS：DOM 查询
来源：http://hz.zhijiandao.cn/gtzodkeowb.html

document.querySelector(".item")
来源：http://hz.yongpay.top/gtcdkidrhc.html

[U101] JS：classList 操作
来源：http://hz.9152youxi.cn/gtpsjohxkh.html

el.classList.toggle("active")
来源：http://hz.9152youxi.cn/gtokywcneo.html

[U102] JS：本地存储
来源：http://hz.52xcode.cn/gtjlaybpcn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ywan-chungtsiang.top/gtghexrmeq.html

[U103] JS：定时器
来源：http://hz.yueranfly.top/gtnjbrstkz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinyuanbaomall.cn/gtdxlonuaw.html

[U104] JS：防抖
来源：http://hz.shangyingyoupin.top/gtvzhkjiwc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtbdsomrsk.html

[U105] JS：节流
来源：http://hz.zhixingplan.top/gtbqdcgynf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jiagoushi.top/gtmcshhghr.html

[U106] JS：日期格式化
来源：http://hz.zdqjudy.top/gtxuilualz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxuanxn.top/gtngjmmckh.html

[U107] JS：数字千分位
来源：http://hz.xinyue.icu/gtqftnnebj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hammf.cn/gtoocnayik.html

[U108] JS：随机整数
来源：http://hz.tian-w.cn/gtfzzokeet.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhoulong.xyz/gtusjwebmh.html

[U109] JS：数组分组
来源：http://hz.aizwys.cn/gtiazcjbkv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangtech.top/gtvkoqynlp.html

[U110] JS：数组分块
来源：http://hz.shanyushiyangkeji.top/gtfarwlocx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jiagoushi.top/gtaxktpujj.html

[U111] JS：对象转 Map
来源：http://hz.hfpthk.cn/gttgjvympv.html

new Map(Object.entries(obj))
来源：http://hz.yuanzhike.top/gtnfvttshk.html

[U112] JS：字符串补位
来源：http://hz.kuanghao11.cn/gtkwzcesfx.html

"7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtibwbtnjp.html

[U113] JS：正则替换全部
来源：http://hz.nanxinkj.top/gtqitdissa.html

s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtowhfjcbv.html

[U114] JS：JSON 深比较
来源：http://hz.snrcjt.cn/gtefmacqhg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yueranfly.top/gtwypdoaog.html

[U115] JS：生成 UUID
来源：http://hz.zdqjudy.top/gtwebiupep.html

crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtxbepednk.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.chenlongwang.top/gtyjsqpbav.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cdnleiting.top/gtgohgynzq.html

[U117] JS：单元测试
来源：http://hz.zhixingplan.top/gtbxktpxbu.html

npm i -D vitest;  npx vitest
来源：http://hz.xuanzx.com/gtjgfdjfpc.html

[U118] JS：开发服务器
来源：http://hz.xinyue.icu/gtrntkdhuu.html

npm i -D vite;  npx vite
来源：http://hz.hongshengwenyu.top/gtkmlrjada.html

[U119] JS：生产构建
来源：http://hz.shanyushiyangtech.top/gtslefbhmf.html

npx vite build
来源：http://hz.tianlin.xyz/gtgnjzfjgo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gaohongyu789.top/gtuwcmysbl.html

import.meta.env.VITE_API_URL
来源：http://hz.dianchejie.cn/gtifrpbrob.html

================================================================================
来源：http://hz.hywenlv.cn/gtnojpxauc.html

统计汇总
来源：http://hz.svipenyu.cn/gtxuapfjxp.html

================================================================================
来源：http://hz.meibo888.top/gtxkovkdfb.html

按语言统计（条）：
来源：http://hz.xuanzx.com/gtetayvleg.html

Python ......... 252
来源：http://hz.hfpthk.cn/gtefgpykij.html

PHP ............ 252
来源：http://hz.fzhhl.top/gtlgulljys.html

JavaScript ..... 252
来源：http://hz.gogol.net.cn/gtviikcrto.html

TypeScript ..... 212
来源：http://hz.chenzaomai.com/gthczgksaz.html

Java ........... 212
来源：http://hz.birdmap.top/gtkbdedozq.html

Go ............. 212
来源：http://hz.daria6918.cn/gtvprgbttr.html

Ruby ........... 212
来源：http://hz.haohaochexian.top/gtqxgkmzvf.html

C# ............. 212
来源：http://hz.sxryk.cn/gtgdimrccv.html

C .............. 30
来源：http://hz.zycfv.cn/gtcbawjlib.html

C++ ............ 30
来源：http://hz.vqdsnc.cn/gtbfapzcyd.html

SQL ............ 90
来源：http://hz.hysaishi.cn/gthutbqlql.html

Bash ........... 80
来源：http://hz.yanxiufei.cn/gtnmtilanv.html

Kotlin ......... 15
来源：http://hz.nanxinkj.top/gtbjkwmosl.html

Swift .......... 15
来源：http://hz.zycfv.cn/gtocjoausq.html

Lua ............ 10
来源：http://hz.xingfuxueyuan.xyz/gtdxsgfqtn.html

Perl ........... 10
来源：http://hz.hnqzz.top/gtcuufhlft.html

Scala .......... 10
来源：http://hz.jyoumei.cn/gtasitwmhc.html

------------------------------------
来源：http://hz.xinyue.icu/gtbzyqdnta.html

合计 ........... 2106 条
来源：http://hz.zhijiandao.cn/gtloexbyih.html

按章节统计：
来源：http://hz.nanxinkj.top/gtsjawuyyo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xuanzx.com/gtbqbqsirf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jqgufenzy.top/gtoyxiesar.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gtrhzywxeo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yj20258.top/gtorrgisdg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hfpthk.cn/gtujgptunv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigfzy.top/gtjdsvgbux.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtyvuvrmto.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jqgufenzy.top/gtyqacezjg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtqsqhetvz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yuxming.cn/gtbgbduqgj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gtaiihasrj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtjnaiderc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtldwfbdrh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.kuanghao11.cn/gtmaaevekk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hammf.cn/gtiexcuwyn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtqrzyntap.html

Q SQL 专题                              90
来源：http://hz.quarkkingdee.top/gtaiicbohj.html

R Bash 专题                             80
来源：http://hz.smart0.xyz/gtewlovoca.html

S C / C++ 专题                          60
来源：http://hz.fzhhl.top/gtotwmrcqj.html

T 其他语言补充                          60
来源：http://hz.chenlongwang.top/gtbsnytzxc.html

U 高频实用片段                         120
来源：http://hz.cashguo.top/gtygeptfle.html

------------------------------------
来源：http://hz.yj20258888.top/gtpiqwtysv.html

合计                                  2106 条
来源：http://hz.nwbrower.top/gtzqjqzphk.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gtwcnnbnqf.html

使用提醒
来源：http://hz.yonumen.top/gtnlsvutqz.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtvhjndbpi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.9152youxi.cn/gtjzxudntl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yvedp.cn/gtefxlukjq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jinqigfzy.top/gtexblmclq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ydzc1.top/gtpikxjoux.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.quarkkingdee.top/gttsbphqpt.html

—— 文件结束 ——
来源：http://hz.shuidangran.top/gtsogfsssj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwlowuhlo.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.guannengcc.top/gtzwezgxri.html

Common Programming Examples Cheat Book
来源：http://hz.cdnleiting.top/gtahcbahgh.html

================================================================================
来源：http://hz.vqdsnc.cn/gtkawkzwfb.html

【收录内容】
来源：http://hz.cheryme.top/gtriqgfygn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xuanzx.com/gtajfynmrv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhoulong.xyz/gtdmdarooy.html

SQL · Bash · C · C++
来源：http://hz.chenlongwang.top/gtraqnetvk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.0kj1m.cn/gtgwwyesaw.html

【使用说明】
来源：http://hz.hongshengwenyu.top/gtqkymhdib.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.gogol.net.cn/gtdeipagrl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hywenlv.cn/gtpmxiojlk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenzaomai.com/gtmpjfhwsn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhongyouzk.top/gtewnypbzv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinqigfzy.top/gtieitfroa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.kuanghao11.cn/gtjniyamxw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.9152youxi.cn/gtjtosiihg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yj20258888.top/gtvosmsuui.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.birdmap.top/gtsigfpacf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jiagoushi.top/gtrkjymctn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.andypj.xyz/gthbchdmhf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yonumen.top/gtzcfjknip.html

【文件统计】
来源：http://hz.xuetiantiany.cn/gtplwsmimf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ybcxt.top/gtcphucggz.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtafrytxqj.html

目  录
来源：http://hz.aibaodan.cn/gtcqmucehi.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtcxqjnskt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gtynqgztws.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xuanzx.com/gtzotcmnve.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shzxlz.cn/gtgyhrdcst.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jlsjyb.cn/gttpatwyqo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xziqi.cn/gtyvtrzplp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhiwuduotai.top/gtzvnujifz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gogol.net.cn/gttacmhomj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.52xcode.cn/gtcsazyqkc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtergqnmcu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cashguo.top/gtbsiywonh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gtngfjfyjt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtnzvklcwq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gtorucsdqc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhongyouzk.top/gtbdbwppkg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.fzhhl.top/gtccpsfqxc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtbtniefao.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.hongshengwenyu.top/gtwrthlnun.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.wangshuangyany.cn/gtjdueydul.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.tanke756.top/gtzhtnqfau.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xylfe.cn/gtjavsdiau.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xingfuxueyuan.xyz/gtycsbkoun.html

================================================================================
来源：http://hz.hysaishi.cn/gtmsptjhtc.html

A. 基础语法与类型
来源：http://hz.hnxiangtu.top/gtxravqpdo.html

================================================================================
来源：http://hz.cheryme.top/gtbxrychnu.html

[A01] Hello World
来源：http://hz.jqgfzy.top/gttwnesrel.html

Py:   print("Hello, World!")
来源：http://hz.pycfn.com/gtmsynaghn.html

PHP:  echo "Hello, World!";
来源：http://hz.shuidangran.top/gtzqbmtlpo.html

JS:   console.log("Hello, World!");
来源：http://hz.9152youxi.cn/gtnahowbum.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.aizwys.cn/gtybblwols.html

Java: System.out.println("Hello, World!");
来源：http://hz.jlsjyb.cn/gtemyjlzxz.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.guowangkeji.top/gtvwzsmpsn.html

Ruby: puts "Hello, World!"
来源：http://hz.quarkkingdee.top/gtlowcznst.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yuanzhike.top/gteclginzp.html

[A02] 变量声明与赋值
来源：http://hz.yangfankeji.com/gtfurefbpk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.birdmap.top/gtjcdntodl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.xziqi.cn/gtxwvcgfea.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hammf.cn/gtepwbcmck.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.smart0.xyz/gtpizhcnqi.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.dashuyun.cn/gtmwyzmdin.html

Go:   name := "Alex"; age := 20
来源：http://hz.fengsongda.top/gtzwdpqlni.html

Ruby: name = "Alex"; age = 20
来源：http://hz.guowangkeji.top/gtcttneygr.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.chenzaomai.com/gtageeilqp.html

[A03] 常量定义
来源：http://hz.meibo888.top/gtgjxidpfb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.cucudq.cn/gtsrrmfjxo.html

PHP:  const PI = 3.14159;
来源：http://hz.meibo888.top/gtlerqkzth.html

JS:   const PI = 3.14159;
来源：http://hz.hfpthk.cn/gtpkvteenb.html

TS:   const PI: number = 3.14159;
来源：http://hz.fzhhl.top/gtfzssgiki.html

Java: static final double PI = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtofvihrfq.html

Go:   const PI = 3.14159
来源：http://hz.zhongyouzk.top/gtfvkqhqhd.html

Ruby: PI = 3.14159
来源：http://hz.yj202588.top/gtbxjqviwf.html

C#:   const double PI = 3.14159;
来源：http://hz.wangshuangyany.cn/gteqqkhnve.html

[A04] 判断变量类型
来源：http://hz.snrcjt.cn/gtsasbaubs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jlsjyb.cn/gtjabnkrtx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shanyushiyangtech.top/gtsopilykl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.snrcjt.cn/gtdeonazrj.html

TS:   typeof x; x instanceof Date
来源：http://hz.kuanghao11.cn/gttcrlsjei.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yvedp.cn/gtfupoxwsj.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yvedp.cn/gtgvhaeujb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yuxming.cn/gtxjqwguqi.html

C#:   x.GetType().Name; x is int
来源：http://hz.cucudq.cn/gtepknswoy.html

[A05] 整数除法与取模
来源：http://hz.yj20258888.top/gtsygdhhkv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhengqikj.top/gtqhamippc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jqgufenzy.top/gtxcfbkgyo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shangyingyoupin.top/gtnflswxsg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ivvv.top/gtqhvfqnuz.html

Java: 7 / 2; 7 % 2
来源：http://hz.316326.xyz/gtridrbcxf.html

Go:   7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gteotpjjzs.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ydzc1.top/gteqpotjvr.html

C#:   7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtghdtfeyx.html

[A06] 字符串转数字
来源：http://hz.aibaodan.cn/gtvxcwpgig.html

Py:   int("42"); float("3.14")
来源：http://hz.52xcode.cn/gtgmjzokgu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.sysykeji.top/gtcpisfihb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.meibo888.top/gtmivuekic.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.shangyingyoupin.top/gttzqujvyf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zdqjudy.top/gtkvbxztsi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.guowangkeji.top/gtvivkkayg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yvedp.cn/gtxkiwsdrl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.kuanghao11.cn/gtdeurkdik.html

[A07] 数字转字符串
来源：http://hz.aizwys.cn/gtdlqiihmi.html

Py:   str(42)
来源：http://hz.aibaodan.cn/gtarhzfzdn.html

PHP:  (string) 42; strval(42)
来源：http://hz.birdmap.top/gtcnmbtmgx.html

JS:   String(42); (42).toString()
来源：http://hz.yj20258888.top/gttkhbxstj.html

TS:   String(42)
来源：http://hz.316326.xyz/gtokwwcihv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hysaishi.cn/gtozxaygby.html

Go:   strconv.Itoa(42)
来源：http://hz.jianghu66.top/gtxnmilvnx.html

Ruby: 42.to_s
来源：http://hz.jlsjyb.cn/gtspwfcodw.html

C#:   42.ToString()
来源：http://hz.jinqigufen.top/gtnfvxhxho.html

[A08] 取整与四舍五入
来源：http://hz.gotoacloud.top/gtebekjjio.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jlsjyb.cn/gtvuwhfvaq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.nanxuanxn.top/gtnceqbsak.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.fengsongda.top/gtouqpintd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.haohaochexian.top/gtoasehrwg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.chenjidiqi.icu/gthqkarisr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.xylfe.cn/gtunyeqmbn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.iojbl.cn/gtfjtmhdll.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.zhixingplan.top/gtiegmphgu.html

[A09] 绝对值与最大最小值
来源：http://hz.ehwqpu.com/gtboxxywtn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.gogol.net.cn/gtlujvfztk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yongpay.top/gtelodapvg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhijiandao.cn/gtfxlsbavw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jiagoushi.top/gtpmxpsypv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hammf.cn/gtgvjsgpnp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.cashguo.top/gtntwwzjap.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.shzxlz.cn/gtykglyzaf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.wangdashe.top/gtabhwbuwa.html

[A10] 生成随机数
来源：http://hz.tian-w.cn/gtpthubhco.html

Py:   import random; random.randint(1, 100)
来源：http://hz.feifeiyinyue.top/gtdtvlfdik.html

PHP:  random_int(1, 100);
来源：http://hz.yuanzhike.top/gtxxiymgpp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.sysykeji.top/gtisyudczc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.meibo888.top/gtepegeofw.html

Java: new Random().nextInt(100) + 1
来源：http://hz.ppjwa.cn/gtrmcdwwei.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinghuilouyu.cn/gtrhuiwpyn.html

Ruby: rand(1..100)
来源：http://hz.hnxiangtu.top/gtmibvrcpz.html

C#:   new Random().Next(1, 101)
来源：http://hz.ybcxt.top/gtngjbjnmc.html

[A11] 条件表达式（三元）
来源：http://hz.haohaochexian.top/gtsacigmji.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.yj202588.top/gtsknwxjjw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yanxiufei.cn/gtinhyhnzr.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.aibaodan.cn/gteluqzmox.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.sxryk.cn/gthrmsraqj.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.haohaochexian.top/gthnqlplgj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.yuanzhike.top/gtgqmpfupv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.zhongyouzk.top/gtihmlmpqh.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.redwolf501.top/gtweiagact.html

[A12] 字符串插值 / 格式化
来源：http://hz.hammf.cn/gtkjsozaow.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.gzhubu.top/gttcdhhzjt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.jqgfzy.top/gtqzfolxnm.html

JS:   `Hello, ${name}!`
来源：http://hz.xingfuxueyuan.xyz/gtkojrpfcs.html

TS:   `Hello, ${name}!`
来源：http://hz.redwolf501.top/gttzwpgxsr.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.chenzaomai.com/gtqldurdql.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.pycfn.com/gtscbndrkx.html

Ruby: "Hello, #{name}!"
来源：http://hz.cashguo.top/gtrchewuex.html

C#:   $"Hello, {name}!"
来源：http://hz.shanyushiyangkeji.top/gtzwznejwp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.guannengcc.top/gtzjjghvfc.html


<!-- 参考信息 -->