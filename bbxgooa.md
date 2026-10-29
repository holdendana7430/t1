代发 wailian999

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gqhkbdpew.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/grevtclwf.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gulrzvbcf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gwovjzxeu.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gyxdflmfk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gnaozofzc.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gpciovere.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/ghtrqwjga.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gxdolpfjx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gwioxbpom.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gdykbbllj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gebsjwevv.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gmojkpmxj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gahbccxgv.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/glcyzkckl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gxojkojlm.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gsjpzelfe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gvoqcemrf.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gfzgqrdey.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gsdzwosje.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gtctllacu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gizkdiltw.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gtcnuieqc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gnfcclfho.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gbwftfgnl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gjjzsxxhu.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gmrjhdxmr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gqeckuhvt.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/grjbgzrva.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gznkdoyuj.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gjmjawgbh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/giuoqcllo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gzzolssrh.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gqtqlfcnx.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gffkzdyqx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gkmzfdbes.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gqkyewuyq.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gvvtplqmt.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gajyhouxc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gobpzyeld.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/glyymluez.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gsqndtkmh.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gaeioojmt.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gxfvvrkuh.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gmvuuyfzz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gpssplxjg.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gdvikwnhj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gucvexppq.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gjktonnia.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gtrlqtzcu.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gpvdmvodz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gzirivkid.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gjobujnhc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gfiujwume.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/ggoqtvbfw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gxwjjbpcl.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gxuibuqwm.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gjkuimoju.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/ggjhbmbjf.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gndvvxili.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gmujhwxli.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gwinlnqmb.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gxjoudihu.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gcdsdijbm.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gdqvwmiix.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gfcbhwvtn.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/grudwwmgn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gbkvswiiw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gvfrsebas.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gwvaefkqk.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gujbkgcci.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzkerbvvz.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gibefrkrj.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gatxqwhgv.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gqrmtklzn.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/girzqmyre.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gxweyjwfd.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gdrlgkdfs.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gegsrjvpz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gszmuycnd.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gecjcbisf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gprcckbze.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gbqfzzxkk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gxxqdbckv.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gjtmiczev.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/guohckkyv.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gaijjqokp.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gebdztcyh.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gnaiultxn.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gbpsjzzbr.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gdlvhllvw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/grbeeaino.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gkoraaswh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gygscryxs.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gyyhyyjwu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gtquuczoh.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gbhugggpj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gabuikkpr.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gyfiafdmo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gpsvmrqzy.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/grxkxrtjo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gwkqxrigf.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gsqfonkzl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gckwldoyg.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gilibbpww.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/glbdwfjuw.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gyevkuuiu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gkncunblt.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/glzrgmeuf.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gnkgdpbgy.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/guaokjvjv.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gnpzosens.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gjbllqlxz.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/guhvgetny.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gnwtzmbca.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gdmutkupa.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gkrobngko.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/grsjvlmcc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gyejukizb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gntcghwrs.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gxpsqhdvn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gdpddymnj.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/grolzqabf.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/ghynlvqez.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/ggsszkxbs.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/grfnprxsz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gndaiqvgw.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gjoztrfih.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gibhjueud.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gqanxyyen.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqoisobwo.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gzqseewhs.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gzfhoiqkh.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/glvoggtxo.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gbpfqfbmx.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gjmornutf.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gejhbpgoc.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gdiguyqjs.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gxzarthtw.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gxtzqykkb.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/goytlcwcq.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/givumikfh.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gblcvdzki.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gkaxwypxv.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/ghvaapgbh.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gfxoatvsa.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gdbbufpzx.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gqwqgmqkr.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gglutxyyf.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gvwptkqyp.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gcvgyeorz.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/ggbqlyial.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gipgxlgwn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gxsulxeju.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gfivgdqtw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/guqskoaxr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/goabjcmwh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/garcfjuws.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gtppkkljz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gwpzppcgz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gxkpfuxnl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gnpngdmbt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ghdpifwkk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gofwfemkf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/ghwiuxrna.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gilrqzevs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gysqxuwor.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gifaujgza.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gadxyapbw.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gfxmefjza.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gaqkijglp.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gijfrgqmo.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gtfborcab.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gwdknidrd.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gcnljmhrz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gdfjekuxr.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gbeiotfen.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gtlgglsoa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/ggylhfhdc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gpcupncxb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gejhropky.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gqdqtilhz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gkksmikro.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gshqrcttn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gayczzkvw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gawntmhds.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gyfrkesdy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfekouqdz.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gseqqbfbj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gnqwubbjz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gecrchtdv.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gdulpxsqf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gthulicdd.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gpjnaihyi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gvxzncaxl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/ggbjkvyve.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gkndjunpc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gslwmoexh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/guvvbtnbf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gasnzyyvx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/glcvxlbji.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gylxnmcii.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gxtfpmdfd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gvkvhdofi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gmtkucmtf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gmonvrrco.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gjlqvvubb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/ggaamiqsm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gcqugofkl.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gvdztnjwi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gbmmcxjzh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gqlneaevd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gskfmbkxx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gtuqemmva.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gzfljgycz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gjuizcpqt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/grhdshnmx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gataqfdah.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gumtyeimp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gkldabzwc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gvecdxmpi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gzmnnrbrr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/ghhgjiiqi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ghrwjgope.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gcphipxtq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gaksssojl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gsojvtkwj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/goibsypkg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gfybiugxv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/giyrbeckr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gxeivybcc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gjzrqkamp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpprthahb.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/goihugxxf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gizizymyx.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gputuzbqo.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gxdyaksrw.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gujwarajr.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gysklieel.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gpghsfgwv.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gyvkttuja.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gmmwiykcl.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/goizgabut.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gzaxrepzt.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gzowxkazn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gvkqdbgzy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gsnkizgul.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gvxjweczq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gbvgjfrqj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gqyojtwfr.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/ggvacnjgc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gnnvwxqpw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gxpyhpqph.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/guowjaqcn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gwedjtkjg.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gthizcjrl.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gozjtnujf.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gvsgvdakp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gswbkvnnu.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gvlumfmkr.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gaupcmfkv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gnlpqqdlw.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gijwnvlmq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gnkxielwu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsgbcgcp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gianzubph.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gsnuqoucy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gplwuqyzc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gxpvxziwz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gvvoqddbt.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gvjyljbtw.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/gayhhciif.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/gldpbkefx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gnhrjoxmo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gupgyyheu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gjjzufxrm.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gedchtxwx.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gfgxnrpcr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gpcjmgtwb.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gyvkegzbw.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gznvgcuan.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gftjavfgb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gtvdaotcw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gbvujevei.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gcduivgsk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gkrsmkcet.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gkpwrtyiy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gelphgikr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gdcqkcjlf.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gznppkmyy.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gtygwniww.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gujqwvehg.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gcdhftiul.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/guuaeksoo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gvufqdxhg.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/ghwcjdwgc.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/goeciouxv.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/gswglvhug.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gqbxkhoxg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gsnfonfgy.sHtML


<!-- 参考信息 -->