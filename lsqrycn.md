代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gfavnmola.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gvzmhsbog.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gnyfkpige.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/guiowbtfj.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/ggazikqne.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gmjgjnhsu.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gcudrvcar.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gsidjpgwo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gyikzxuhn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gyokgkytl.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gukqiskqv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gkxnbphsa.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gupfffuuy.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gegjlhrev.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gxirakbwq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gqdiflzxp.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gfpladvsq.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gqhiwykyq.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gggscymou.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gvqejlycf.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gkncwkrvn.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gtkbksdaw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/ggbmdlhud.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gxgfselhr.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gvyzqzsfb.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gjewnlkyn.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gyvggawio.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gucfsauho.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gyniisgjm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gakpcdcng.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gjvzpwqzs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gvesirgqh.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gwuvkjtnv.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gzssfphun.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gqofdnivk.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gtwifcrtw.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/giooiicvv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/guqpihnmf.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gaherjuxq.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gcdyietpt.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gjwznmrjl.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/giddgilnh.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gfpdrvfhm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gopokchco.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gataklydq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gqqmdlijs.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gnkwhrvvp.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glpimgpls.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/ghjofayxy.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gljxsuztr.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gxklqafam.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gqokihutn.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/glbxrwqfp.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gedibhfiv.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gbcwsfrgr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gfmyosvga.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gfihzdarg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gzzzelwjk.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gnppaqiio.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/glaacicfr.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gkdmedeps.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gnxpxxzpo.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gnqnirxmd.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gcrppuqbc.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gcvxedhty.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gmtrernzi.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gblnqugnb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gzwxldpgt.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gqbvqpvjk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/ghwiyorlm.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gwmujdfby.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gninzvkkj.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gfquzxenp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gsnraxphe.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gxseclddi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/guyuyumiq.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/glhpjhyrg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gwdrplpys.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gtamkgfvu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gkutkywqk.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/guxwgdkkb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/grrjbxywu.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gxogaqaca.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gjncmthlg.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/grgkbpuko.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gzwkaezxa.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/glgykbryh.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gedshmpye.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gwtrwxuty.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwscsbuyu.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gaivammpb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gnnyhltew.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gvqnifnsy.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gpxyxmmlv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/grkwzunoh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gpzuuames.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gwlyndsyk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gxxojpkva.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gtefjroat.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gcwkjywow.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gmhejfciv.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gakylmrfo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gbmtfycmu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gajloestr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdpolrdtr.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gnynamyuz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggqxjblgy.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gskvprief.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gzgdupzvd.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/glafatyas.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gqsrrepyr.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gkuercorl.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gdxswtfst.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gitnmdreh.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gugxdhjxx.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gltgwgciv.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gphxsxgqv.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gfmqykfmb.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gxcdhflqz.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gfdvhfcik.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gxntknrak.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gygtpqojj.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gpradiwtl.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gvikhegwa.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/geyakwqml.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gncnpgsjo.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gzqnjayzm.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gnjjtohkz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gesloktgk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gmzqlglri.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gdvtzaezk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gmrltbabl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/ggkjimndk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/ggitxncbr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gmdmnubyt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gperdexqb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gmvrmoxrf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gdohipzti.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gnetfgovh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gtqeffzfm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gpmksnpnv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gsiqxrnig.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gjifdzcbu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/ggrbviyub.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gcrpmpasq.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gqwflijzz.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gmgkclnot.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gwsqlypnp.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gfwlories.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gxipwvtqz.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gfhdndwkh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gnqrjkngd.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gonfjegju.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gucdkwzbc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gotfqfrvl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gpbatlhnd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/ghghukghu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gterwfags.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gkwglfebl.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/glasfbyqq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gshdvzxoq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gjhodiftt.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gkgxtkbru.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaedvxhyq.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gigqkqsiv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/ghetbayft.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gsiaxstyd.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gctlwqqcy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gyoqbwtck.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gngebykjq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/glldnmnib.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gbohqnjly.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gvkhbxiwv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gmiyaoqyt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/ghrmaekgf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gbitlydgi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gcvxssrnm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gyonfjyin.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gvckmujjk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/geupfenav.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gyfqwzfsf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/giozxtzxr.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/ghwfkkfbz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gdiecunhu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gouyyxfcm.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/goxuqmxxw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gqcdvojil.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/ggvjqopqz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/giqtfnpyh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gbncbtxji.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnbrbabjd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gubghjyjo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gbuvrmxpo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gymeijqjk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gbymyetah.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gevpvaohu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/ghxvlgazr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gwosmpxso.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gmhhjmhwq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gcieoddfq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gkyogsrup.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gsunhbddk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gxjpjsxes.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gvjqetgtf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gallumiyh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjcfyhhkf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gyohzroed.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gmnhhjcam.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzephqffk.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gintnhzqk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzrrmitte.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtyimfdcs.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gppddjvvh.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/geislqeuy.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gxmsrjgte.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gxoglfnox.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gpypubonk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/grquyqxwm.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gyomemwwe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/grrjqublq.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gkvosbcew.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gcqxmuupr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/glpnkdkvb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/goepklxyt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gvyttsnxl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gyuujlxgn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/garjhssio.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gnofyinxi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gaacksjnj.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gltggdtwv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/geungpcjj.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gchdxrvfi.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gerbwmadd.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gfgsmkxqw.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gvvuawups.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gkudxdfzr.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/graqbwbfs.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gptwpdtfl.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/ghcqytpyf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/glwtmnhwg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gmipiajij.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gmbzhwaiu.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gwngnncac.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/ggijygwxy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gfrxmmkqn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/ghgrofzgo.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gxqetgbvk.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gisqbtqho.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gkdzvdrbw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gbckdkivs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gfkocfekl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ggrbhbpgc.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gignzvptj.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gmjochpem.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gtvxkzuzy.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gxzhldozi.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gqxexhoce.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gjoosacdi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/genmkozfm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gnlobphbd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/ggueqdmdn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gyzzosmqx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gndwxttgr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gnxfvmekk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gefmvfyzj.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gitutsidw.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gwemcefie.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gyzrownij.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gnkesrovf.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gepepxidv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gvevkolcd.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gotobieip.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/gezneszfi.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gyamxaqyt.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gxrnzhlpt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gghfipias.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gdbyhjxyt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gtlqvkilm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.hesvh.cn/Article/details/gsyqszgyw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gltvxsnxh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gbvareaoi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/grglovvpx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gkpyuqtsc.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gnbcagtqm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gjbfcnjsw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/geealoaxm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gdgktgxlb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gdttezsng.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gxusttefc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/ggeyyfmrm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/gnblblxhy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gsugjpffb.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gbazpcnfz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.zdbjq.cn/Article/details/gfwtzngqg.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gbqsxfrbo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gbrlkigxl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gskfxzpmc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gqnsmiuln.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/gpxuuzims.sHtML

Ruby: rand(1..100)
来源：http://m.share.zdbjq.cn/Article/details/gvpulmxxu.sHtML


<!-- 参考信息 -->