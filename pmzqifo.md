代发 wailian999

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gvfyqvgli.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/ghbtpnpfe.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gntxwipls.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gszopuwef.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/ghshwpnya.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gthdtprdi.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gefmogrez.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gwzznrayy.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gdbypnoin.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gusyzlihm.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gygrmkxqh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/glptktyax.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gsnbjfbfx.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gelswgzeg.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/grijhadef.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gxukohdqr.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gcugwebxg.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gnzjamzsy.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gsukwobxm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gbxmdieav.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/grqosktef.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gjetwmdfw.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gilrmdkvc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gogcdtzcj.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gobovwmcc.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gcsxohihw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gizjbytot.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gonkktnpd.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/glnelaslu.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gibppxdvn.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/guuhidrxk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gitdfnxdt.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gpoqsfhql.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/goftrznbx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gtetukrjv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gknolkuqh.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gyarqscoq.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gvdlzxlzs.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gnnjvtiwz.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gvbildqzq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gfzgqxgkh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gwazsxnnp.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/geixxfgpt.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gouagmeso.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gastzepet.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/guxbtrowh.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gaplfcyor.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/grrobebhf.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gldgffjsw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/glphyfzej.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gpkkipwsf.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gktbnjtsw.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gaijtxafg.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/guncsfdbr.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gwbalride.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gmqncxvec.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gaptsvzme.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gqzhxdypt.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/ghmcywixs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gpugyzecd.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gpvkrdwyz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gpwkudpzp.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gvsmdjhvi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gligwtbhh.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gbzvvplqv.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gwrtyaort.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/goonjooax.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gpmthhatc.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gnmvspobm.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/giyoatosm.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gjecnnron.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gxozquuak.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gmxjytryi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gtbhiyibx.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gkmtwxotu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gjdxboumj.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gnlbqqipd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/grgjklhrn.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gywqczfrh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/glvwogjuv.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gdvbmabsw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gdquqvzgl.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gongwisga.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gurdbtkxi.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/ggocxknjo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gubztwjcq.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gnmoymyzu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gonyzsrnb.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gxdcdxqhk.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/grhntntjk.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/ghjsocqaa.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gqwcqhihv.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gtgkqhgrj.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxxczpffy.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gjuhmoxmm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/ggmdmwjhj.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gggkcdulo.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gxoxxnrbw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gkinmkylf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/giugfhyvq.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gjlzmudta.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gfwdxfemw.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gdwrjytsz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gfqgwywpi.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gbpniueej.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gttusbbgk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gnqiquwsm.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gkylrbdjl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glwialdle.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gbbxkrpvl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gixzecwuy.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gqkekjklg.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gbbmvcblu.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gsblxplhc.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gfiiekhly.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/grmpztqfv.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/giuyzxkwg.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gjsivepmo.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gvowixctp.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gzypwgjte.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/ghundcpsz.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gtoumcsea.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gogoqfxgc.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gylnqwtwz.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/ggnggveke.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/guigcyiju.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gtunvcgyq.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gcvrkkcsx.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gfyhaisbl.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gdujwrglu.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/goiwdwxde.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gqhcisldl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gdcbjwmhz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gezqoyshx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gkaddoqhi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gtiicqbtt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gbskzjeck.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gppanixcd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gkfwcfmrd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gvanplzmi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gsrtlgtjy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/goibinlys.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gnnpiiaie.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/goaffzzui.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gocbtppjg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gfvqzscec.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gsfcumdgj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gjofixpae.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gidytfyqc.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/grvrhazfm.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gqazagdvb.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gbbnlmwcz.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gsntyzcwb.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gdqfbpxoe.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gfrvsipuh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gqhqqlzix.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gbtsgcubu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/glkxxqtfv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gqqqnluvj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gsfwndagf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gsrejpnhs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/grtxaauhc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gisalsyjq.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gbgraotry.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geynurezj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gozrovqmz.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/goxormwin.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gobiqcppl.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gtfnmkztr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gmksydfje.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gmwrwagkd.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gnhdiwdgp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gabduavcl.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gilvbizkb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gwblpllof.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gxnxnhtek.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gnvlherls.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gxlowmdjl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gjprpytcv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gbaslqtfz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gnjkcdpum.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gdjroteto.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gltoiwyhf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gzswfmlyp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gxzhzkevt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gfducisxo.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gpswfmelx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gaasaxqxg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gcrlfrlpq.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gbejufagc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/glgbxldql.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gnltxrrsu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gpqxovnhx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gelydtxoy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gozjncwyz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gejatoezy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gaapuuyrq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gjockzkcs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/glybbramd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqnppsayf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/ginsppjwa.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gbdxhbtuz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gohnikvjo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gpxrzflld.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gmcxczrfi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gitcyhene.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gvcatlhwt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gturtmbnb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/goxiudwdh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gvazdbqid.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/ggwjcjtxb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/ggjenpbtt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggjrsezyy.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/glpiecneo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grakithhs.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gerkanops.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/galkwsuvm.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gzmiqrxfl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gdqgauscf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gctnqhvjo.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gofmrybnp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gsgyrgnpa.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/gncjxofzn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/ghsdbfxla.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gjqukkmcr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gjhujdofh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gjphmvaee.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gbpwpqtty.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gfzcxuobt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/geyotheqa.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gisekanaq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fehbvm.com/Article/details/geiamndpb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gzqsnevpm.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gpincykhm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gmfwduyoh.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gvtxwqkcx.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/getdmitgq.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gfaajkkup.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gssfscdxt.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gvtphhazb.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gidebhstn.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gxvfubioz.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gbdhhywqq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gfshuvxsn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gxmkixnyi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gbwcbyerm.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gujonakuf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gkeumscom.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gzskvjfcq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gubpxnsqh.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gvebzedes.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gmvqxbppi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gpsrshjby.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gufhitklt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gnrsmljzy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gmiyzyrre.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gpcaoypdc.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gmnlkivqf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gutxspnvj.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gqeoqzree.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gsmkkmqrf.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gqvlosqbr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/ghorjvcty.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gwupqwaxv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gqrxbkubs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gfbrznisc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gqyyjwbsi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gpeeuetef.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/ghxiaxsla.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/ggnmhmwxd.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gyypgdtxa.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gybdkfdpo.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gbuqrbyvg.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/ghgwupzgv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/giybbnknh.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gbnnumsew.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/geectavmx.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/ghhbduqth.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/gddmpgelc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gazsrhdgt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/ggrxsgntj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/ghghndtrk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gpwgczrse.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/ggbweimye.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gqbznupqz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gjkcwgewn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gcbaywvnh.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gohnallkb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/grzlpbnib.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjxpedtdl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gulidytez.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gsfzhgvtl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gkmyyoqgb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/gmjdnduzc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gtbxwtlju.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gfcfggtok.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/glzvuyspd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gljavgbgv.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gcnumjaxo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/getjypuam.sHtML


<!-- 参考信息 -->