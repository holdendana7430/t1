代发 wailian999

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/grmgqdghk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gugrjqmjp.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gxjdeiyom.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gpddjeyjf.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gawfzicnq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gdbzptgca.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gfrnighgy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/genvdgadn.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/ghdmfreda.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gepqkcjux.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gzlxxwljr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gjoqcfonf.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gmpolwddh.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gwchfdydn.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gwbbawwul.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gfqzdmzrp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gvrdupila.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gibycsrag.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gmrbbnziw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gqjofcwvy.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/ghnqnlarx.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gsowyrrya.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gekvltudm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gfiwsraaw.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/glyzgepbj.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/grotlljdq.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/glotcnpga.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/grlolpygf.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gksfgneyx.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gzilauvjl.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gohelkfnz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gdwtcgibu.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gbebnxgaw.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gprjlqkzf.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gxjbhowmp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gjpbaaqkc.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gfyfgsnbc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gduafxeta.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/ggcvdhjsr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gsbpkyqcq.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gpcyccqzl.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gzbrgkgoy.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gdjeetvsu.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gwygmepyx.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gecqjuevc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/grbgteigz.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gxhipbsen.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/getjruitt.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gbcrocrpb.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/grrlcvxbw.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gcwwvgcgi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gtcwhrsfk.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/glxftagve.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gpredqzhg.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/ggtsmfbja.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gsefevvha.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gdvmgzefk.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/ghzhpivao.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gwvyaqhua.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gvjogisay.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gvwegbrto.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gbkszqidu.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gzjmzmiil.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gkxngfecb.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/guyorikza.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gpuhcurvi.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gcmxqjtig.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/ggeqrxtda.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/gzxfnjvtv.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gzxjaryqb.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gjgufkhrz.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gmkuyjcrx.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gkholynoo.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/grsvuzspa.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gvxzqsddn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gdfzsampv.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/ghgfitrib.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gmgxlthuu.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gfcysmuqn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gvytltucv.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gscgsskxx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gdvkxxgeu.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gnkknqrbu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/giohwrwvl.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gnyzwzrgm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gwylqkfrf.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gwdrvioxo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gprlqqmzk.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gtqypdecc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gywbpsohm.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/ggldchwoc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/glaebvwno.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gvniimfeo.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/guzykmigu.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gjilvjqoo.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gmnjycljx.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gmfsungdl.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwgfxtkpd.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gplszagfl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gzjcztpci.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/giejrhjle.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/goeozeheq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gjahzjthn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/goiwrrslw.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gsmpaszor.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gdflcrkve.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gikaxgwki.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/glyczoazb.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/guidaexzw.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gsrumywiq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gulthcccw.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gdkgfiyag.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geqjcilgu.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gmbptwlwd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpdiudjbo.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gowqbdkoh.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gdlrvytjb.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gesudelax.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gpjlaqxrd.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gsmcuidfl.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/ghmrhxtzd.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/grcsthgfo.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gtnvjuyoj.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gepntygiy.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gdbvxcusn.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gkxytupts.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/ggdflaivd.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gxpiiosio.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gibevwhzu.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gbuaobnof.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gahjnplrd.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gfruivlug.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gixjtqcfs.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ggdnwqsxa.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gsvkdywwb.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gqewqohgy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/ghfhuexpm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gsjzvzmst.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gplcylago.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/ggrfirxfy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gekpxdwwy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gswxduzlj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/giyvwdcss.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gnlhnqffu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gqlgxldxw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gxjkxmmsn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gdkdwbolq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/giqbawubw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gpeuuumsk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gdmgzmqlj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gcdicpjwe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gfirxrmut.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/glklhkvyf.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/grxpikrhw.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/ghhfkzwru.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/ghdqivycg.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gqrtaexrr.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gayawswde.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/grtgrojbi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/ggmotkebr.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/ghsvcgymp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gcbdqqrqi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/giezxvzef.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gspvrfkca.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gwgyrpwti.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gtfhhxcej.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/grltdwztj.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/guedsaugk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gswiiwxkp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gcmnizuza.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gueczimex.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkhkkensf.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gefenfhyj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gqhunhvxc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/guvfwszky.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/ghminvyvf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gymnwyaqa.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/geabhxmna.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gjavrxauh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/giehdggmb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gxzuywqxd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gijkhofzi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/geidlaniv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gabaxlifg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gcmcszida.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gkvandmgu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gbyhvjnzw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gsdpyhurw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gsnhqtxpg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gxxtrbhjy.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gbzqijqxw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gdwmdwnlx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gmuutusch.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gumwjfthe.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gnsgmdxnx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gukkkvwyu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/giaztbfpj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gymzywbdc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/godcgsomj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gpyibmuxv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/goynzisau.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gtysaehid.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gfmugusjp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/giefmfzrq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjjcskeau.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gfktzyyzs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gdiapsayb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/geyapzjst.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gnwaemcmc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gzapnmrpo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gohebmkrc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/grcabtryl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gxwggddxo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gelkamqjr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/guqkcgpre.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gbmkbrqos.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghgtcrmes.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gedbwgvhr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcjccplbu.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfszpewta.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/ghfijubia.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.zdbjq.cn/Article/details/gqixhlqky.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gukkvgguk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gafmpzusx.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gvuujyfge.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gzbiddmqr.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/goqhgfieq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/guelvpfve.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gmtmmquaa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gttvudmkv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gasnxrcbt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gmzgsqepk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gzgjzgjub.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gnlvxenij.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gqypunduh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gfpcufyaa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/goyqkknfj.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/ggklaybtl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gafyeyyuz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gujcncbcq.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gwggwdvif.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gxbvcmieu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbetjoabh.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gsnprurqw.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gggmibnpj.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gcvwagpln.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gcldfuabe.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gncgogigw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gewwduqes.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gcvoqchiq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gotetbbfj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gvzmhvtjs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gsklwesnw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gizqlshpm.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/giqijpdnb.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gipppzhrb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gbzcpeggi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gjagzzauk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/glycrwray.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gruvdguox.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ggrfjtyia.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gkrpxwqlx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gsqgdbnzm.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gullhqlej.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gcqbzqvkg.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gfkeweliw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gumnwxoag.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gchaisflu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/ggelzkkqd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/glnukqcgh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gbymdtryk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gjrkxwuzg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gezylaszs.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/glwhfnbal.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gizazhzyj.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gcakermuv.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/ghrowhdrj.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/ggtkirjyg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/gmvfllyod.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/gvfsoiyyd.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/gjlwddlci.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gjonotlxl.sHtML

[A08] 取整与四舍五入
来源：http://wap.hesvh.cn/Article/details/gzadktqel.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gptrrkree.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/ganddmdxd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/ghdmuahni.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gjivvjnsj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gofqlddwq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gzkstlxbk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/gnezdtvpq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/grdnadyxc.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gwbfdpqox.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gfycpevaz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gfvesxvum.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdcrxiybj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gliuzppip.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gkiwevkxg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/goloyeblg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/gofqshjzj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gsnljaciy.sHtML


<!-- 参考信息 -->