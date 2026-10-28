代发 wailian999

[U69] PHP：PDO 预处理
来源：http://hz.zycfv.cn/gtujzoowtt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hammf.cn/gtomewvmwv.html

[U70] PHP：PDO 事务
来源：http://hz.cucudq.cn/gtyzsxuoda.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.feifeiyinyue.top/gtqyfqbthw.html

[U71] PHP：抛出异常
来源：http://hz.aizwys.cn/gtbslecmhh.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinghuilouyu.cn/gtacqiqgvr.html

[U72] PHP：写错误日志
来源：http://hz.xingfuxueyuan.xyz/gtvobqjrup.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenlongwang.top/gtgfppqrol.html

[U73] PHP：读取 ini 配置
来源：http://hz.shanyushiyangkeji.top/gtlcgiwxzv.html

parse_ini_file("config.ini", true)
来源：http://hz.xinyue.icu/gttjcsckzv.html

[U74] PHP：读取环境变量
来源：http://hz.redwolf501.top/gtkahgaxtz.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jyoumei.cn/gtwphtusub.html

[U75] PHP：依赖注入
来源：http://hz.svipenyu.cn/gtpvxtwleg.html

composer require psr/container
来源：http://hz.xingfuxueyuan.xyz/gtmsnccnfy.html

[U76] PHP：简单路由
来源：http://hz.wangshuangyany.cn/gtvaounmre.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hammf.cn/gttvwhtwkj.html

[U77] PHP：模板渲染
来源：http://hz.zhoulong.xyz/gtluogqzkl.html

composer require twig/twig
来源：http://hz.wangshuangyany.cn/gtpmfjfaoz.html

[U78] PHP：单元测试
来源：http://hz.zhengqikj.top/gtzykwbjko.html

composer require --dev phpunit/phpunit
来源：http://hz.zhixingplan.top/gtbaoqyzmm.html

[U79] PHP：静态分析
来源：http://hz.chenzaomai.com/gtweyfcxkp.html

composer require --dev phpstan/phpstan
来源：http://hz.fzhhl.top/gtzmfgnxxm.html

[U80] PHP：代码规范修复
来源：http://hz.jiagoushi.top/gtgvfpnmbi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.redwolf501.top/gtmlybukum.html

[U81] JS：初始化项目
来源：http://hz.smart0.xyz/gtbbhkwxss.html

npm init -y;  npm i express
来源：http://hz.dianchejie.cn/gtfasjptjh.html

[U82] JS：package.json 脚本
来源：http://hz.zycfv.cn/gtnjvghmju.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yongpay.top/gtjbzuqtla.html

[U83] JS：ES Module 导入导出
来源：http://hz.smart0.xyz/gtivvzdojt.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yueranfly.top/gtxsvlxwuc.html

[U84] JS：CommonJS 写法
来源：http://hz.haohaochexian.top/gtukzzjyxl.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tian-w.cn/gtwecvuesf.html

[U85] JS：可选链
来源：http://hz.feifeiyinyue.top/gtevydfyph.html

a?.b?.c
来源：http://hz.jinyuanbaomall.cn/gtmiormcqr.html

[U86] JS：空值合并
来源：http://hz.jinghuilouyu.cn/gtkvnqltwd.html

a ?? b
来源：http://hz.kuanghao11.cn/gtbngmlknb.html

[U87] JS：解构默认值
来源：http://hz.yongpay.top/gtsremhbxd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhongyouzk.top/gtobunlbun.html

[U88] JS：对象展开合并
来源：http://hz.cucudq.cn/gtpleeexyk.html

{ ...a, ...b }
来源：http://hz.bjfxy.top/gtekxenblb.html

[U89] JS：数组去重
来源：http://hz.kuanghao11.cn/gtbkrfwauj.html

