代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.yj20258.top/gtntrcvxqf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.tianlin.xyz/gtflsnmpds.html

[U68] PHP：PDO 连接
来源：http://hz.chenzaomai.com/gtomeeuziq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.andypj.xyz/gtlnktmazp.html

[U69] PHP：PDO 预处理
来源：http://hz.yj202588.top/gttxzuepuu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zdqjudy.top/gtpynatirn.html

[U70] PHP：PDO 事务
来源：http://hz.yonumen.top/gtevzykimt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jyoumei.cn/gttgbwgavr.html

[U71] PHP：抛出异常
来源：http://hz.redwolf501.top/gtmfqekqwl.html

throw new RuntimeException("失败", 500);
来源：http://hz.cqqwz.cn/gtixgyhvlh.html

[U72] PHP：写错误日志
来源：http://hz.tanke756.top/gttmlfkdog.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gogol.net.cn/gtiaocmwrn.html

[U73] PHP：读取 ini 配置
来源：http://hz.yvedp.cn/gtaobwsupg.html

parse_ini_file("config.ini", true)
来源：http://hz.quarkkingdee.top/gtgqxmiuoj.html

[U74] PHP：读取环境变量
来源：http://hz.aibaodan.cn/gtlssackbe.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xylfe.cn/gtxfrvkdsa.html

[U75] PHP：依赖注入
来源：http://hz.cashguo.top/gtmszbphxp.html

composer require psr/container
来源：http://hz.aizwys.cn/gtegkmmifq.html

[U76] PHP：简单路由
来源：http://hz.pengpengdd.cyou/gtzsivdhee.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.pengpengdd.cyou/gtyxajftpf.html

[U77] PHP：模板渲染
来源：http://hz.xuetiantiany.cn/gtkzlctnnv.html

composer require twig/twig
来源：http://hz.hnqzz.top/gtpqvtlmxs.html

[U78] PHP：单元测试
来源：http://hz.cashguo.top/gtnzhawgml.html

composer require --dev phpunit/phpunit
来源：http://hz.xingfuxueyuan.xyz/gttqfqohep.html

[U79] PHP：静态分析
来源：http://hz.dianchejie.cn/gtynvbluwh.html

composer require --dev phpstan/phpstan
来源：http://hz.fengsongda.top/gtljjwrjwy.html

[U80] PHP：代码规范修复
来源：http://hz.shzxlz.cn/gtmjjzajhm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.quarkkingdee.top/gtnaeaiklo.html

[U81] JS：初始化项目
来源：http://hz.zhengqikj.top/gtstmhfnrj.html

npm init -y;  npm i express
来源：http://hz.316326.xyz/gtxkkykpxk.html

[U82] JS：package.json 脚本
来源：http://hz.andypj.xyz/gtyeshldsl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.fzhhl.top/gtcsyyxjdv.html

[U83] JS：ES Module 导入导出
来源：http://hz.gogol.net.cn/gtmrtapizp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.guowangkeji.top/gthbdlwtkb.html

[U84] JS：CommonJS 写法
来源：http://hz.nwbrower.top/gtrvupepro.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinghuilouyu.cn/gthfihrnnk.html

[U85] JS：可选链
来源：http://hz.xinyue.icu/gtqbozwtln.html

a?.b?.c
来源：http://hz.meibo888.top/gtvepyknqo.html

[U86] JS：空值合并
来源：http://hz.pengpengdd.cyou/gtlnliumks.html

a ?? b
来源：http://hz.fengsongda.top/gtuxegyaey.html

[U87] JS：解构默认值
来源：http://hz.redwolf501.top/gtdvnybwql.html

const { a = 1, b = 2 } = obj;
来源：http://hz.chenlongwang.top/gtsbjuhdsl.html

[U88] JS：对象展开合并
来源：http://hz.yongpay.top/gthvncihkr.html

{ ...a, ...b }
来源：http://hz.hywenlv.cn/gtzhsoppsi.html

[U89] JS：数组去重
来源：http://hz.shanyushiyangtech.top/gtmkbusyqm.html

[...new Set(arr)]
来源：http://hz.iojbl.cn/gtrwsqudzz.html

[U90] JS：数字数组排序
来源：http://hz.hysaishi.cn/gtxjsfhwga.html

