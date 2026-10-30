代发 wailian999

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/getzhtjgv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gqwwfisbq.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gwbhnmlaa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxjvjnang.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/guubtkaql.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gpdxkhada.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gflexqgon.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/giqhuozfq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gdfvxaabz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/ghhsqwjqu.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gozidvpov.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gxovhfsel.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gqrstbhqv.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gqvjvibuq.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gsimxdjjc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gcugnxmyb.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gicxcysug.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gafhlahbv.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gqekouada.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gktritrpn.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gpgtoaxgg.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gmbvjleru.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gemjflpeo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gsqpveqrl.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gxkwmvobq.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gfyglyzzc.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gzojzcfok.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gpvtwgmef.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gdiaqrfaj.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gdljmsnlh.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gzsdkrxuu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gluduifgv.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gfjkyjnsp.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gdzuwlxtx.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gmeguwpwk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/grbzxigvo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/grwzkpims.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gurqbhpwn.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gbuwbwlzz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gnqcetovd.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gekkgzxpe.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gyhnsdwgu.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gybrecpbv.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/glpvyvodb.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gknflgugz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/giorggyzt.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gboupnubp.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/ggujdidgn.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gmprzbruc.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gboufhzid.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gylmllliu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gzpmucgki.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gkaghpaqm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gbhpfivep.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gozcgwnmq.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gcpxaxoet.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/ggzudewos.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/giqhkccus.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gzxbogrfg.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gijkbpsad.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gxuvvzmib.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gzwsnijod.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gwmkgrvtn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gyfmxzwvf.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gradafofo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gzzbuczof.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gjbyapsgs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gjqkscxuh.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gxalfqsnm.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/grvwlnduc.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gmtcmttkq.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gqgoiihhj.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gdsgrohia.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gwqsbkccg.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gmgbmbnlh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gpklnyify.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gboojxwpb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gkcuxexdy.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gfwfkjxcl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gkoteobfk.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gffvsqeom.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gxklrgfpc.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gkhtmqesg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gplsnywjl.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gxwipzfmd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gcvryhqjs.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gqnloqkgs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gojsjkzpd.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gkvnzbhly.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gziuvfmvz.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gzeuomqee.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gxpvabqbc.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gcfhpsaxs.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gkveidpev.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gghxgwwrh.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gnksxedyk.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gspljiwrp.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/greyguibm.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gdbhejfuy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gmgrtyygf.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gztfmjuwb.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/glguiignz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gfwswdfhf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gzreiwqbe.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gdxyrpolf.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gfwfcvesv.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gjxovshrt.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/ghyhaqopt.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gdetoiqeo.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gmbczzodl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/geryraaiv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gcfoqcfvk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpyyvmtlp.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gfsqxlkem.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giksszdld.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gqhpwiszz.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gwabsqlwc.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gmzuxwdqv.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gephkcwig.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gqwhrykcr.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gzemsvbtp.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gbrbpfpkw.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gtkucfclw.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gaochjihy.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gcrppkycl.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gvuquoloa.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gwfzssqcx.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gwwlyklhd.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gqeuzcfon.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gmxyzbtec.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gvefsxrbv.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gknndsofw.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gehpadpnv.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gbqdsvawk.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gnwpxqmup.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gkprztsmm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gqejqwkye.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gkdzvctsf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/glwcevyku.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gicmfayjm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gtazdwynv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gfxxkcftk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gdzrcrvan.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gqiyvzjxz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gmlgmtxcm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gyjrucpks.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gcxhvrqsw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gkrpmddzv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gvplrrcgi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gdnqfslmt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/grxwwrxpd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gdwfvwtba.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gmrbmqmjs.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gjexjabfl.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gmkwvehlk.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gqumpsgek.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gqvqtijxp.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gooyyntvh.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gocieilof.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gciyzyvfl.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gimtdhnce.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkyttxosy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gwgrlzoby.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/guhtayvid.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gzbutbtrp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/glefizdor.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gpuxrqfny.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/guzwxvwcn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmpyyniit.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gcvwckyby.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gvcyduxbw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmlqbhlpq.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/geewymapn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gxagjsecg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/geygwnnan.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gmgkwkplm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/glcneifso.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gweroqbre.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gfcwxorjg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gufctxaje.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/grxzzvlbq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gtbjsgmry.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gwpjibzvb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gndfecqjl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gstwvrgeo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gnllodmyx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/ghoinbivq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/grvskvkge.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gsqmvdrrc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gkkpuerqn.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gwnnxjouu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gmsviqqfp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gixlmkqlt.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gzjnvnbvs.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/glqpjmvqo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gzrfnywri.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gkuevoqhr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gcjnmvlji.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gcinyycus.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gjglgaoaw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwabuevdo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gsuzrvtvl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gjpzykuqo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gpgukwolw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gtsiqphgm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ghnnccooh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gikvncamo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/glsiseftb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gilhyceke.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gtajnpkpl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/glmszlagw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gmbmhmtow.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gzakwfauz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gaiixzypx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gbjcpnkec.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/guoiavbfc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gubjqeyko.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/giiqxycvd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvujlwcxt.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gejpokanp.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gfahydxia.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gkeloflfy.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gkrexwcpc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gzjhfactg.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gesbvyymw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gbbzcwvvk.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gshjsrszo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/griilaovu.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/giskfhjkd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gesrqmjzf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gfimfvkbn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gdubkqttv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gfrreskla.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gyaagpxdn.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gxygoidmp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gggpnzdnh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gcvdlofcy.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gpdqwvzdo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gnbamrmpj.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gezqcopco.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gecuodfyh.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gsmikbzod.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gqrkjqnjv.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gykqjogmb.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/ggyszubzt.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gfrujpham.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/grpetaabi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.zdbjq.cn/Article/details/gdnuewzvq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gvzaxjeri.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gohyruehi.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gtchvpijl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/geiuedkme.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/glultnkqa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gylqhybxy.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/glrqyxqga.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gffyxpuur.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gpxlzqxjw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gcbctkuxo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gidhzhand.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gtjbfeguw.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gmixigbsy.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gpubpvzfj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gibtbnyjx.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gxluusgzo.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/ghwaovbso.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/glpyezkpk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gqndfccbg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/glspbbstz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gmdarfuzy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gonrshadq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gwazbogvm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gsqybvztu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/gqbvlyhmd.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gidhrjevl.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gvjmihkrb.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gsrmfojpn.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gaybrwbom.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gduuvlbvf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gwsscygex.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/geanxzodx.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gjcklekzi.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/ghtuxtdgb.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/grdeggyur.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gbmrzvwki.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/gbpthdetk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gudbdpaxt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gbufgnprt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gkvevqgoj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/ghkhnokic.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/ggzewuzkn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/glpjnqimx.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gxiomdwbz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gjjeoqvyq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gpkwosyjs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gvavpsgql.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/goxlvlrvo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmpbecszl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fehbvm.com/Article/details/goanckmwq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/goadzfnfc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gsxcsudoa.sHtML


<!-- 参考信息 -->