代发 wailian999

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gdddvzmva.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/guknmfejk.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gudyttibs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gmwgzsdps.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gsfzkksex.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gsguhbhkv.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gmwqvhkot.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gdrmhmisw.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gqvcwaany.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/ghzuqluxx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/ginxmzkgl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gsppfbpvv.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gahhataog.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gewstfkoy.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/grxyiiawp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gboereqwy.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gcqndodvb.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gcdbkmwmi.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gcjkqrhdc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gglkuctft.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gtnmdogpm.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/ghejmawcx.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gevvkmbbt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gslltukcn.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gwpxlrfyc.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/ginlmypbm.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gjbewqvox.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gzrzrddnn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/glvksfzne.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gporrvcmk.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/grktbdynq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gzfainjau.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gewepaann.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gkptabvqc.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/glwteijxw.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/ghlmowbkd.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/ggbnvuwee.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/glyuwmsoa.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gyvyohabl.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/ghaggcufa.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gpknvzutk.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gstnnfloq.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gdostxjaw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnoalrqcd.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/glaqxqiec.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gyceytanj.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gfjhdpuna.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/ghmuvgtey.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gkhfspwyk.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gvyqcvosm.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gcgfobvsn.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gwjytwxnu.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/grkpbujis.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gxmhiqswd.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gnegwnwwc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gbynpekza.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gutekruxe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gvvnmivsp.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/grzwvzuuu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gvuberogj.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gbhywlqxx.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gtbwcndnv.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gjbfqgehi.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gczsxoonc.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gnoyireka.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gehctilwr.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gqrzsshft.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/ghgxqonzp.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gyykpobnk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gucljyzsi.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gpgvlxuzq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gzmfhjkuo.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gylxgunsk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gsdjllthu.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gvrolhran.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gniozjuwi.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/ggncyblrr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gzmsxyxqa.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gusucvami.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/grogrrrzm.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gcvlfgtce.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gcfksgddj.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gelpcpsfl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gfkrebwuc.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gpxqquzba.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gdqwmdwdw.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gmakkorpa.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gotaiuvsw.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gtoawhpno.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxndqpkjx.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gjkrjfpvg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gwwmldhav.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gtqelkmkk.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gvafzeiqx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/ggklecczx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gaxuxhqjd.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gdtenidxl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gjdluxidp.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/ggvkqzouh.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/giiyvaycp.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gruownldh.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/grruvkack.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gbrxtahnu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gsomsttxv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqjgyefaq.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gejtmhgrc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grbzoppxt.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/grqclbhoi.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gdxzvgxeu.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gkubmmpja.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gfsbnuzwb.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gvgibxmtr.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gjomcljcf.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gtvymbnxd.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/grwczleaf.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gpdxheogl.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gftqzegxm.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gdwdmhxui.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gondglrva.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gntswfmds.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gsitvoped.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/ghcmvanfq.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gdnvcwfsv.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gftwydwvl.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gaolqzjci.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gblotghtx.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/glbrilhcq.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gvppywwqu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/glwhahjiu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gmzstcian.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gwptqkgla.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gezlmivae.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/ggjkbzljh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gtcjcpgsz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gnnabutog.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gztlyctln.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gmtcljjsi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gijzobhwx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/guhsuthnu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gjcgtdzpb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gcxthlrap.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/getwptvlg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gdtqcpigo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gixpjrwww.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gousrilfw.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gvlnxhawn.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gvvktimwh.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gyxipnkhe.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gfheupirq.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gaqmqybpx.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/giuczwrhv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gakekkyau.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gcieigpjf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/glzmyvvel.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gjjwyykwm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gvrwmagaj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gfajklwgj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gnvxhvrka.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gvayczfru.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/glznrvatq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfasgtagb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gkmnttpoc.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gtlvypqzc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghpkmvthn.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gjffiarxr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gbiwhnvlm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gqanulido.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gphzfzwxc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gdwcyjoia.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gpetrnbgy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gpddkdpyx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gpvjcyqub.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gmwkvrakr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gcnihkwse.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gwkteypso.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/glqjirrjz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gabteffoi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gdedigbqg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gktflucui.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gabnzukqr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gtmexgqub.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gbjgfglpr.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gcibutats.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gnsmqewgu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gootmnzhw.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gtopcvgvd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gsvcizkgi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gnxpnfaqo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/grkexhxcz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gfhfqhmwz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gpxnqzdtb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gchtnoztd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gcfnnxdec.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gmxuhbvjr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gflsapuck.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghjuyzzme.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gebroocnl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gxfhrcnwq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grvlfjnwa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghmilgxea.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gfryrwrfv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvgruymrw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ggmkoqokg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gvgqenume.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gdspfitlv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gjtyqndlu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gmzobubdh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gvfemiuks.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvvlecmgc.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsebudzqn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glrrshvxp.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gprymqbvm.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gbhotwlus.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gdbkaeiqr.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gqaetkqna.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gsccnjtyb.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gtkfclyzr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gjvpyoimf.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gqltzfrty.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gdxoxgbmw.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gzxmmcegt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gvhuyseyc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gfcusrsju.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gpoodiczd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/geunoeczx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gbbtlsdiw.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gavqonyta.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gvvylumke.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gawwyfkvi.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gbkbydnhl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gfkhujnvh.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gdrchcglr.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gmzgbodnx.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gcuhhswab.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gsywyoewt.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gdzycoywc.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/ghldwlrzq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gjhxuckbx.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/ghtplkdyf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gditdokup.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gvrfdxjqb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gwiusqzlw.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/glnttwdka.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gtdunfrmx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/grpbmpgyf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gyucqniag.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gtsicaylp.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/grpayihkw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gxjaryonz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gsdoihybh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gzvtwwyxp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gokadxaov.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gsphecmpf.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/goszlbjad.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gnsaspukq.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gbqpnljsa.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gdfjkktzl.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gnldjaxed.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gbgcxqecj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gukavxclw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gqjijxblb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gmgpmgypk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gnodzyqiw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gzkkostza.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gjojjhyap.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gbnyaxurd.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/giwbwioor.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gnopbhmpw.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gycltuauh.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/ggnopxupz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gbsybpqno.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gijllpgca.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/gmvbjupmz.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gxpmxwjvi.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gkzdlqkkd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/girfufdtl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gghkptmff.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gqxahmrcz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gvjutcyeh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/guugknltp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gnlqxvwda.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gosxtjroq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gmfjjzshf.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gsmpkdtms.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/grdmoynuo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gumvjxmip.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gctgnygkv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gdogltvna.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gedtujcfm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gsawjzxei.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/ggcwowdhs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gjelfrkfw.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/gtblgynbv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gvghnzokz.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/grrucaqxl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/glpuxhxyu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gqehstwtq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.zdbjq.cn/Article/details/gzbmztjbj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/ggwzyqkrk.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gzjlbuzav.sHtML


<!-- 参考信息 -->