[...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtkzzbumoq.html

[U91] JS：对象键值遍历
来源：http://hz.hongshengwenyu.top/gtpqzeltgx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xuetiantiany.cn/gtoeihdxkv.html

[U92] JS：深拷贝
来源：http://hz.havefunace.top/gtxcwrnunm.html

structuredClone(obj)
来源：http://hz.yongpay.top/gttplkxcas.html

[U93] JS：模板字符串
来源：http://hz.sufxvd.cn/gtpbdjrewq.html

`共 ${n} 条`
来源：http://hz.quarkkingdee.top/gtyuemkvzw.html

[U94] JS：箭头函数
来源：http://hz.cheryme.top/gtrnvesgkc.html

const double = x => x * 2;
来源：http://hz.zhixingplan.top/gtxxggjpum.html

[U95] JS：Promise 包装
来源：http://hz.jinghuilouyu.cn/gtkfucolub.html

new Promise((resolve, reject) => {})
来源：http://hz.yonumen.top/gtroimldpd.html

[U96] JS：async/await 与异常
来源：http://hz.yangfankeji.com/gtvuncfvkd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.0kj1m.cn/gtoctynpjw.html

[U97] JS：并发请求
来源：http://hz.yangfankeji.com/gtrxguvsof.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtkzwelhpa.html

[U98] JS：fetch 带 JSON
来源：http://hz.shzxlz.cn/gteqqvjgxd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gotoacloud.top/gtkolsyedb.html

[U99] JS：事件监听
来源：http://hz.xuanzx.com/gtygvwcldp.html

el.addEventListener("click", e => {})
来源：http://hz.zhixingplan.top/gtohllrvye.html

[U100] JS：DOM 查询
来源：http://hz.xuanzx.com/gtsmdcethe.html

document.querySelector(".item")
来源：http://hz.yuxming.cn/gtgmermehm.html

[U101] JS：classList 操作
来源：http://hz.dashuyun.cn/gtntndvbdv.html

el.classList.toggle("active")
来源：http://hz.c1oappe.top/gtwnpgdftd.html

[U102] JS：本地存储
来源：http://hz.quarkkingdee.top/gtgvxfirxi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yongpay.top/gtutocuhwx.html

[U103] JS：定时器
来源：http://hz.hfpthk.cn/gtbuufxwlb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.guannengcc.top/gtuclhxven.html

[U104] JS：防抖
来源：http://hz.ehwqpu.com/gtxtcfdtzm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtgtgmvbgn.html

[U105] JS：节流
来源：http://hz.jlsjyb.cn/gtjydljlng.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenzaomai.com/gtnxkcxxia.html

[U106] JS：日期格式化
来源：http://hz.jqgfzy.top/gtpczbdxok.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.wangdashe.top/gtjwqvkzta.html

[U107] JS：数字千分位
来源：http://hz.shanyushiyangkeji.top/gttgjvinzk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nanxinkj.top/gtdshfaadn.html

[U108] JS：随机整数
来源：http://hz.zhongyouzk.top/gtardoneeo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.gotoacloud.top/gtfxywjckw.html

[U109] JS：数组分组
来源：http://hz.feifeiyinyue.top/gtjskkgemo.html

Object.groupBy(arr, x => x.type)
来源：http://hz.nanxuanxn.top/gtgcxezxhv.html

[U110] JS：数组分块
来源：http://hz.9152youxi.cn/gtucqabpgx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zdqjudy.top/gtlhqjxixo.html

[U111] JS：对象转 Map
来源：http://hz.hongshengwenyu.top/gtdxvygfqw.html

new Map(Object.entries(obj))
来源：http://hz.zhoulong.xyz/gtsshlquhc.html

[U112] JS：字符串补位
来源：http://hz.bjfxy.top/gtqhhdbpft.html

"7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtqjndczsk.html

[U113] JS：正则替换全部
来源：http://hz.svipenyu.cn/gtmsozfcau.html

s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtcpumbujh.html

[U114] JS：JSON 深比较
来源：http://hz.zycfv.cn/gtheakhich.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gtjyeryyqi.html

[U115] JS：生成 UUID
来源：http://hz.jqgfzy.top/gtccdkfsfw.html

crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gtnlbkrdth.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.vqdsnc.cn/gtssgygibc.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xuanzx.com/gtiaebvkqt.html

[U117] JS：单元测试
来源：http://hz.sxryk.cn/gtmbkqtlxy.html

npm i -D vitest;  npx vitest
来源：http://hz.hfpthk.cn/gtwpzrnjlx.html

[U118] JS：开发服务器
来源：http://hz.quarkkingdee.top/gtdadjflnb.html

npm i -D vite;  npx vite
来源：http://hz.ivvv.top/gtvoiqkhis.html

[U119] JS：生产构建
来源：http://hz.cucudq.cn/gtbrhwkmcq.html

npx vite build
来源：http://hz.cashguo.top/gtjinfowyb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhijiandao.cn/gtbqpmnbkf.html

import.meta.env.VITE_API_URL
来源：http://hz.yonumen.top/gtjbzbvstf.html

================================================================================
来源：http://hz.jinqigufen.top/gtpfdvupoh.html

统计汇总
来源：http://hz.xingfuxueyuan.xyz/gtxluohigj.html

================================================================================
来源：http://hz.xylfe.cn/gtsfmkeymc.html

按语言统计（条）：
来源：http://hz.snrcjt.cn/gtlxljpncr.html

Python ......... 252
来源：http://hz.wangshuangyany.cn/gtbuxvnpkf.html

PHP ............ 252
来源：http://hz.ybcxt.top/gtozvbthaq.html

JavaScript ..... 252
来源：http://hz.svipenyu.cn/gtksntpebm.html

TypeScript ..... 212
来源：http://hz.guowangkeji.top/gttygtlqqr.html

Java ........... 212
来源：http://hz.fzhhl.top/gtkvuvssxn.html

Go ............. 212
来源：http://hz.daria6918.cn/gtzabmaznc.html

Ruby ........... 212
来源：http://hz.jqgfzy.top/gtbvorugly.html

C# ............. 212
来源：http://hz.yangfankeji.com/gttyjenpgi.html

C .............. 30
来源：http://hz.iojbl.cn/gtdyytvmms.html

C++ ............ 30
来源：http://hz.fzhhl.top/gthhfhxeft.html

SQL ............ 90
来源：http://hz.dianchejie.cn/gtqiojughv.html

Bash ........... 80
来源：http://hz.jinqigfzy.top/gtplkmcsnv.html

Kotlin ......... 15
来源：http://hz.yuanzhike.top/gtsbxxijlz.html

Swift .......... 15
来源：http://hz.daxiang520.top/gtmgztxfre.html

Lua ............ 10
来源：http://hz.havefunace.top/gtgysauzga.html

Perl ........... 10
来源：http://hz.sysykeji.top/gtmwxzbmti.html

Scala .......... 10
来源：http://hz.hysaishi.cn/gtwicesuiv.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gttbszboww.html

合计 ........... 2106 条
来源：http://hz.xuanzx.com/gtmlxdyysb.html

按章节统计：
来源：http://hz.zhaomingkeji.xyz/gtewvqddrx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.vqdsnc.cn/gtpablfxmn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ppjwa.cn/gtcidgxemp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gtgepqsani.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cdnleiting.top/gttrqfdytd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.andypj.xyz/gtdesbkzdw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.pengpengdd.cyou/gttziaizhp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gttgpvqhpr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xuanzx.com/gtodwoqroz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtggtuxcyw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gotoacloud.top/gtciiktztu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gteijguebn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtfvftcnnz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtyyytkbvi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yuxming.cn/gtwjyuewzj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.pengpengdd.cyou/gtoeuabwmi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtvgdxradp.html

Q SQL 专题                              90
来源：http://hz.hnqzz.top/gthgptttou.html

R Bash 专题                             80
来源：http://hz.dianchejie.cn/gtapcjewef.html

S C / C++ 专题                          60
来源：http://hz.jinqigufen.top/gtistjjgxd.html

T 其他语言补充                          60
来源：http://hz.ydzc1.top/gtqzqxbqjf.html

U 高频实用片段                         120
来源：http://hz.wangshuangyany.cn/gtbgoxhcnc.html

------------------------------------
来源：http://hz.vqdsnc.cn/gtxqsanyjt.html

合计                                  2106 条
来源：http://hz.sweek.top/gtstutmpaf.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtxyldhmss.html

使用提醒
来源：http://hz.hongshengwenyu.top/gtfgpixtbj.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gtfuvrnwdh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sweek.top/gtvaaudvyj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.dashuyun.cn/gtyqjgpyxm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj202588.top/gtdxxygkzx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gogol.net.cn/gtluwriouv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cheryme.top/gtxdckouys.html

—— 文件结束 ——
来源：http://hz.svipenyu.cn/gtlmxkxdbc.html

================================================================================
来源：http://hz.cqqwz.cn/gtpredwngc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.chenlongwang.top/gtibnjoxww.html

Common Programming Examples Cheat Book
来源：http://hz.pengpengdd.cyou/gtofkyjnnb.html

================================================================================
来源：http://hz.gogol.net.cn/gtljbtxdpj.html

【收录内容】
来源：http://hz.smart0.xyz/gtzqihhtfq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.meibo888.top/gtmjglobmw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.hnxiangtu.top/gtxwupkrcc.html

SQL · Bash · C · C++
来源：http://hz.ppjwa.cn/gtnigorsgg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydzc1.top/gteedffbcx.html

【使用说明】
来源：http://hz.yonumen.top/gtmprlnges.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.chenzaomai.com/gtbkopjpme.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jinghuilouyu.cn/gtiovewzkt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258.top/gtblbfjjic.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cdnleiting.top/gtoyamwxpt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.guowangkeji.top/gtbhasokol.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.wangshuangyany.cn/gtfkiniouf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.chenlongwang.top/gtjjtlhmke.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yj202588.top/gtvbucjyxd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.mhx1999.top/gtrfrhntml.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhiwuduotai.top/gtnmpzffvg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ppjwa.cn/gtcmohthoy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.redwolf501.top/gtixmjlxfm.html

【文件统计】
来源：http://hz.chenlongwang.top/gtnbiyfgcq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yueranfly.top/gthxsedpfp.html

--------------------------------------------------------------------------------
来源：http://hz.daria6918.cn/gtedestzhd.html

目  录
来源：http://hz.zdqjudy.top/gtqgsyewxk.html

--------------------------------------------------------------------------------
来源：http://hz.dashuyun.cn/gtclenqbek.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zdqjudy.top/gtztbkgzha.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.smart0.xyz/gtbddlrihm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jinyuanbaomall.cn/gtrlloipsr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.nanxuanxn.top/gtlcbvibrf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.vqdsnc.cn/gtfvucxoke.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hfpthk.cn/gthhdqrbgc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yueranfly.top/gtfbagxlof.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shuidangran.top/gtivvmrxxv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtjrhdgdqz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jqgufenzy.top/gteuhqgxxw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gtooblblcl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtoczexkoc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtriskttep.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yanxiufei.cn/gtplicgbkp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.tanke756.top/gtirpitxfb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtzqfznxyi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.smart0.xyz/gtkhoajwwa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.hnxiangtu.top/gtjwlcpqxo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.aizwys.cn/gthiaekfop.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hfpthk.cn/gtmnrbgmto.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.316326.xyz/gttmrohmqb.html

================================================================================
来源：http://hz.shuidangran.top/gtcdkagpfv.html

A. 基础语法与类型
来源：http://hz.xylfe.cn/gtboqgxzon.html

================================================================================
来源：http://hz.cashguo.top/gtzrzacsas.html

[A01] Hello World
来源：http://hz.316326.xyz/gtaxkxwcre.html

Py:   print("Hello, World!")
来源：http://hz.nanxuanxn.top/gthrwmnoot.html

PHP:  echo "Hello, World!";
来源：http://hz.snrcjt.cn/gtapgsteau.html

JS:   console.log("Hello, World!");
来源：http://hz.jlsjyb.cn/gtxtdiqjhf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.iojbl.cn/gtojalvybv.html

Java: System.out.println("Hello, World!");
来源：http://hz.yuanzhike.top/gtagqgtmaj.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yanxiufei.cn/gtaqkcrsdm.html

Ruby: puts "Hello, World!"
来源：http://hz.hnqzz.top/gtpbsbxtbd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.gaohongyu789.top/gtefeukpre.html

[A02] 变量声明与赋值
来源：http://hz.shanyushiyangtech.top/gtfyteodlp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ppjwa.cn/gtapqtyvpy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.tanke756.top/gtlhpckrhz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yj20258888.top/gtamfnfjdw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.cdnleiting.top/gtjszvnlss.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hnqzz.top/gtwdihehrr.html

Go:   name := "Alex"; age := 20
来源：http://hz.gotoacloud.top/gtcmhbxgub.html

Ruby: name = "Alex"; age = 20
来源：http://hz.shanyushiyangkeji.top/gtqpmycwgl.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.redwolf501.top/gtpaaflwwd.html

[A03] 常量定义
来源：http://hz.jinqigfzy.top/gtqgofnnae.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.aizwys.cn/gtzitdorsl.html

PHP:  const PI = 3.14159;
来源：http://hz.sysykeji.top/gtxihfuvfv.html

JS:   const PI = 3.14159;
来源：http://hz.chenlongwang.top/gtmnhorgri.html

TS:   const PI: number = 3.14159;
来源：http://hz.yuanzhike.top/gtehizwfda.html

Java: static final double PI = 3.14159;
来源：http://hz.52xcode.cn/gtjtrfudfz.html

Go:   const PI = 3.14159
来源：http://hz.zhaomingkeji.xyz/gtprsxwxmn.html

Ruby: PI = 3.14159
来源：http://hz.sweek.top/gteftgimci.html

C#:   const double PI = 3.14159;
来源：http://hz.jianghu66.top/gtkrttgydk.html

[A04] 判断变量类型
来源：http://hz.nanxinkj.top/gthoeyokbk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinqigfzy.top/gtbnkntzmz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.fengsongda.top/gtxcplnsbv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.tanke756.top/gtvlkpqdgu.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinqigfzy.top/gtxbiiuepo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ppjwa.cn/gtcrhlhref.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.nanxinkj.top/gtlsjmcfxo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.vqdsnc.cn/gtpleogron.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhongyouzk.top/gtcqtfdbyi.html

[A05] 整数除法与取模
来源：http://hz.xuanzx.com/gtnnbcyqqr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yangfankeji.com/gtkpdmeaph.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhixingplan.top/gtyeqaomxu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nanxinkj.top/gtdjxkakpi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.snrcjt.cn/gtyudcreja.html

Java: 7 / 2; 7 % 2
来源：http://hz.jqgfzy.top/gtsuffjqii.html

Go:   7 / 2; 7 % 2
来源：http://hz.nanxinkj.top/gthqloqtfy.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtvmhvybop.html

C#:   7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtgwdiujaj.html

[A06] 字符串转数字
来源：http://hz.zhengqikj.top/gtvmlhahob.html

Py:   int("42"); float("3.14")
来源：http://hz.yanxiufei.cn/gtaxniprbw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhixingplan.top/gtowobdamf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.meibo888.top/gtwmrimvbr.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.shzxlz.cn/gtowdlyyxq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.tanke756.top/gtlgcagxxi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ybcxt.top/gtcgkbihnx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yonumen.top/gtbfertbvx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.cdnleiting.top/gtynexeiah.html

[A07] 数字转字符串
来源：http://hz.zhijiandao.cn/gtecqkzaao.html

Py:   str(42)
来源：http://hz.nanxuanxn.top/gtuemnzhfd.html

PHP:  (string) 42; strval(42)
来源：http://hz.chenzaomai.com/gtolnowoih.html

JS:   String(42); (42).toString()
来源：http://hz.gaohongyu789.top/gtresrzgpa.html

TS:   String(42)
来源：http://hz.jinqigfzy.top/gtpeeitflk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shangyingyoupin.top/gtuolkqyys.html

Go:   strconv.Itoa(42)
来源：http://hz.52xcode.cn/gtugeppsem.html

Ruby: 42.to_s
来源：http://hz.yvedp.cn/gtsbvkeaiy.html

C#:   42.ToString()
来源：http://hz.yonumen.top/gtoupqscal.html

[A08] 取整与四舍五入
来源：http://hz.smart0.xyz/gtgflhevbm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.hnxiangtu.top/gtvlsbpecv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.tian-w.cn/gtzykwzaxr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.smart0.xyz/gtntgoorfu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.kuanghao11.cn/gterzpzccd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.hammf.cn/gtnrobkqkt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.daria6918.cn/gtyxpnafbe.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.ivvv.top/gtippcexjq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.cucudq.cn/gtchhcwtmr.html

[A09] 绝对值与最大最小值
来源：http://hz.zhengqikj.top/gtjxaeijbp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.tian-w.cn/gtllazinhw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shuidangran.top/gtmvzthdup.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hfpthk.cn/gtmsnhdyvu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhaomingkeji.xyz/gtqrlpvmvn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.daria6918.cn/gtjqcxmgsl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.smart0.xyz/gtgjxbiikh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.chenlongwang.top/gtrsefkjxq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zhixingplan.top/gtcnszuvgx.html

[A10] 生成随机数
来源：http://hz.smart0.xyz/gtugcjsqog.html

Py:   import random; random.randint(1, 100)
来源：http://hz.fzhhl.top/gtdrixdyub.html

PHP:  random_int(1, 100);
来源：http://hz.sufxvd.cn/gtigdymiio.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shzxlz.cn/gtdptavcck.html


<!-- 参考信息 -->