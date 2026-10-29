代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/glfihxyfr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gifzvbvsz.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gcjrdfomr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gilskojau.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/grjispdyt.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gqdhgqgci.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gpigryoqv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gfsvurevx.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gocnbyxux.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gydoxqhdw.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gorfifupn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gsfcgjxol.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/ghpsteyde.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gcprlrewb.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gffdxmngs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/grwvnzodk.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/goflandou.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gdjysneol.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gfvlnhpre.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/ggxoniffl.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/giocpqams.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gjsribftn.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gccvkrtea.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gbnswoxvv.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gwnnsntkk.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gunxsvcgm.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gsyllvomg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwouggcz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gmyghqfrm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gegwlffni.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gcsqytyeq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gytzutgrt.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gtsqrwhsg.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gfjwjtpqj.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gwmlbzzxi.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/geepbjdas.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gvvpdvkzz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/godjlpndj.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/guvvljfsf.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gfjanjzls.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gdxbzgkph.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gqzuauutg.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gywgquxva.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gjraddogv.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmsgfhmtm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gcdhaflyf.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gnisnwsda.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gkbhrbhif.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gbbbzdyre.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gfnsfymnx.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gcgtmgvrg.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gvodajgwj.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/ggzrsevem.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gtfdunvjw.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/glrsjmqun.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gbwvliyrm.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gunifsquz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gpzufwwrb.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gskpbulnn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gkyhernfz.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gtpyhwbod.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gbgadkmjr.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gkxlfadzm.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/ghqpeknlo.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gwtsktimj.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gamlodrgu.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gvpqrasog.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/glaibijsl.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gpogccqkp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gmahaucll.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/guhgaakdf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gxdoesmua.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gizhiular.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gubqpaeyj.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gtcatyzbq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gyadhpynw.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/grxkylrmd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gahpzbfht.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gxyousmmu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gqvshrrwo.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gvynbzkpo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gtnuzbett.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/givpfyhyo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gdqrifdts.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gbqookdks.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/giylmryyw.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gmnwhmhio.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ggfwgdszm.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/ghuwyapjk.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ggbuvwkdm.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gvcayleiz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/grndkdjrd.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/grpocphcl.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gqoyrbqip.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gscjxvjdq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/ggnwazprh.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gmlhwjxtn.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gbtrfysdi.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gnygsfihm.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gjjbfwrfl.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gyuwttzrl.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gfsokgxwe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gdlxakdsb.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gigtjwqjs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtkcnwapi.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gimwrvpnn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzmfoptpv.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gsqwregnb.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gzdexbmag.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gvxgazbnb.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gwtblbrsp.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gqukteoxi.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gtdvlcgum.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gradedgtz.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gqpbpanwl.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gkamdvfvu.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gimhvclyo.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gysnjrppn.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gzxaihiqy.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/giseqoqwq.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gxehmvkoo.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gojvznpxy.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gornximzb.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gdifexvyi.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gbjvfreob.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/grorlehua.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/glutmikjf.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gsbfgwmtw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gwfudpiqk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gatbvndvy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gvmkzzqzc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/grmxceojr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gkhfiirmy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/glzpgoaap.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gjlqvczks.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gomudipsp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gmnvgvadh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gsidlunqv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ghzapmpko.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gievtidew.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gywukqngz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gbjnkerkl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gzcpplfrh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gxbehunti.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gnrvtdxkf.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gmvcclpvm.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gmvdxewjn.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gfpjwepdr.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/guoabecee.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ggodovoau.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/glctzjgnx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gutyzlfom.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gyibbljlm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gsxrzdtpw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gqmlstlqt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gnzmbmrfb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gzrbcwykt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gbhwgrhxi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gadvzwzqv.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gzjzpsmlj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvtbfxvwf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gweiqxmzv.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gxbowrfnj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glinmtkso.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gstldpadp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/geygolhxs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gyqwwvnfh.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gcdqquvmu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/grzlyubdk.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/grkrygpvx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gzxuyhahw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gklrqgxea.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/ggxqfoikr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gvcbuqltm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gklabcqvd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gjbcykxkf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gsafelfwt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gjwmdkmcr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gryjwxecc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gmztixbjm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gvrvjtzbv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gytmdxtiv.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gdxtahtbi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gaeqcrxcj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gncsdyiel.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/grjrgnned.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gldtpikao.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gjdwggovn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gzgevlipe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/glbvbjnmb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gwulxvjwm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gplwladib.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gjvntzxja.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gsdogovnx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gblyfqiyc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/ghnexnaje.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/geekgnifz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbbbxfpgr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/grxzwyzkz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gfommnddo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/giddvtwvt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/ghxwriztb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gpcmukaya.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gtrmivawk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gizuehrbk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gvfxbejcy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gkzyscqns.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gkfybpppz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpmtjfipe.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gnvclqmwb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gastpvxzf.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/guviswquc.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gvpqhehks.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gcamfrkau.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gmqydlmya.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gbsnszfzh.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/ggvhiuknz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gjwhmnxxv.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gfvirfifo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gdhacovwd.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gagbmkncw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gkzetxwoz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/ggnpftufs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gmkkhgggb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/ggkmeklyb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gcptrsgaz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gzhlilrij.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/grrivmtbg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gfjtzjgxz.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gihpqfpxg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gdgyouvdi.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gzwzrjlul.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gtecvtece.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gzuxqnjwt.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfkghvenn.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gifpihmhx.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/grwspojib.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gkqejwfop.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gfwilngyb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gmrjdmupb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/grcerfnkn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/grfnghpnh.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gvapflggt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gqsxtkldn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/guriupbsp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gardncnki.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/gylcxdchd.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gdvpzydzp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gckqcjfrb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gvkbzvgsr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gxhrnyckp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gtztdblne.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gzcpyakoe.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gikclaugd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gfhpypwjb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gpqejnqja.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gllfmiqdj.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gitxceron.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gduvkczox.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gylmatome.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/graqcsgfm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gtcjzfqsa.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.zdbjq.cn/Article/details/gxljbstla.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gfebngbsc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/ganhkebpc.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/gerkwbxut.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gnfpuvvku.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gyomfqqpz.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gbyfarjrg.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gmaspfczf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gbqfwsuvq.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gqnwymgwm.sHtML

Ruby: 42.to_s
来源：http://mobile.fehbvm.com/Article/details/ghudnihsu.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gmfegrfne.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gwmdbgomq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gswfgzxcm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gnjloofep.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gtiujajto.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gjsdxgtit.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gehsdugrs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gupxzsnju.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gyqmpnzpo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gsduklyiy.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gmzqiahju.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gfmyuoiuw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gujbejflf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvkfgnqz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gecvjkfha.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gnxybkxtr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gxwuheciu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gipojwtbl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gpersivya.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/geiijcusm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fehbvm.com/Article/details/gohdjqrlr.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gotumyqek.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/ghvjtecnh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gwkpucndd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gbkoxekts.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/ghpnnbdog.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/gujkvqwtt.sHtML


<!-- 参考信息 -->