[...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gtinewjwnc.html

[U90] JS：数字数组排序
来源：http://hz.jyoumei.cn/gttaarjqrs.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtfpyknbsu.html

[U91] JS：对象键值遍历
来源：http://hz.jqgufenzy.top/gtkykhuhrn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shanyushiyangtech.top/gtutcagadb.html

[U92] JS：深拷贝
来源：http://hz.52xcode.cn/gtricasjmb.html

structuredClone(obj)
来源：http://hz.iojbl.cn/gtdrhkqjfs.html

[U93] JS：模板字符串
来源：http://hz.sufxvd.cn/gtxbjjbarg.html

`共 ${n} 条`
来源：http://hz.yj202588.top/gttovphdhg.html

[U94] JS：箭头函数
来源：http://hz.gzhubu.top/gtxxvltqyl.html

const double = x => x * 2;
来源：http://hz.ivvv.top/gtmwcgcbul.html

[U95] JS：Promise 包装
来源：http://hz.xinyue.icu/gtdgdvgpcu.html

new Promise((resolve, reject) => {})
来源：http://hz.quarkkingdee.top/gtsqiobmpk.html

[U96] JS：async/await 与异常
来源：http://hz.sxryk.cn/gttvxtlyxy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtddbjbazn.html

[U97] JS：并发请求
来源：http://hz.yangfankeji.com/gtlhpoqcht.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtxcymmejy.html

[U98] JS：fetch 带 JSON
来源：http://hz.yangfankeji.com/gtpkhgivuy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jinyuanbaomall.cn/gtfdmdihoz.html

[U99] JS：事件监听
来源：http://hz.feifeiyinyue.top/gtqnlvootg.html

el.addEventListener("click", e => {})
来源：http://hz.gotoacloud.top/gtmoargklg.html

[U100] JS：DOM 查询
来源：http://hz.cdnleiting.top/gtosrlwjqq.html

document.querySelector(".item")
来源：http://hz.xuetiantiany.cn/gtkelrldpg.html

[U101] JS：classList 操作
来源：http://hz.shanyushiyangtech.top/gtogkpucwb.html

el.classList.toggle("active")
来源：http://hz.jqgufenzy.top/gtgvcbayxf.html

[U102] JS：本地存储
来源：http://hz.zhiwuduotai.top/gtrjebxbbq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xylfe.cn/gteevxqdvr.html

[U103] JS：定时器
来源：http://hz.sweek.top/gtgebpwefg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinqigfzy.top/gtwztbvesw.html

[U104] JS：防抖
来源：http://hz.jlsjyb.cn/gtjseaomni.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtsgfoiojs.html

[U105] JS：节流
来源：http://hz.zdqjudy.top/gtdqsjduev.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ydzc1.top/gtvkemzmjq.html

[U106] JS：日期格式化
来源：http://hz.fengsongda.top/gtivccffnw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj202588.top/gtnbosyqha.html

[U107] JS：数字千分位
来源：http://hz.snrcjt.cn/gtqizefbek.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.kuanghao11.cn/gtawveumhe.html

[U108] JS：随机整数
来源：http://hz.quarkkingdee.top/gtptgenkgt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinqigfzy.top/gtcrfiqctr.html

[U109] JS：数组分组
来源：http://hz.zycfv.cn/gtuxpsztux.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xingfuxueyuan.xyz/gtolganemw.html

[U110] JS：数组分块
来源：http://hz.gaohongyu789.top/gttgjupneo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yueranfly.top/gtrjgrwona.html

[U111] JS：对象转 Map
来源：http://hz.zhiwuduotai.top/gthsarjpza.html

new Map(Object.entries(obj))
来源：http://hz.xinyue.icu/gtyicinzja.html

[U112] JS：字符串补位
来源：http://hz.smart0.xyz/gtgaygqywn.html

"7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtcebapdzj.html

[U113] JS：正则替换全部
来源：http://hz.fzhhl.top/gtasavhymn.html

s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtpmvawbby.html

[U114] JS：JSON 深比较
来源：http://hz.yanxiufei.cn/gtrtijsnzd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gtcxzbyqqb.html

[U115] JS：生成 UUID
来源：http://hz.yuxming.cn/gtrpeszzmx.html

crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gtzdlztzsf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinqigufen.top/gthacltsye.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cdnleiting.top/gtokvyrjqi.html

[U117] JS：单元测试
来源：http://hz.kuanghao11.cn/gtiwqnemkt.html

npm i -D vitest;  npx vitest
来源：http://hz.shangyingyoupin.top/gtvzucufjh.html

[U118] JS：开发服务器
来源：http://hz.zhiwuduotai.top/gttpogvaun.html

npm i -D vite;  npx vite
来源：http://hz.aizwys.cn/gthhyxfskn.html

[U119] JS：生产构建
来源：http://hz.yanxiufei.cn/gtrygcukfr.html

npx vite build
来源：http://hz.jinghuilouyu.cn/gtvgshjtwg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.aizwys.cn/gtniqstrxh.html

import.meta.env.VITE_API_URL
来源：http://hz.andypj.xyz/gtbitniwvv.html

================================================================================
来源：http://hz.nanxinkj.top/gtfxrzsnmg.html

统计汇总
来源：http://hz.cdnleiting.top/gtoyaxkywq.html

================================================================================
来源：http://hz.hywenlv.cn/gtetxfmtfp.html

按语言统计（条）：
来源：http://hz.hnxiangtu.top/gthbbeempg.html

Python ......... 252
来源：http://hz.shzxlz.cn/gtpbrsokof.html

PHP ............ 252
来源：http://hz.yuxming.cn/gtbiutaiwx.html

JavaScript ..... 252
来源：http://hz.chenjidiqi.icu/gtzftnxpai.html

TypeScript ..... 212
来源：http://hz.tanke756.top/gtsqmtdvkv.html

Java ........... 212
来源：http://hz.bjfxy.top/gtuewvekyj.html

Go ............. 212
来源：http://hz.zhoulong.xyz/gtrifgfkxy.html

Ruby ........... 212
来源：http://hz.smart0.xyz/gttzntvxbb.html

C# ............. 212
来源：http://hz.zhijiandao.cn/gtmbemyjnw.html

C .............. 30
来源：http://hz.ehwqpu.com/gtmrltzkjk.html

C++ ............ 30
来源：http://hz.vqdsnc.cn/gtezimkbvy.html

SQL ............ 90
来源：http://hz.hfpthk.cn/gtsdqrbjwj.html

Bash ........... 80
来源：http://hz.yj20258888.top/gtifsywizz.html

Kotlin ......... 15
来源：http://hz.guannengcc.top/gthktqfgow.html

Swift .......... 15
来源：http://hz.chenlongwang.top/gtbadoswde.html

Lua ............ 10
来源：http://hz.chenjidiqi.icu/gtygvmkrqx.html

Perl ........... 10
来源：http://hz.zhixingplan.top/gttptrjsoo.html

Scala .......... 10
来源：http://hz.snrcjt.cn/gtitugzafy.html

------------------------------------
来源：http://hz.quarkkingdee.top/gtsgixnxpc.html

合计 ........... 2106 条
来源：http://hz.gogol.net.cn/gtbepgrcsc.html

按章节统计：
来源：http://hz.chenlongwang.top/gtmkbowzqe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jyoumei.cn/gtzfdcscvc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gtxkmlzovm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinyuanbaomall.cn/gtibdpzhhg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yvedp.cn/gtswsykphv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ywan-chungtsiang.top/gtnjhbvwpy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtjaorqoib.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gtxljtzwss.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtnksmjmdu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtcatrmack.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yj202588.top/gtwooazeri.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtuphaijdu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtywlayfih.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtivcdqule.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhoulong.xyz/gtjouydpzr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.quarkkingdee.top/gtwjaxwkvu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtbmggfcvv.html

Q SQL 专题                              90
来源：http://hz.ehwqpu.com/gtuegtcodh.html

R Bash 专题                             80
来源：http://hz.pycfn.com/gtydcirtvu.html

S C / C++ 专题                          60
来源：http://hz.andypj.xyz/gtqcvksgdg.html

T 其他语言补充                          60
来源：http://hz.cdnleiting.top/gtsrwkinqz.html

U 高频实用片段                         120
来源：http://hz.ivvv.top/gttkeoocju.html

------------------------------------
来源：http://hz.yangfankeji.com/gtnbkztvwc.html

合计                                  2106 条
来源：http://hz.quarkkingdee.top/gtfsdkpped.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtlgchyjxp.html

使用提醒
来源：http://hz.tian-w.cn/gtefajzwgo.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtrawwjifd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.tanke756.top/gtypsiwrcu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhengqikj.top/gtzhunjnxn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.meibo888.top/gthkrgzgmo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yongpay.top/gtqskgpxck.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.wangshuangyany.cn/gthqlqqvru.html

—— 文件结束 ——
来源：http://hz.vqdsnc.cn/gthfutvnhp.html

================================================================================
来源：http://hz.yuanzhike.top/gtisctatto.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tian-w.cn/gtpobfwmvi.html

Common Programming Examples Cheat Book
来源：http://hz.pengpengdd.cyou/gtorzojrgy.html

================================================================================
来源：http://hz.ybcxt.top/gtoyqotufc.html

【收录内容】
来源：http://hz.zhijiandao.cn/gtgdoywiov.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jqgfzy.top/gtpijccpzn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhoulong.xyz/gtrepmlrdf.html

SQL · Bash · C · C++
来源：http://hz.wangdashe.top/gtxgwngeug.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydzc1.top/gthwjrvcsn.html

【使用说明】
来源：http://hz.nwbrower.top/gtcairbxjr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.tianlin.xyz/gtjvnyjfvy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zycfv.cn/gtbufewflp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.snrcjt.cn/gtkbapwmev.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.guannengcc.top/gtjmdaddzc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ywan-chungtsiang.top/gtwzhlweuq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhijiandao.cn/gtaqktrlrr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jlsjyb.cn/gtkaqfvnzc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.tanke756.top/gtqwuhfrcj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yanxiufei.cn/gtrkiyntjs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yj202588.top/gttdifshqf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zdqjudy.top/gtpbosrwdn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shanyushiyangtech.top/gtuxjhnjwi.html

【文件统计】
来源：http://hz.yangfankeji.com/gtitvkmytd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gogol.net.cn/gtvdmrutyf.html

--------------------------------------------------------------------------------
来源：http://hz.shangyingyoupin.top/gtqpcynxwe.html

目  录
来源：http://hz.zhiwuduotai.top/gtfsiaqaez.html

--------------------------------------------------------------------------------
来源：http://hz.guannengcc.top/gtolcxmdez.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shanyushiyangtech.top/gtsfxnuchj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj20258888.top/gtejrwdocm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.daxiang520.top/gtwvyemfeq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhengqikj.top/gtyceqdhxr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.fzhhl.top/gtqgzvumgp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yanxiufei.cn/gtxbrromqb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhaomingkeji.xyz/gtkpvddqfl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ivvv.top/gthtxptyoz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gtimkclrbz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.xziqi.cn/gtlfntehhn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtjjwuagjo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtcpcwjzlj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtieuerwqa.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.daxiang520.top/gtpuuvabrl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shuidangran.top/gtmakrlvvh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.316326.xyz/gtuorrtnjq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nanxinkj.top/gtqkmfydqi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.hammf.cn/gtwevbensz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yanxiufei.cn/gtanpuijec.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xingfuxueyuan.xyz/gttwtxilia.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhaomingkeji.xyz/gtdpdaslyh.html

================================================================================
来源：http://hz.kuanghao11.cn/gtrcexsemp.html

A. 基础语法与类型
来源：http://hz.hnxiangtu.top/gtlguuhvkj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttocrkoiz.html

[A01] Hello World
来源：http://hz.gotoacloud.top/gthsuqhmer.html

Py:   print("Hello, World!")
来源：http://hz.bjfxy.top/gtviduaiea.html

PHP:  echo "Hello, World!";
来源：http://hz.daxiang520.top/gtizrlsqtl.html

JS:   console.log("Hello, World!");
来源：http://hz.wangdashe.top/gtkymgyiao.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.tanke756.top/gtxntihitr.html

Java: System.out.println("Hello, World!");
来源：http://hz.jinyuanbaomall.cn/gtbrwuelve.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xingfuxueyuan.xyz/gtdjmbzcfa.html

Ruby: puts "Hello, World!"
来源：http://hz.xuanzx.com/gtbxgrobjr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.andypj.xyz/gtwkqimrrt.html

[A02] 变量声明与赋值
来源：http://hz.9152youxi.cn/gtqqhcdwui.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yonumen.top/gteftemevo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hammf.cn/gtvlunryuc.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.aibaodan.cn/gtipwhhwta.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhoulong.xyz/gtldpfjhtz.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.c1oappe.top/gtpkoxugbd.html

Go:   name := "Alex"; age := 20
来源：http://hz.zycfv.cn/gtffmsorpz.html

Ruby: name = "Alex"; age = 20
来源：http://hz.c1oappe.top/gtdpxvxpmx.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.nwbrower.top/gtvqcvgqxa.html

[A03] 常量定义
来源：http://hz.haohaochexian.top/gtyxvxzqdk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhoulong.xyz/gtmcobrukj.html

PHP:  const PI = 3.14159;
来源：http://hz.redwolf501.top/gtwvvhwylp.html

JS:   const PI = 3.14159;
来源：http://hz.yueranfly.top/gtinpxhwpv.html

TS:   const PI: number = 3.14159;
来源：http://hz.hnxiangtu.top/gttiqqxxex.html

Java: static final double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtevadxnjq.html

Go:   const PI = 3.14159
来源：http://hz.xylfe.cn/gtovikorov.html

Ruby: PI = 3.14159
来源：http://hz.nanxinkj.top/gtlpstqtnt.html

C#:   const double PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtmnidgtef.html

[A04] 判断变量类型
来源：http://hz.quarkkingdee.top/gtdalsxkwb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yj202588.top/gtxenahrzd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jinqigfzy.top/gtycdqkrmx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.pycfn.com/gtifzwlghf.html

TS:   typeof x; x instanceof Date
来源：http://hz.chenlongwang.top/gtqodtmasq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.kuanghao11.cn/gtqgfjiuqr.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yonumen.top/gtfjgyxsti.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.chenjidiqi.icu/gtzvcpaufq.html

C#:   x.GetType().Name; x is int
来源：http://hz.ydjk.org.cn/gtchotxxhx.html

[A05] 整数除法与取模
来源：http://hz.pengpengdd.cyou/gtymrkaxiv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.xylfe.cn/gthvgzlqvt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.gaohongyu789.top/gtbdboyvzo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.havefunace.top/gtzfudtytq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhongyouzk.top/gtajcaxfjs.html

Java: 7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtsnmbzwjv.html

Go:   7 / 2; 7 % 2
来源：http://hz.316326.xyz/gtywxxvolc.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.cashguo.top/gtvxvfbvei.html

C#:   7 / 2; 7 % 2
来源：http://hz.zdqjudy.top/gtlmbtlfih.html

[A06] 字符串转数字
来源：http://hz.zhijiandao.cn/gtlsquhhvj.html

Py:   int("42"); float("3.14")
来源：http://hz.aizwys.cn/gtmezksisq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jinqigufen.top/gtizenkqqn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.shanyushiyangkeji.top/gtyrqbppzn.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cqqwz.cn/gtsyhfjfzw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.xylfe.cn/gtiohzavdn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jinyuanbaomall.cn/gtvgrwpfrj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.svipenyu.cn/gtpjsgcmpl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hnqzz.top/gtwjzfwmpq.html

[A07] 数字转字符串
来源：http://hz.zdqjudy.top/gtppymlhlo.html

Py:   str(42)
来源：http://hz.yueranfly.top/gtvjukyvui.html

PHP:  (string) 42; strval(42)
来源：http://hz.jyoumei.cn/gtnxzrqrrs.html

JS:   String(42); (42).toString()
来源：http://hz.0kj1m.cn/gthshabsby.html

TS:   String(42)
来源：http://hz.52xcode.cn/gtnwbjiqcc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.chenzaomai.com/gtmxmgbtiy.html

Go:   strconv.Itoa(42)
来源：http://hz.jianghu66.top/gtumsuffyj.html

Ruby: 42.to_s
来源：http://hz.cucudq.cn/gtjzyvjtnd.html

C#:   42.ToString()
来源：http://hz.jinghuilouyu.cn/gtlznhvcjf.html

[A08] 取整与四舍五入
来源：http://hz.yonumen.top/gttsgfdthn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.fzhhl.top/gtgqcycmrw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhongyouzk.top/gtthaonotq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yonumen.top/gtcrxnknfv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.hysaishi.cn/gtpxcjmczu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.guowangkeji.top/gtqcaiaqxw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.shanyushiyangkeji.top/gtgsjpcreb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.xuanzx.com/gtmncondqf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.cdnleiting.top/gteegssuka.html

[A09] 绝对值与最大最小值
来源：http://hz.havefunace.top/gtwmugbddy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhixingplan.top/gtcuokuuoy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yueranfly.top/gttvbwixmr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yanxiufei.cn/gtjmcabnan.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.pengpengdd.cyou/gtwewlutlp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhijiandao.cn/gtvazidmat.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.nwbrower.top/gtpimdhbgv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.cashguo.top/gttemthrcv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yueranfly.top/gtgizqezoe.html

[A10] 生成随机数
来源：http://hz.gzhubu.top/gthnruxedk.html

Py:   import random; random.randint(1, 100)
来源：http://hz.nanxinkj.top/gtfptfwlre.html

PHP:  random_int(1, 100);
来源：http://hz.fzhhl.top/gtmbgjrezo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jlsjyb.cn/gtsdjgtzhg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.bjfxy.top/gtvxjumwgc.html

Java: new Random().nextInt(100) + 1
来源：http://hz.jinqigfzy.top/gtlqeewhdk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.shanyushiyangtech.top/gtgmcajvvf.html

Ruby: rand(1..100)
来源：http://hz.cdnleiting.top/gtbmbazsvi.html


<!-- 参考信息 -->