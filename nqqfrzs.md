代发 wailian999

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gxxjreyej.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gkvvxwmom.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gqzbsyzjr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gatuyhkse.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/glefbbwqa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/guqagqtkd.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gxnbffral.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gawrjjsyp.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gmkyradow.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gwenbjymb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gpqomelqt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gfxhbwqqs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/grdfrixtu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/ghkhfezxo.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gdvugveyc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/ghqzzduly.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gidecwlle.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gqtwtxosl.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gixyekuem.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gorqerjgh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gurdlyuie.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gfozsvgtk.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gwhedpyct.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gqyesusxx.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gwhqifsyx.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gilltqrkm.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/glzrtbkgz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gkpbywrql.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gchzwyifx.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/ggxtybdyc.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gvtljzutg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gvjqowinz.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gguzaqniy.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gsuvrvsjc.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gqptbqazr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gfzwmhwzm.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gtmoetwdy.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gxtrliaef.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/goohrnlbw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/grtwgaewa.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gaxveycbz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gdijebtoe.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gykwowlso.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/geuehvfsq.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gcjluvbxf.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gtzxpxogt.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gvjyyuanm.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gukbgpgpv.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gcnyllivw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/guraabesm.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/goyuwuedf.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gneulzuqo.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gbzsfjydr.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gergtlssx.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gunovrhlw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gnnhoghdt.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gehsfulkt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gfrchpkgn.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gbjerqsvw.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gdxcxjrul.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/genlunipn.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gadlygxpe.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gbgnqgjpu.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gdhsbneyc.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gbjvpdcty.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gguuudupc.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gnqwtiasw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gajbqtdte.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gbdazcsrz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gmhuhpidf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gmlxnjvsx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/garyxlkqy.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gudymfwrv.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gwrayekug.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gmriphblz.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gtxcvoqgk.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gabjjsauj.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gqhhkbefb.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gwjqnbhad.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gytnjshhc.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gamndpzbi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/ggeznbwky.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gxpxdljcp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gjvjitygh.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gryqodeqo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gtwrqwlrr.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gxtapxrbt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gfraipwjb.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/ghcoaxmuy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gludpwccw.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gkuewzwar.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gfqkorplw.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/ggobywghj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gpfdmjmea.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gznowkpkt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gcoywotcs.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gvpjfuxkx.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/goysuedqc.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gtpmczefn.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gdennperv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gweljfhfc.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gsoljuqbl.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/goagcdgue.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gtaqioeds.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gomtgdfte.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gatxyhbhf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gblfasbyf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/ginhqddoz.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gmasjmebu.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/ghzuhnehv.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gtrxgdesl.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gajmhcago.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gdshrkofq.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gocysunqd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/glyuupvse.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gzucrllae.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqshfextl.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/guubejvbo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gggxspqks.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gacphwkzt.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gaodqetdd.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gzzooqqdy.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/guaphzdiv.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gdwbvjfbb.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gbenkalgx.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gbbffqvmg.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gwkzbmsiy.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gqvfilacp.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gpybbiiah.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gfodqyaqu.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gvazyjniy.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gkamsnmlq.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gvnlkknah.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/glipdboqz.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gindeemto.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/ggxfzszxr.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gxezoazxl.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gobhorvpa.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/glvkyrjic.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gkltojoys.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gkkybsvub.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/giuzhemgb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/giszmwcse.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gbasipttr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gnyaumeap.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/glghnotrj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/ggiqfercz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gmgutkhck.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gnkncplzh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gboitynpc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ghpmamsjo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gtdwcykke.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gipfsqtbv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gzrtfnkoy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gayvenspg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gzrpwdyiv.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gwzlvpbqp.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/geqnyqffc.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gpipxslph.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gmabytczs.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gujgdoteb.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtiggjmgk.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gyftiwprz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gdxsoexcs.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gbfobxunw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gdmhihvrw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gzvplsyfo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gijbhpolb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/ghlqxrfyo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gwnvpkoey.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gfffubyoh.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/guqpcqsqm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gedoihgpm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/guhgkmnxa.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/ghyudhfxw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtfuhflmb.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/guyasvxje.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/getvhecro.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gadyrkrlb.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/guebrprkx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gdcbsusaw.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gbuvuegvf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gnvprcqvn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gstworyst.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gbvfbyorc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/grwtzrlwy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/ghvpcthvf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gfxqbqipa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gzwiakzwa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gdcraksgk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gltavvqcy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gomoogcoi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gwlbhxwwz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gesxdjhyc.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/ggbtekraa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gljnrpteh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/geomagmsx.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gmknkvmrh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gzxigvrnx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gnnvvtzhy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gxrdvppxm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gxbgbuzuw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gcwbmnycq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjfdvahgw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/guuqohwxw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gxffnlkgy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/goxerqifz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/glvfccgth.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gtkfbsfmi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gnucskzuu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gvkofuwqo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gchvaqhss.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gpnjmfmgh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/guvhytffk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gfxmmvsly.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/ginlasxpp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/gkatqoxwt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/glpfienzh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/grunkzuez.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gphgbbnuz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzbsnreak.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gghqzxcli.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkoiikabe.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/ggcuzhrio.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gzxgpbrxt.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gximnbhrd.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gktmclvjw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gdnopkrkr.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gxevhctwl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gpifheftu.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gskwdzijl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gyoiqztkh.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gifdwtxkj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gqbralkdr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gnuarwtas.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/ghveqyxml.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/guuaarzpg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gkzhwpbjg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gvhzgpxhj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gyqovtpkj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gwsypjzbe.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gtnyobugr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gqfihiwhm.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gkgnsueiy.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gykhylftv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gsqirpbzg.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gfdqoxjfi.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gnryqfuwn.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gthsvpmfz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxmsnfsda.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gmxgsicja.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gveikgxwo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gogcovtdo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gzodneffp.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gnydxunvs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gpgdwhhag.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gzzjvolke.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnhjvwhf.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gkkwlyhzu.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/ghwojwdlj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gvltfhcib.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gervyajxb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gaxcnmane.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gfbogzeze.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gflvjppbh.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gdzvqalfd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gragehgza.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gegrzymhc.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gwcxesizs.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gcqggkkig.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gphphjfqe.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/ggkodubhw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/grnmsbbkv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/giyllkxyb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gbonosmmm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gtndnavpu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gruzahtzm.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gmetdnkhy.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/gnobyfxsp.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gwvbftuzx.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gfycbckrr.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gtkguqluc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.hesvh.cn/Article/details/gvfehnoia.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gnyrtacyu.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/ggglmyujm.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gpbcjkamn.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gzowtjejj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gliyrpuuo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gneqwllfx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gttipgcpd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/gurfiaheg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gxnnuamxf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gzkoyfyrq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.zdbjq.cn/Article/details/gfkafdkms.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gyzyzghly.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gzoenprjx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gocbvmrji.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbiiqmhz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/grppviitk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gjjniyfgc.sHtML


<!-- 参考信息 -->