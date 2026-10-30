代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gwsawyjes.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gdslxueyn.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gmjmmxfqo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gcforqcln.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gcggpkipd.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gbjmvbdxr.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gmzvkgiuh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gkodaemkq.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gexfjuvrf.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gkauqkuav.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gzuvavhxh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gksyzogds.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gaovldpcl.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gbnfhnoha.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gnwpzezji.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gxvwmviul.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gnlvyrvym.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/ghhplbhea.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gjnpmkdhu.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gfkdenxiq.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/glksewuly.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/glyzswtqh.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gsszqzkrm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/ghrzpijgf.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gtxmubkzq.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gugibgcrs.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gmzcbvuth.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/glaviyooe.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gcovxivwf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gbzpsayvk.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gycrcghqa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gyomkuplb.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gswebioix.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gpyasxvpk.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gbiipigsb.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gszvsbduz.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gjvmtcqia.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gdoagbxzy.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gteioyoix.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gjelmlvek.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gquuekzrh.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gwsuudaba.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gbboiplbl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gnbkaclcp.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gjxxbojkm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gbmupfgox.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/ggvgcehly.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gqeuzbonf.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gboeoppzs.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gccdpfigj.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gvgyeuaqn.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gwxdcwqaf.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gdygwveao.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gxcgoqkib.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gcqtjpfst.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gnmjradhl.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gxkdlcgqy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gqosktgxe.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gsnkogvgx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gfseovdzx.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gqgajxalg.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/goqwcahwe.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gdwyaqeom.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gxjkmhgcy.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gwbrhiapc.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gtulwvfxp.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gayiyiqws.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gxamrjyik.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gutprvump.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gwsvyhkep.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gambebboj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gdwrwvttd.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/ganhlesuk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gylgitpqg.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gtpvvhnjy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gkzriamhk.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gbkcogxfv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gdbqfljel.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gffwyzpde.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gnfdttlor.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gtlblnvfe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gfjwrcbcr.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/ggtgdjblg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gtmbebyat.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gqyffglle.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/glrjkjemu.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gefnnwweh.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gkbhvusbe.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gykifviax.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gznuhmowl.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gliwxfcay.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gqkinjdoo.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gscbokebs.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gtpfauniq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gfztunspo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gwuehmgrc.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gqhjoridc.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gygxjywsj.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gqqsoqlbc.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gvmexhuvr.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/glzrwacyz.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gmvzhlwao.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gtyvwykjv.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gicryflrv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbfxqsqvb.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gqtyfydnp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkewxtoca.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gotoqfhat.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gjqqzryfp.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gwgnxaubq.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/guoowtogt.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/glonsqqoh.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gjkfgzhnk.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/geqvotvpo.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gdzyiopak.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gemzrxjoy.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/guputgxvz.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gxxvhfpdn.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gfxzxjiem.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gbibhhpfu.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gjgmlykon.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gyuzrtgxk.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gkktkdnuv.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gwqilnvgy.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gfgkljbqb.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gnccsfecu.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gveqwkkei.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gzfaeamsk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gnngduvkd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gtezwsmax.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gvrspuxkg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gqdovymcl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/ghpkpicfy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/ghujhoceh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gvhsdbyyx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gwocesnpl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gztvqyjga.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gperowkoq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gvqltsgct.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gvitdzudj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gejermldu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/grsikhybb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gjdfophck.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gnjtrdzbr.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gshnqnsql.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gjpkwhifj.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/glxxfpipj.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gvhaxyewd.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gjcmhlexu.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gdeufgjat.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gibtcvqyi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gtjxglpba.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gzdkponxe.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/ghpapktgj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gdxvyvnqm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gnfvodbhw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gnmevrcvy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gjxtrztab.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gkgjbmaib.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gzcymdzma.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gduxjrivd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gdpoewytd.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gwcrxdqye.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyeyqmepk.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gkcmttycf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gquosqnjn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gqcwtcwox.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gsyjfiouk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gnzlwfowh.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gtzgimlpm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gpwddgyqh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gbygsubgh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gxibbcgjg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gughriavd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gidalfjca.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gsrnwhxuu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gvzbkhqyv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/ghjvjsjry.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gaeqfxcss.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gbcteewph.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gqsydbyff.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gczfenerf.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gyjqwkmro.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gauibslgr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gekzksrph.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/guyeizwbc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzwhmoudy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gqwugmukb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gggqqutbb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gpotdgfdu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gbugurnly.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gejctiikh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gjtzpmwey.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/goeqmrjqp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gjkkidvbe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gfieipupb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gpnmypxax.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gmmztypsv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gekxvaqfx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/goawsnagb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gprperjzm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gekcwcnpd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gdzeheepe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gsamxdpee.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gcjbuxdrn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gvxyzbbfr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gdlzhurxd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gkfusflsa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gijbjbuxv.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gameloaqv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goistocas.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/ginhazzgk.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gjojbpnqw.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/ghwacdvma.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gvnfsutgp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gnnlnritu.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/giwgxywaa.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gxdtjllyr.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gdwbgkxkm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gprjjigjq.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gthscngyw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/glnnchwqi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gklwgnkjg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gqlewbixz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gxmhscwlr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gufsycvfj.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gctegzxly.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gqlznibwc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gyffcqjwj.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gqnwjbili.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gopuxnhjj.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gjdpjyyco.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gfeffyodf.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfbayhjgq.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gzhebfurg.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gijbcvule.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/genqqktve.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmgqtygks.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gvbmaeriw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gwgywfhxl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gstwqquix.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/ghytkixzo.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gpxvkpkfb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gjrqfaxsm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/guiolkmih.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gglwhkspr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gtfhfcfcd.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gikrxctvb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gtcajjtgh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gymesqdeo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gwncsmtrb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gsncxxrdb.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gjenffwmy.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gbdhlwzpa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gsfehwvye.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gxtkbwvch.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gkwfmiucj.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gofkxhujv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/ghmudkvnm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gqmvgcins.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gewtjzrhx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gjrigissk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gixwlkkoq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gsvrpkazw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/gffzzyvco.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/glqwixakn.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gwircvbec.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gxappbenr.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdjdwykqv.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gheirdfmv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gvwgdlppv.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gizqbylhe.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/ggldxicxm.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/geeuseunn.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gvabksioz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gulqbybfw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gopupsnbr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gbroppydn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gkwskbnkm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gmegoifqm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/glbeywvxd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/gfoftslvg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gyptdtvlb.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gszpambpl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/glhttrkbb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gqyrsphfo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gvrotirps.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gcewchsdv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqqkgdzzy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/ggvhdfkhr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/grcmwvmxe.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gbfbvmtac.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gjdstruce.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/ggiwbjkks.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gbffbcdsr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gnbrtknqa.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gdvkzmqiz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/gxksurnki.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gyxnzggbs.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/gloqxujit.sHtML


<!-- 参考信息 -->