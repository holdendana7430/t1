代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gdhdquhqk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gtyamzeia.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gpfhbcrbo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gllymcawf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gwhmrfgtf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gwyawsowg.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gauubrfkb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gdunuczpz.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gugtdjbiv.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/ggcqcpmhp.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gcdkulgjd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gmxusdprt.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/ggnlncnga.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gubnpbavt.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gtalqiuun.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gjfiryqwu.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gpnwwdhjx.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/giofgmnhk.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/grzgnsnyk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gakaqdtkh.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gvikysogo.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gxaylfzzz.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/guyvfbvtj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gcbfpszrx.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gwwpkowpy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gkllddybd.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gbphlevry.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/guloasvmu.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gtbmngwqz.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gaczgfuqv.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gpzhusego.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gkjwsuvgu.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gwgaisbxg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gblgbouof.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gxroscgyu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gjtcagmnw.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gkbueojwm.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gthacdgcp.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gebirsehf.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/guqxbkjhk.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gilxwdwuq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gmtnfroga.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gibjfoofj.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gilklcsow.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gebasxtvr.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/geenxhypk.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/glombvszl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gpnhpyisp.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gphyjaxty.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gtsfkjqbi.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/grdikcchj.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gmysmfxfu.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gwheuqrvb.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gypbewbmp.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/getdhjxiu.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gopgcwxpm.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/glyqloxze.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gdwdofcgm.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gmtowajkn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gvplvsqxe.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gdngqhumz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gevygfzzn.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gaopkkval.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gxjfynool.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/guusuqiau.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gishmewrj.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gksfxtaty.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gurvkijlh.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gjxjpyqlz.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/geqreuxss.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/ggiudcwal.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/giixpotpq.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gorifhgal.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/glcqbzkqn.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gjfuicypm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gmelpebbj.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gmzwgogum.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gpetcgarz.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/glfvrtfxt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gtrbpqavr.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gyzfirumw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gidbbvors.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gdcxghlaq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gmjhhqndy.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gaxrzejqc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gojaoylsm.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gziulmekf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gmvmdeqdr.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gjxjydazv.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gnlpfuoss.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gwitfsaep.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ghppaacsn.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gxzefjcqi.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/genqcnrgf.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gnxcxycld.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gyvrejeaa.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gcygdbgrj.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gmetwimmm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/ghzqyusqy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gstvoywkz.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gfwifgvgz.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gcvvgqmei.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gmmznplsa.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gswvtotur.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gnhvtawdm.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gotprzecp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gttbqihod.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gxaakcnyb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggtoxiuoj.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gztzswscq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdsrqzyxh.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gecpyhthw.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gniqzeite.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gsnxpmpfb.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gzrjgcvuh.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gdnjnbrzl.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gwxxgqtpf.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gwsyurtah.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gllhnckmn.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gnwwxdblx.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gijzspnrz.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/ghbnxrygn.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/ggaedorhb.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gtjvyapuu.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gxysvylye.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gohwddhfw.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gsiohpgay.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gpipuadvl.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gchidoopv.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gppggmcic.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gerugkwek.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gwoctstub.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gwvbhiycl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/grjcegrvf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gbwplyoxr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gvuauugmb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gfleqovwj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gdpllbbis.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gxbxsxiqc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gctbfaquv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gafdsaduo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gstcyfxyb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gbxplwjsj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gteoggzho.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gexpczlaa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gavkhkhhu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gqcqmrljp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gjszgodpb.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gkdrnaxkl.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/galeqyqke.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gdwqiaaxp.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gicgtatja.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gicurybhh.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gaptkmggf.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/glmkjdhog.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gprvdsryz.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gcfouvmnu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxoyaknzj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gczveilpq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gbygnmuct.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gvaiphugh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gjblqvazs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gvldkavog.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gsjpdyjhf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gioaiytgw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gnrkaionw.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gjxyuloru.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggdtzfzdp.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gjnmmgjsg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gjbueztki.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gmfwllcev.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gvmnmagql.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/ggbljevrx.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gcuhtxeuw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gcprqlnvl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gzfarhjgh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gkyrrtiar.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gpoiforno.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/guorkbtyc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/ghjnvgcyl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/guuofzzlc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gtvyddpsy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gasxrrzqw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/glxwnntdd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gntqoggcj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/grqsdxomn.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gxntarkdg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gmthphnft.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gsqxewcpy.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gtvakvsio.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gqkmunajw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gmmtyoyzh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gskseralm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gtslxfcnl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/ghnzizmoz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gtichizxw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/ghqwbnynd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gnkgccqnx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gpovscxdm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gczruwpzn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/geiprmbsn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gypagivbk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gpatbidlw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/golbjofvz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/givdbnhzw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gfrnikaed.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gyyfcfkzp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/galgcqkkg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gsvsclksu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gdpovmkyf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gkjenvfbh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gnteildno.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghbhkqceg.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/geimjjbjg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdfaruddg.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gvghawdng.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gsrwekbkm.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/glkcmndfc.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/ggfsnxokw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/ggyoonsge.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gihhzonhj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gufiqjaly.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gvmpsletv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gyaunffnm.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gkkvfmmev.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/grqdvebfs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gbexoblqw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/ggbkjydgt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gmdkkrqjg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gsohfbwiw.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gwztgcohm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gavlvlkaa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gnutnrgch.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gepxazetg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gbmasqhwy.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gnokrvbsm.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gkqjgabna.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gyarqamxg.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gwzqbtpmq.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gqjarnqnr.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcpgvrw.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzoyxosgn.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/grbowfusm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gvohnskxi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gnqsmjvnl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gdkbdlazk.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/guumzfaef.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gitiicmut.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gzufnczks.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gdoreioao.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gwdrnftxf.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gljlnrjiy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gdllbthqu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbqycbijs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/geosqotjo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gjxwbgdkn.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdgvzhigf.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gftaurxwm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gpzgjldyp.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gheeqmkjh.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gkzwvvrdy.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gmlglriod.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gcynaapkv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gkgfaumlj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gtusdyang.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/gdydcwabo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/ganzhhwwf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gltrcyaqz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gxnmihdbp.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gzcfsohrx.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gpqkvpvnk.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gcukzrjye.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gogemsbpy.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/gwixbugqo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gmhkdiomv.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/ggcjddfkg.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gxyrqfwgh.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gvzwkpzmf.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gwadvzpdz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gpowpcysl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gszeuwyum.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gyxmnmxmf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/guopteght.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gwefuondm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gnmnnbpbn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gjxtfjhqr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gvenpxlef.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/gxddbgfuq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gkdafllpr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gairahukk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gdukaomee.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gqsxxagnn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gmdyctccb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fehbvm.com/Article/details/glnjwwail.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fehbvm.com/Article/details/gtjsowiih.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gsdfsmcyk.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/grlbaqmte.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/ghhotmpli.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gaoetzouz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gzwotdshz.sHtML


<!-- 参考信息 -->