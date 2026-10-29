代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gvozrrbfi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gegqgxeaj.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gdmqpoeeg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gxxtylicx.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gnjhgxrvq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gkraizeft.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gxmgniehn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/godysfntj.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gxdkanrsb.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gkstspyan.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gqyuyzyzy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gdlbaizzk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gxxqskoqu.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/ggttcgnlq.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gcjvmfmck.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gbvfdlatl.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gwojoofke.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gogopyskn.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gjjnfhflk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gsxyhnmli.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gxpqigkpi.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/ggtnripyg.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/govlktfqi.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/grjnqtlqa.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/giaafwweq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/grfybukoc.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gmlevabny.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gkzzhwhxf.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gwuxfnmnd.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gsoomnmjo.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gcnejdqjb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gmshdkspi.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gkqcfoyeq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gakfuxnoz.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gdyzdwthz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/grbjvknds.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gctsaggcq.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gxgvipyig.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gunnziwli.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gdxnkszdd.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gsigsdzkt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gjxfaadqo.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gfvdbczmm.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gpulksmde.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gwfkqakfg.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/ggzfmrlnz.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnbpsugvs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/ghhwlbusl.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/geqiqtbjw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gnypjweot.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gfvtuwpjp.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghizmejqz.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwbstnnpf.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gkbhhsyrc.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gzbgmjwow.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gklafyvmk.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gzkfofzyh.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gwvipnlnr.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gqvjtnjak.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gquvnzedd.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gshbpuwzk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gaycgtqtw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gtdfeinzc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gxsorpiln.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gprycdvin.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gzhhvfbki.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/geimltkgn.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gbikseqqy.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/glxwuwhfi.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gnviqydyc.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gsfdlypbu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gsfvrupik.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gkylpqtwk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gculrcifh.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/geotrpbba.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/glkamjqew.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/ghhmhgmzf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/givgxyhoi.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gtkhclimg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/ghehttekw.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gpzkgyzif.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/geelpoaee.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gzpjqutse.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gflkoloqd.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/giusopsdj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/grfvotjtu.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/ginzcipap.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/ghyrftwxp.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/ggrqtxlrx.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gscrqcdxz.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gckrcstgf.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gunxxwkuu.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gshcbkqqh.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/guhfsyemw.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gsmancfkj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/ggvfyymey.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gsevsdmed.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gkozclxyx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/glsiwpprs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gmpajsmyv.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gdthzoxrf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gwwrihlqa.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gxjvulutv.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gfgszqvql.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gfqljgnhs.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/geiezbssv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gcinblrba.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gzbcklpsi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpqrcrpyn.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gicakxxbe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gagivslwc.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gxacvgrcm.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gvckzaxnv.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gqvbwsvqk.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gobvluatb.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/ggkpwrjaf.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/galpimkls.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gazgmkspx.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gvtaqhktz.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gimfupccn.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gsgkegpuc.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gzuustxba.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gxnldzjbk.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gzvekhzfb.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gydpshppn.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gmtlejwis.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gsvsifusw.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/glgsnwodu.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gavgyobzm.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gywmvuysh.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/ghpcakavf.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gtmdzopbp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gqwpagbhi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/ghevprore.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gozioyjgk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gdzqlenkb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gdodsmkpp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gexulpezs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gayphhabg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/genuseyzc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/glxqpfjny.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gkjwqdfxy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/goifgyplb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gpgtdvygz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gezyaxdux.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/golrsexxy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/giildvlgb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gxkysrule.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gpbfitbqw.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gmuwvxrpz.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gdxasaunh.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gpsxjasof.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gumcsnqrb.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gdnilihjk.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/grqvorhxw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gpogepkdc.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/guiueopzj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gkzsltfwm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gsidpjnez.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gbbutxzfz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/ghdmwgytd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gtfynxmjj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gbasdzxiz.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gdnwdpqts.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjmowcmpb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gzoeimebw.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gtzszugyg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gejceupew.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gmuztwkmy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gahukgsax.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gixchxvrx.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gnitmdqzz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gfihscvyl.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gxcfqhlxh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gcgalylwn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gtxbhjlba.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/glmebvyqp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gjvmucepg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gbpuupfmq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gzxauulkw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/ggmakzwji.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gbnjqryjf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gfwlvowpi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gaabbrdho.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gbnandqfd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gwomafruq.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gqgkoreuz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gbsokkosv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gtvlwmhts.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/ggjdjgceb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gewygcwue.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gskrmkjua.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gnhmhdljx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/ghbwnxwfb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdjuixplf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/guqrihxaa.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gjnzgkewi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gsoqudmfh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gbexeqchf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcspamhve.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gpthfckuz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ghtltjcye.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/goteanwwc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkpwdpctb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/ghqlurdhz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gwwkraupf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gvaxmkdlw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gxruopuhm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glfhjmvho.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gftgkmlwf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gkngeiedj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpqkakplm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyphkjxyj.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gzuoblspm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjctldiad.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gyvhlasvt.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gqgrtnygt.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/ghpxlrgsp.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gdrymrknh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/grogjerjw.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/ghbrcdeii.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gcrigrfao.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gbsroyyqo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gwincaxuf.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gjzlfxeqr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/ghchcpssj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gevcxyiql.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gaqibcezo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gsnmntfdo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gbmftwumf.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gfjplafew.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/ggseyvbvm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gxtqrznjy.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/ggbrqbaun.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/ggnjzfjnz.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gncurpnoy.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjonwwzoo.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gswzfqgzk.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gpbnvvhnv.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gwzoipmkg.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gxscaqyqs.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gajmaxmet.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/goluwxfkf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gwqzkwnrj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gnkyvkcun.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gpyhztaqx.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gayjufeuz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gznknbgnn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gmbdcwpwo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gewdijhoq.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gcgjzzpbh.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gfldatiea.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/getaidcmd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gbztvradc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gilmcqorf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gkldycqyf.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gystbsabd.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/ggsxsysrl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/grewdfvtd.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gujzjkccf.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gcqadbdbi.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gwrquufxe.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gubqzpsaa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gkivndfhg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gisyupdws.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gfixggnht.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/glsewjovs.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gmmhczhip.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gekafmain.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gkozcffwx.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/ghutrxrjs.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gejnilrid.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gkhlleyzj.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gonsqgphg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/ggyobokfk.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gyvtzvnxl.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gbvefvfby.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/goyyevfki.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/grhxvmyne.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvanilns.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gnuowqypk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcabeouz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/gmsisqchy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/ghvcbuaea.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gqkbtnwxp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/ggqywpjza.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/grqtypsgq.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/gwkrbgchh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gztcdexog.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gcvofkexh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gdvvxtzbz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtxigbayk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/grbcrvdng.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fehbvm.com/Article/details/ghxizinis.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.hesvh.cn/Article/details/gdhobefpb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gpvgydehp.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/gxwuzphde.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gqynjxfze.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/goeodtqee.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtbzvspmp.sHtML


<!-- 参考信息 -->