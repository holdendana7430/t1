代发 wailian999

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/geagpcksi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gtiegkawb.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/geguhztux.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gtlyjoggt.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gnxdrktee.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gkwtezmbw.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gkiagusuu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gbytipucm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gqscwfybm.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gruoqfuvc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gbghiojzo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gcorocftm.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gaabwmvrh.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gnpelolzj.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gwnyfiuut.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/grztumwny.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gdsaxcnvt.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gpciqfkjg.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gvlcponsh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/ggnthkdxx.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gjqrckqsc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/ghlulweba.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gaxmxwfsp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gbyxmcwak.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/goiyzubhk.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gclnugiuy.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gzkiolnkb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gdojmfpeo.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gbmacjypx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gberzbhlx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/graarjjit.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gagyrscxu.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gqhmxjkby.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/geaimoukr.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/ghdfphcjn.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/ggvprwcoh.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gnznurtvl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gnomyyupp.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gjqjvzwpe.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gkjuyxqvd.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/guswogpsv.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gsmuyyevl.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gqpbzgwvy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gewezhdpc.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gupcomfso.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/giswttckf.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gtcjmwmex.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ghzwcfrqy.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gphlxkxud.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gxxzzjfhx.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gksispswe.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gdburtxdi.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gyivorykr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gkxzwwroj.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gbxwqytis.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gcfgbllxl.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/goeztiqoh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gdgacjtxw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/grhtfqmja.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gwmgzklag.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gaeyhhjqd.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gvcavyxjx.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gbtnvyafs.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/greieppbx.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gpqxoaxgd.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gajeegefa.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/ghwrarafd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gnsapvyvt.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gqkpcszan.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gxlvghydf.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gnvcyzqul.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gpaeqrigr.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gxboufsqg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gibjitdye.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gdbkcialo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gkdtbuzlz.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gdrqpehhz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbrfikuq.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gbeogxrfd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gjmfcdsjv.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gxewucxcx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gbngzfabi.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gygwacpgi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gktpedohx.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/geppsphgr.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/guofjnklm.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gciedydcw.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/ggvqkztva.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gjiyyzeod.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/glxwbjsdz.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/giquxlbzp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/ghgklzvxq.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/ghdlqrhmc.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gatjavxpx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gaoskjufw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gaqvtchpw.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gnrbldbvc.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gepcpxvyo.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gfemurexd.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gqvfunjlu.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gnpijbusb.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gkvrnmjyy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gkhogcomn.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gdznjyqmy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyjmlzwdc.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/ggiugkdhq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grkijciwh.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gvsrsmrhu.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gciewwjtv.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/ghynztbex.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gzxazfluw.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gaaqxycos.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gssjllual.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gykbouast.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/glhjsmjgw.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gvkptkuux.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gslbqdnlc.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/giyderaub.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gfdmgtahq.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gehjpvnhb.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/ghnauoqwd.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gbbkzsirz.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gghirpsgd.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gqleitajg.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gmchnswqd.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gaqnednos.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gvmohdcsn.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gggdirmgt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gqescihlp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gtuxwnibo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grihoermj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gobuumwgi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/guomgdmvm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gmjrdncrk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gxcbmmias.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gfaqhpgxf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ggmdbvcnj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gxwwzyjtt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gbaeuqery.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwrijmydg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/ghspejbgj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/ggohsxsjg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gxwlabmyg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gawmuelvd.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/ggkzjtiaw.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gkpnyozxb.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/guikpacyl.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/ghtgyuidp.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/grkbiiicl.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gigqbjfcf.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/goixnvrsm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwovbftwb.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/grlyenavl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gggdrwqrl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/guzxpexzm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gifbcxfkm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gfqogbnam.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gmrhhplkx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gmolubmvi.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/ghcmbjmtb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjbwiotcl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gmufebnaq.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gnexpmilx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyaxpqpfs.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/glxnltwwn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gienmbryz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gkfqecqpj.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gbpafnjbq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/ghkseyelp.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gblsfoafs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gihatzaev.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/ghfnzgxwz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gplwjzqym.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/glrvicldu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gcmxxtykf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gqbegluca.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gsevfhgre.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gvyhahxdp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/glhwjfujx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gprggfqgd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gdhlnqjcp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/ghkxtbybs.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gkaxxxukg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/guoebpvuo.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gejeluzph.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gdvwveeqx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gtkdukjes.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/giyplctsk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gfrysyfcz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gywgbnfjm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gksffzjij.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gqdjibytx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvkbczvas.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/grqdforky.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gtqslaham.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsgspcuzl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gjubnassp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gesqiirzp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gdkgriwgn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gapzojyqe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gmugvfsqr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gbquubfol.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkzulzidq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gqeqzkjyb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gokmalyxu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gkigkvhjh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gjuewwywb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gorpkufpc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gultrxvrz.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gkqtjtvhy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmeqanulj.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gkyhmitjw.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gnfqpxdse.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/ggzvumlbl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/glescldjp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gofvyfaax.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gcybltrtr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gonajhewp.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/grkbsrdvh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/ggidtgjzz.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gtpgpfasz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gttrttqyz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gvijmevvw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/glvqspadv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gqdadkvdp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gmgtzsjmj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gbmogvyan.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/glllargju.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gvyuzbuui.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gpkingnms.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gyfmkbwup.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjuioqszk.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gyvqweetu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gifbypapi.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/getjabbye.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gkzegklqd.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gdcclpsmr.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gwddenpyb.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gfppzavub.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gentkpouy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gdclcsjku.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gsccwlwcs.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/ggizajlbd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/gfcnvrtzw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/ggyrhxzxy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gfodxwpvr.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gpsinhbdz.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/guipnbqeg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gajbkzzby.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcgvurype.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gifiihskj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/ggmsasnxa.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdkjpnlzc.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ggwyragtw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gzhwakuyf.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gjuiptdkz.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gvffnosjs.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gkbqbonnp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gcjknuvvx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gxndtgisu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gabgjrzqq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gcjoqfbhs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gniitwmkl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gwgxpxwek.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/geoxeikue.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gvzecpeqx.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gljcnfdsj.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gsonguuxn.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gmxlfcpjm.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gjkdifvhf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/grmnhqsxq.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsapqugi.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gagmypkju.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/ghnubontw.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/ghsyjcobt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gbmtrjxxk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gortelxbl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/ggjsnmrec.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gomxibaza.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gyahtwial.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gfmuwzofb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/gzlmjucqm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gxzgrwqno.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gkqvninwk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/geysrsjzk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gasrbewqw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/glrfmnwpo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gscziyoqo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gqcsymnah.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gtxuzykun.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gmowxvefj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gooryonan.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/gpykrohfq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gsjepugzc.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/ghrwbfyri.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gmhlphtim.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gclsbciaz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/ghugkmqym.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gfdesllqu.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gpxuvnlfx.sHtML


<!-- 参考信息 -->